---
title: 'Module: src/extraction/function-ref.ts'
type: catalog
provenance: extracted
module: src/extraction/function-ref.ts
status: fresh
symbol_base: scip-typescript npm @colbymchenry/codegraph 1.2.0 src/extraction/`function-ref.ts`/
symbols:
  captureFnRefCandidates: captureFnRefCandidates().
  CaptureRule.mode: CaptureRule#mode.
  normalizeValue: normalizeValue().
  FN_REF_SPECS: FN_REF_SPECS.
  normalizeSpecial: normalizeSpecial().
  cFamilySpec: cFamilySpec().
  CaptureRule.field: CaptureRule#field.
  NormalizedRef.node: NormalizedRef#node.
  TS_JS_SPEC: TS_JS_SPEC.
  CSHARP_SPEC: CSHARP_SPEC.
  RUBY_SPEC: RUBY_SPEC.
  SWIFT_SPEC: SWIFT_SPEC.
  FnRefSpec: FnRefSpec#
  NormalizedRef.name: NormalizedRef#name.
  LUA_SPEC: LUA_SPEC.
  FnRefSpec.dispatch: FnRefSpec#dispatch.
  PYTHON_SPEC: PYTHON_SPEC.
  GO_SPEC: GO_SPEC.
  JAVA_SPEC: JAVA_SPEC.
  KOTLIN_SPEC: KOTLIN_SPEC.
  SCALA_SPEC: SCALA_SPEC.
  DART_SPEC: DART_SPEC.
  PASCAL_SPEC: PASCAL_SPEC.
  PHP_SPEC: PHP_SPEC.
  CaptureRule: CaptureRule#
  FnRefSpec.idTypes: FnRefSpec#idTypes.
  RUST_SPEC: RUST_SPEC.
  lastNamedOfType: lastNamedOfType().
  phpStringContent: phpStringContent().
  phpEnclosingCallName: phpEnclosingCallName().
  FnRefSpec.layers: FnRefSpec#layers.
  FnRefSpec.special: FnRefSpec#special.
  rubyEnclosingCall: rubyEnclosingCall().
  FnRefCandidate.name: FnRefCandidate#name.
  FnRefCandidate.mode: FnRefCandidate#mode.
  isRubyHookCall: isRubyHookCall().
  FnRefSpec.unwrap: FnRefSpec#unwrap.
  FnRefSpec.ungatedModes: FnRefSpec#ungatedModes.
  FnRefCandidate: FnRefCandidate#
  CaptureMode: CaptureMode#
  NormalizedRef: NormalizedRef#
  NormalizedRef.skipGate: NormalizedRef#skipGate.
  FnRefCandidate.line: FnRefCandidate#line.
  FnRefCandidate.column: FnRefCandidate#column.
  FnRefCandidate.explicitRef: FnRefCandidate#explicitRef.
  FnRefCandidate.skipGate: FnRefCandidate#skipGate.
  FnRefSpec.addressOfOnly: FnRefSpec#addressOfOnly.
  NAME_STOPLIST: NAME_STOPLIST.
  cFamilySpec.extra-typeLiteral0.special: cFamilySpec().(extra)typeLiteral0:special.
  cFamilySpec.extra-typeLiteral0.addressOfOnly: cFamilySpec().(extra)typeLiteral0:addressOfOnly.
  RUBY_HOOK_RE: RUBY_HOOK_RE.
  RUBY_HOOK_NAMES: RUBY_HOOK_NAMES.
  PHP_CALLABLE_HOFS: PHP_CALLABLE_HOFS.
---
# Module: [`src/extraction/function-ref.ts`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts)

## Classes
### `CaptureMode`
- def: [`src/extraction/function-ref.ts:60`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L60) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- doc: How to pull candidate value nodes out of a dispatched container node.
- signature: `type CaptureMode`
- used by: [`mode`](function-ref.ts.md#CaptureRule.mode), [`cFamilySpec`](function-ref.ts.md#cFamilySpec), [`mode`](function-ref.ts.md#FnRefCandidate.mode), [`ungatedModes`](function-ref.ts.md#FnRefSpec.ungatedModes)

### `CaptureRule`
- def: [`src/extraction/function-ref.ts:67`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L67) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- signature: `interface CaptureRule`
- members:
  - `field` — [`L70`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L70) — Field holding the value for rhs/value/varinit (defaults per mode). — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `mode` — [`L68`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L68) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- uses (calls/refs, reference-scoped): [`CaptureMode`](function-ref.ts.md#CaptureMode)
- used by: [`captureFnRefCandidates`](function-ref.ts.md#captureFnRefCandidates), [`cFamilySpec`](function-ref.ts.md#cFamilySpec), [`TS_JS_SPEC`](function-ref.ts.md#TS_JS_SPEC), [`CSHARP_SPEC`](function-ref.ts.md#CSHARP_SPEC), [`RUBY_SPEC`](function-ref.ts.md#RUBY_SPEC), [`SWIFT_SPEC`](function-ref.ts.md#SWIFT_SPEC), [`LUA_SPEC`](function-ref.ts.md#LUA_SPEC), [`DART_SPEC`](function-ref.ts.md#DART_SPEC), [`GO_SPEC`](function-ref.ts.md#GO_SPEC), [`JAVA_SPEC`](function-ref.ts.md#JAVA_SPEC), [`KOTLIN_SPEC`](function-ref.ts.md#KOTLIN_SPEC), [`PASCAL_SPEC`](function-ref.ts.md#PASCAL_SPEC), [`PHP_SPEC`](function-ref.ts.md#PHP_SPEC), [`PYTHON_SPEC`](function-ref.ts.md#PYTHON_SPEC), [`SCALA_SPEC`](function-ref.ts.md#SCALA_SPEC), [`dispatch`](function-ref.ts.md#FnRefSpec.dispatch), [`RUST_SPEC`](function-ref.ts.md#RUST_SPEC)

### `FnRefCandidate`
- def: [`src/extraction/function-ref.ts:36`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L36) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- signature: `interface FnRefCandidate`
- members:
  - `column` — [`L39`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L39)
  - `explicitRef` — [`L47`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L47) — True when the value was an explicit reference form (`&fn`, `&Cls::m`,
  - `line` — [`L38`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L38)
  - `mode` — [`L41`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L41) — Which capture position produced this candidate (gate policy keys on it). — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `name` — [`L37`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L37) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `skipGate` — [`L56`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L56) — Skip the same-file/import name gate for this candidate. Set for PHP
- uses (calls/refs, reference-scoped): [`CaptureMode`](function-ref.ts.md#CaptureMode)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`captureFnRefCandidates`](function-ref.ts.md#captureFnRefCandidates), [`flushFnRefCandidates`](tree-sitter.ts.md#TreeSitterExtractor.flushFnRefCandidates), [`fnRefCandidates`](tree-sitter.ts.md#TreeSitterExtractor.fnRefCandidates)

### `FnRefSpec`
- def: [`src/extraction/function-ref.ts:73`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L73) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- signature: `interface FnRefSpec`
- members:
  - `addressOfOnly` — [`L117`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L117) — C++ only: in args/rhs/varinit positions, accept ONLY explicit reference
  - `dispatch` — [`L77`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L77) — Container node type → how to extract candidate values from it. — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `idTypes` — [`L75`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L75) — Bare identifier node types that can act as a function value. — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `layers` — [`L84`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L84) — Transparent wrapper layers between a container and its values — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `special` — [`L97`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L97) — Whole-node reference forms needing bespoke name extraction — — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `ungatedModes` — [`L107`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L107) — Capture modes whose candidates skip the same-file/import gate and rely on — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `unwrap` — [`L90`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L90) — Unary wrappers whose operand is the function value — C/C++ `&fn` — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- uses (calls/refs, reference-scoped): [`CaptureRule`](function-ref.ts.md#CaptureRule), [`CaptureMode`](function-ref.ts.md#CaptureMode)
- used by: [`tree-sitter.ts`](tree-sitter.ts.md#scip-typescript-npm-colbymchenry-codegraph-1.2.0-src-extraction-tree-sitter.ts), [`captureFnRefCandidates`](function-ref.ts.md#captureFnRefCandidates), [`flushFnRefCandidates`](tree-sitter.ts.md#TreeSitterExtractor.flushFnRefCandidates), [`normalizeValue`](function-ref.ts.md#normalizeValue), [`FN_REF_SPECS`](function-ref.ts.md#FN_REF_SPECS), [`cFamilySpec`](function-ref.ts.md#cFamilySpec), [`maybeCaptureFnRefs`](tree-sitter.ts.md#TreeSitterExtractor.maybeCaptureFnRefs), [`TS_JS_SPEC`](function-ref.ts.md#TS_JS_SPEC), [`CSHARP_SPEC`](function-ref.ts.md#CSHARP_SPEC), [`RUBY_SPEC`](function-ref.ts.md#RUBY_SPEC), [`SWIFT_SPEC`](function-ref.ts.md#SWIFT_SPEC), [`LUA_SPEC`](function-ref.ts.md#LUA_SPEC), [`DART_SPEC`](function-ref.ts.md#DART_SPEC), [`GO_SPEC`](function-ref.ts.md#GO_SPEC), [`JAVA_SPEC`](function-ref.ts.md#JAVA_SPEC), [`KOTLIN_SPEC`](function-ref.ts.md#KOTLIN_SPEC), [`PASCAL_SPEC`](function-ref.ts.md#PASCAL_SPEC), [`PHP_SPEC`](function-ref.ts.md#PHP_SPEC), [`PYTHON_SPEC`](function-ref.ts.md#PYTHON_SPEC), [`SCALA_SPEC`](function-ref.ts.md#SCALA_SPEC), [`RUST_SPEC`](function-ref.ts.md#RUST_SPEC), [`fnRefSpec`](tree-sitter.ts.md#TreeSitterExtractor.fnRefSpec)

### `NormalizedRef`
- def: [`src/extraction/function-ref.ts:514`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L514) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- doc: One normalized function-value: its name, source node, and gate policy.
- signature: `interface NormalizedRef`
- members:
  - `name` — [`L515`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L515) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `node` — [`L516`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L516) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
  - `skipGate` — [`L517`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L517)
- uses (calls/refs, reference-scoped): [`Node`](../web-tree-sitter.d.ts.md#Node)
- used by: [`captureFnRefCandidates`](function-ref.ts.md#captureFnRefCandidates), [`normalizeValue`](function-ref.ts.md#normalizeValue), [`normalizeSpecial`](function-ref.ts.md#normalizeSpecial)

## Functions
- `cFamilySpec(extra?: { special?: string[] | undefined; addressOfOnly?: boolean | undefined; } | undefined)` — [`L142`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L142) — C / C++ / Objective-C share the C-family initializer & assignment shapes. — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `captureFnRefCandidates(container: Node, rule: CaptureRule, spec: FnRefSpec, source: string)` — [`L408`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L408) — Extract candidate names from a dispatched container node. Returns the — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `isRubyHookCall(name: string)` — [`L284`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L284) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `lastNamedOfType(node: Node, types: Set<string>)` — [`L600`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L600) — Rightmost descendant-or-self named child of one of the given types. — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `normalizeSpecial(node: Node, type: string, source: string)` — [`L612`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L612) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `normalizeValue(node: Node, spec: FnRefSpec, source: string, depth: number)` — [`L525`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L525) — Normalize one value expression to zero or more function names. Recursion is — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `phpEnclosingCallName(node: Node)` — [`L822`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L822) — The function name of the PHP call whose arguments contain `node`, if any. — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `phpStringContent(node: Node, source: string)` — [`L813`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L813) — Content of a PHP string literal node (single- or double-quoted). — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `rubyEnclosingCall(node: Node)` — [`L837`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L837) — The Ruby `call` node whose argument_list (or keyword pair) contains `node`. — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)

## Module values
- `CSHARP_SPEC` — [`L250`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L250) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `DART_SPEC` — [`L310`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L310)
- `FN_REF_SPECS` — [`L376`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L376) — Capture specs by language. — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `GO_SPEC` — [`L201`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L201)
- `JAVA_SPEC` — [`L229`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L229)
- `KOTLIN_SPEC` — [`L240`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L240)
- `LUA_SPEC` — [`L322`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L322)
- `NAME_STOPLIST` — [`L121`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L121) — Names that are never function references even when grammars call them identifiers.
- `PASCAL_SPEC` — [`L332`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L332)
- `PHP_CALLABLE_HOFS` — [`L347`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L347) — PHP core functions whose string arguments are CALLABLES — the positional
- `PHP_SPEC` — [`L360`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L360)
- `PYTHON_SPEC` — [`L189`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L189)
- `RUBY_HOOK_NAMES` — [`L283`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L283)
- `RUBY_HOOK_RE` — [`L282`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L282) — Rails/ActiveSupport-style hook DSLs whose symbol arguments name a method of
- `RUBY_SPEC` — [`L262`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L262) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `RUST_SPEC` — [`L217`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L217)
- `SCALA_SPEC` — [`L300`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L300)
- `SWIFT_SPEC` — [`L288`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L288) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `TS_JS_SPEC` — [`L177`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L177) — documented in [extraction-function-ref.ts](../../../concepts/extraction-function-ref.ts.md)
- `addressOfOnly` — [`L142`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L142)
- `special` — [`L142`](../../../../../../raw/code/codegraph/src/extraction/function-ref.ts#L142)

