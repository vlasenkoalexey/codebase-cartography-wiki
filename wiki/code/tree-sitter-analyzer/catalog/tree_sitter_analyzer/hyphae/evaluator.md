---
title: 'Module: tree_sitter_analyzer/hyphae/evaluator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/hyphae/evaluator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.hyphae.evaluator`/
symbols:
  Evaluator.eval: Evaluator#eval().
  Evaluator._apply_pseudo: Evaluator#_apply_pseudo().
  Evaluator._eval_simple: Evaluator#_eval_simple().
  Evaluator: Evaluator#
  Evaluator._eval_base: Evaluator#_eval_base().
  Evaluator._target_names: Evaluator#_target_names().
  Evaluator._eval_selector: Evaluator#_eval_selector().
  Evaluator._eval_combined: Evaluator#_eval_combined().
  Evaluator._filter_edge: Evaluator#_filter_edge().
  Evaluator._filter_imports: Evaluator#_filter_imports().
  Evaluator._filter_has: Evaluator#_filter_has().
  Evaluator.total_matches: Evaluator#total_matches().
  Evaluator.was_truncated: Evaluator#was_truncated().
  Evaluator._cache: Evaluator#_cache.
  Evaluator._symbols_of_kind: Evaluator#_symbols_of_kind().
  _key: _key().
  Evaluator._all_functions: Evaluator#_all_functions().
  _EDGE_PSEUDOS._EDGE_PSEUDOS: _EDGE_PSEUDOS._EDGE_PSEUDOS.
  Evaluator._filter_position: Evaluator#_filter_position().
  _INHERIT_KINDS: _INHERIT_KINDS.
  Evaluator._max: Evaluator#_max.
  Evaluator._was_truncated: Evaluator#_was_truncated.
  Evaluator._total_count: Evaluator#_total_count.
  _FUNCTIONISH: _FUNCTIONISH.
  _CLASSISH: _CLASSISH.
  _POSITION_PSEUDOS: _POSITION_PSEUDOS.
  Evaluator._apply_attribute: Evaluator#_apply_attribute().
  Evaluator.__init__: Evaluator#__init__().
---
# Module: [`tree_sitter_analyzer/hyphae/evaluator.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py)

## Classes
### `Evaluator`
- def: [`tree_sitter_analyzer/hyphae/evaluator.py:73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L73)
- doc: Evaluate a parsed Hyphae selector against an `ASTCache`.
- signature: `class Evaluator:`
- members:
  - `_filter_edge(self, cands: list[dict[str, Any]], arg: Any, edge_kinds: tuple[str, ...], target_col: str, return_col: str)` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L227) — Keep candidates joined to the target selector by any ``edge_kinds`` edge.
  - `_filter_has(self, cands: list[dict[str, Any]], arg: Any)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L297) — Keep candidates that contain a member matching the target selector.
  - `_filter_imports(self, cands: list[dict[str, Any]], arg: Any)` — [`L274`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L274) — Keep candidates whose file imports a module matching the target.
  - `_filter_position(self, cands: list[dict[str, Any]], name: str, arg: Any)` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L316) — Position filters within each containing class (ordered by line).
  - `_target_names(self, arg: SelectorList)` — [`L346`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L346) — Extract target symbol names from a pseudo-class argument selector.
  - `eval(self, selector_list: SelectorList)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L83) — Evaluate the selector and return capped results.
  - `total_matches(self)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L138) — Return the total number of matches (before cap, if truncated).
  - `was_truncated(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L142) — Return whether the results were capped at max_results.
- protocol/private: `__init__`[`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L76), `_all_functions`[`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L180), `_apply_attribute`[`L190`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L190), `_apply_pseudo`[`L204`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L204), `_cache`[`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L77), `_eval_base`[`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L161), `_eval_combined`[`L361`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L361), `_eval_selector`[`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L147), `_eval_simple`[`L152`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L152), `_max`[`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L78), `_symbols_of_kind`[`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L183), `_total_count`[`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L80), `_was_truncated`[`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L79)
- uses (calls/refs, reference-scoped): [`HyphaeSyntaxError`](parser.md#HyphaeSyntaxError), [`SelectorList`](ast.md#SelectorList), [`arg`](ast.md#PseudoClass.arg), [`selectors`](ast.md#SelectorList.selectors), [`base`](ast.md#SimpleSelector.base), [`Combined`](ast.md#Combined), [`SimpleSelector`](ast.md#SimpleSelector), [`pseudo_classes`](ast.md#SimpleSelector.pseudo_classes), [`PseudoClass`](ast.md#PseudoClass), [`name`](ast.md#PseudoClass.name), [`attributes`](ast.md#SimpleSelector.attributes), [`left`](ast.md#Combined.left), [`right`](ast.md#Combined.right), [`_key`](evaluator.md#_key), [`combinator`](ast.md#Combined.combinator), [`_EDGE_PSEUDOS`](evaluator.md#_EDGE_PSEUDOS._EDGE_PSEUDOS), [`name`](ast.md#AttributeSelector.name), [`value`](ast.md#AttributeSelector.value), [`_CLASSISH`](evaluator.md#_CLASSISH), [`_FUNCTIONISH`](evaluator.md#_FUNCTIONISH), [`_POSITION_PSEUDOS`](evaluator.md#_POSITION_PSEUDOS)
- used by: [`execute`](../mcp/tools/hyphae_select_tool.md#HyphaeSelectTool.execute), [`read_hyphae_resource`](../mcp/resources/hyphae_resource.md#read_hyphae_resource), [`_evaluate`](../mcp/watch_push_bridge.md#_drive_subscriptions._evaluate)  (28 test-only)

## Functions
- `_key(sym: dict[str, Any])` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L69)

## Module values
- `_CLASSISH` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L46)
- `_EDGE_PSEUDOS` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L55)
- `_FUNCTIONISH` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L45)
- `_INHERIT_KINDS` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L54)
- `_POSITION_PSEUDOS` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/evaluator.py#L66)

