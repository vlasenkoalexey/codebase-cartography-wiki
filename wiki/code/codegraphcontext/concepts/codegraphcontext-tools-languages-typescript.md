---
title: TypeScript/TSX language extractor
type: concept
provenance: mixed
concept: codegraphcontext-tools-languages-typescript
concepts: [multi-language-extraction, symbol-graph]
updated: 2026-07-04
status: fresh
---
# TypeScript/TSX language extractor

<!-- connect:up:begin -->
> **Cross-repo concept:** part of [multi-language-extraction](../../../concepts/multi-language-extraction.md), [symbol-graph](../../../concepts/symbol-graph.md) across this wiki's repos.
<!-- connect:up:end -->
How CodeGraphContext turns a `.ts`/`.tsx` file into the language-agnostic bag of graph nodes
(functions, classes, interfaces, type aliases, variables, imports, calls) that the indexer later
stitches into the code graph — and the TypeScript-specific syntax it has to handle to do so.

## Overview
`TypescriptTreeSitterParser` is one of 23 per-language extractors that all speak the same protocol:
a `parse()` method returns a dict of node lists keyed by kind, and a family of `_find_*` methods each
run a tree-sitter query and reshape the captures into plain Python dicts. There is no TypeScript type
checker here and no semantic model — everything is *syntactic*, recovered by matching s-expression
queries ([`TS_QUERIES`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TS_QUERIES))
against the parse tree and walking parent/child links. The single design idea that makes this
comparable to the Kotlin extractor is the shared seam: most extractors funnel their query
through the version-tolerant [`execute_query`](../catalog/src/codegraphcontext/utils/tree_sitter_manager.md#execute_query),
so "which grammar / which tree-sitter API" is solved once and each language file only decides *what
to capture and how to shape it* (Emacs Lisp is the one exception — it walks the tree directly via
its own node-iteration helper rather than calling `execute_query`). What is distinctly TypeScript here is the surface it must cover:
interfaces, type aliases, decorators, `extends`/`implements` heritage, `require()` and dynamic
`import()`, and the many ways a function can be written (declaration, arrow, method, expression,
member assignment).

## Diagram
```mermaid
flowchart TD
    P["parse(path, index_source)"] --> FN["_find_functions"]
    P --> CL["_find_classes"]
    P --> IF["_find_interfaces"]
    P --> TA["_find_type_aliases"]
    P --> IM["_find_imports"]
    P --> CA["_find_calls"]
    P --> VA["_find_variables"]
    FN --> EQ["execute_query"]
    CL --> EQ
    CA --> EQ
    CA --> DI["_find_dynamic_imports"]
    DI --> EQ
    EQ --> TSQ["TS_QUERIES"]
    FN --> BK["_bucket_for / _key"]
    FN --> XP["_extract_parameters"]
    FN --> CX["_calculate_complexity"]
    CL --> DEC["_collect_preceding_decorators"]
    CA --> PC["_get_parent_context"]
    EQ -.node.text.-> GT["_get_node_text"]
```

## Design rationale (why it's built this way)
The interesting engineering is in `_find_functions`, and it exists because tree-sitter captures
are *flat*. A single functions query ([`TS_QUERIES`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TS_QUERIES))
matches seven different function shapes — `function_declaration`, arrow/expression assigned to a
`variable_declarator`, single-param arrows, `method_definition`, and functions assigned to a
`member_expression` — and emits `@name`, `@params`, `@single_param`, and `@function_node` captures
independently, with no guarantee they arrive grouped by function. So the parser has to *re-associate*
them. It does this by walking each capture up to its enclosing function node and bucketing by a
byte-range identity key, which is the whole reason [`_bucket_for`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._bucket_for),
[`_key`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._key),
[`_fn_for_name`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._fn_for_name)
and [`_fn_for_params`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._fn_for_params)
exist. Contrast the simpler extractors — [`_find_interfaces`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_interfaces)
and [`_find_type_aliases`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_type_aliases)
just read `child_by_field_name('name')` off one node — which shows the complexity is inherent to
JS/TS's many function forms, not the framework.

A second deliberate choice: TypeScript's structural type layer (`interface`, `type`) is captured as
first-class node kinds. [`parse`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parse)
returns `interfaces` and `type_aliases` alongside functions and classes — categories that have no
analogue in the Python or Kotlin extractors — so the graph can represent purely-typed declarations
that never appear at runtime.

> [!inferred]
> These type-level categories only carry name + line range (plus optional source), not their member
> lists or the types they reference, so downstream the graph likely models an interface as a node
> with no edges to the properties it declares. That is a shallowness the code makes visible but does
> not resolve here.

## Entry points
- [`parse`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parse)
  — the sole public entry. The indexer calls it per `.ts`/`.d.ts` file; it reads the file, parses it
  with the cached tree-sitter [`parser`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parser),
  fans out to the seven `_find_*` extractors, and returns one dict tagged with
  [`language_name`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.language_name).
  The `index_source` flag it stores in [`index_source`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.index_source)
  decides whether each node also carries its raw source text.
- [`parse`](../catalog/src/codegraphcontext/tools/languages/typescriptjsx.md#TypescriptJSXTreeSitterParser.parse)
  (TSX) — the sibling `.tsx` entry point, reached by dynamic dispatch (base→override). Its docstring
  says it "reuse[s] TypeScript logic and ensuring JSX nodes are handled": it calls the same
  `_find_*` methods, then adds a React-component pass on top. This is the concrete way the TS
  extractor is *shared* rather than duplicated.

## Mechanism (step-by-step)
1. **Read and parse.** [`parse`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parse)
   opens the file as UTF-8, feeds the bytes to the tree-sitter [`parser`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parser),
   and takes `tree.root_node`. Everything downstream is a query or a walk over that one tree; there is
   no second pass or symbol resolution.

2. **Run queries through the shared seam.** Each `_find_*` method looks up its query string in
   [`TS_QUERIES`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TS_QUERIES)
   and runs it via [`execute_query`](../catalog/src/codegraphcontext/utils/tree_sitter_manager.md#execute_query),
   which normalizes tree-sitter 0.20/0.22+/0.25 capture-return shapes into a uniform list of
   `(node, capture_name)` tuples. Every text read then goes through the one-liner
   [`_get_node_text`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._get_node_text)
   (`node.text.decode('utf-8')`).

3. **Reassemble functions from flat captures.** [`_find_functions`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_functions)
   iterates the captures and, for each `@name`/`@params`/`@single_param`, walks up to the owning
   function node via [`_fn_for_name`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._fn_for_name)
   or [`_fn_for_params`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._fn_for_params),
   then merges them into a per-function bucket keyed by byte-range identity
   ([`_bucket_for`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._bucket_for)
   over [`_key`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._key)).
   `_fn_for_name` is what handles arrows/expressions bound to a `variable_declarator` or
   `assignment_expression` — it dives into the declarator's children to find the actual function
   node so an assigned arrow is attributed to its variable name.

4. **Extract each function's shape.** For each assembled bucket it pulls parameter names with
   [`_extract_parameters`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._extract_parameters)
   — which unwraps TypeScript's typed parameter forms (`required_parameter` and `optional_parameter`
   carry a `pattern` field under a `type_annotation`; `rest_pattern` becomes `...name`; defaults come
   from `assignment_pattern`) so the stored arg is the bare identifier, not the type. It attaches a
   nesting context via [`_get_parent_context`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._get_parent_context),
   a cyclomatic count via [`_calculate_complexity`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._calculate_complexity),
   and any TS/decorator annotations from [`_collect_preceding_decorators`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._collect_preceding_decorators).

5. **Classes with heritage and decorators.** [`_find_classes`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_classes)
   captures `class_declaration`, `abstract_class_declaration` and anonymous `class`, then reads the
   `class_heritage` child to split `extends_clause` and `implements_clause` into a flat `bases` list —
   so both superclass and implemented interfaces become inheritance edges. Decorators are recovered
   by [`_collect_preceding_decorators`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._collect_preceding_decorators),
   which scans sibling nodes *before* the class, skipping `export`/`default`/`async`/`comment`, and
   uses [`_same_node`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._same_node)
   (byte-range + type equality) to know when it has reached the class itself.

6. **Type-level declarations.** [`_find_interfaces`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_interfaces)
   and [`_find_type_aliases`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_type_aliases)
   are the TypeScript-only extractors: each captures one node kind, reads its `name` (a
   `type_identifier`), and records name + line span, optionally with source when
   [`index_source`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.index_source)
   is set.

7. **Imports, static and dynamic.** [`_find_imports`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_imports)
   walks `import_statement` clauses — bare, default (`identifier`), namespace (`* as`), and
   `named_imports` (each `import_specifier` yielding name + optional alias) — and also treats a
   `require(...)` call as an import. Runtime `import(...)` is handled separately by
   [`_find_dynamic_imports`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_dynamic_imports),
   which [`_find_calls`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_calls)
   invokes first so those become import edges (tagged `call_kind: "dynamic_import"`) rather than
   ordinary calls.

8. **Calls and variables.** [`_find_calls`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_calls)
   captures `call_expression`/`new_expression` callee identifiers, walks up to the enclosing call node
   to gather arguments, and records both a function context and a class context via two calls to
   [`_get_parent_context`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._get_parent_context)
   (the second scoped to class-declaration types). [`_find_variables`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_variables)
   captures `variable_declarator` names but deliberately *skips* declarators whose value is a
   function/arrow — those are already emitted as functions in step 3 — avoiding double-counting.

## Key data structures
- [`TS_QUERIES`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TS_QUERIES) — the dict
  of s-expression query strings (`functions`, `classes`, `interfaces`, `type_aliases`, `imports`,
  `calls`, `variables`, `docstrings`). This is the extractor's declarative core; the `_find_*` methods
  are just the imperative reshaping around each query.
- The per-kind result dicts returned by [`parse`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parse):
  each is a plain dict with `name`, `line_number`, and kind-specific fields (`bases`/`decorators` for
  classes, `args`/`cyclomatic_complexity`/`context` for functions, `source`/`alias` for imports), all
  tagged with [`language_name`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.language_name).
  This uniform shape is the contract the language-agnostic indexer consumes.
- The `captures_by_function` bucket built by [`_bucket_for`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._bucket_for) —
  transient state that exists only to re-group flat captures into functions.

## Dynamics (design intent)
Extraction is purely static and single-file: [`parse`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parse)
never crosses file boundaries or resolves an imported symbol to its definition — it only records that
an import/call/base *name* appears, leaving name-to-node linking to a later indexing stage. Complexity
counting bounds its own recursion: [`_calculate_complexity`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._calculate_complexity)'s
inner [`traverse`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.traverse)
stops at [`MAX_AST_DEPTH`](../catalog/src/codegraphcontext/tools/indexing/constants.md#MAX_AST_DEPTH)
(200) and, when it hits the cap, emits a
[`warning_logger`](../catalog/src/codegraphcontext/utils/debug_log.md#warning_logger) message — whose
docstring is "Log warning message if log level allows" — that is gated by
[`_should_log`](../catalog/src/codegraphcontext/utils/debug_log.md#_should_log) /
[`_get_config_value`](../catalog/src/codegraphcontext/utils/debug_log.md#_get_config_value)
against the configured level in [`LOG_LEVELS`](../catalog/src/codegraphcontext/utils/debug_log.md#LOG_LEVELS)
before reaching the module [`logger`](../catalog/src/codegraphcontext/utils/debug_log.md#logger). So the
depth cap trades a possibly-undercounted metric for a guarantee it never blows the stack on a
pathological AST.

## Edge cases
- **Missing tree-sitter.** If the tree-sitter import fails, [`execute_query`](../catalog/src/codegraphcontext/utils/tree_sitter_manager.md#execute_query)
  raises the actionable error from [`_missing_tree_sitter_error`](../catalog/src/codegraphcontext/utils/tree_sitter_manager.md#_missing_tree_sitter_error)
  (which specifically flags Python 3.13's missing cp313 wheels) rather than a bare `ImportError`.
- **Docstrings are always `None`.** [`_get_docstring`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._get_docstring)
  is a stub returning `None`, and `_find_functions` sets `docstring = None` unconditionally — so
  functions/classes never carry extracted doc text even though `TS_QUERIES` defines a `docstrings`
  query. JSDoc is captured by the grammar but not surfaced here.
- **Function-valued variables are not variables.** [`_find_variables`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._find_variables)
  `continue`s on `function_expression`/`arrow_function` values (and any type containing "function"/
  "arrow"), so `const f = () => …` is a function node, not a variable node.
- **Anonymous / assigned functions.** Naming leans entirely on the parent walk in
  [`_fn_for_name`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._fn_for_name)
  and [`_get_parent_context`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser._get_parent_context);
  a truly anonymous function with no declarator/assignment/property parent yields no name and is
  dropped (`if not name: continue`).

## Open questions
- The subgraph doesn't include `_find_react_components` (called by the TSX
  [`parse`](../catalog/src/codegraphcontext/tools/languages/typescriptjsx.md#TypescriptJSXTreeSitterParser.parse)),
  so exactly how JSX components are distinguished from ordinary functions is out of scope for this page.
- `generic_parser_wrapper` supplies [`language`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.language),
  [`parser`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.parser),
  and [`language_name`](../catalog/src/codegraphcontext/tools/languages/typescript.md#TypescriptTreeSitterParser.language_name)
  but is not in the subgraph, so how the `.ts` vs `.tsx` grammar is selected upstream isn't settled here.

## See also
- [Tree-sitter grammar management & multi-language extraction](codegraphcontext-utils-tree_sitter_manager.md)
  — the [`execute_query`](../catalog/src/codegraphcontext/utils/tree_sitter_manager.md#execute_query)
  seam and grammar loader every extractor shares.
- Sibling per-language extractors: `codegraphcontext-tools-languages-kotlin.md` and
  `codegraphcontext-tools-languages-elisp.md` — same `parse` + `_find_*` protocol, different syntax
  surface (no interfaces/type-aliases/decorators, different function forms).
- The cross-repo `multi-language-extraction` and `symbol-graph` concept pages under
  `wiki/concepts/` comparing this grounding substrate against wikify-repo, graphify, and
  understand-anything.
