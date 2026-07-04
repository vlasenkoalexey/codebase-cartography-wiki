---
title: 'Module: tree_sitter_analyzer/hyphae/ast.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/hyphae/ast.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.hyphae.ast`/
symbols:
  SelectorList: SelectorList#
  PseudoClass.arg: PseudoClass#arg.
  SelectorList.selectors: SelectorList#selectors.
  Selector: Selector.
  SimpleSelector.base: SimpleSelector#base.
  SimpleSelector: SimpleSelector#
  Combined: Combined#
  SimpleSelector.pseudo_classes: SimpleSelector#pseudo_classes.
  PseudoClass: PseudoClass#
  AttributeSelector: AttributeSelector#
  PseudoClass.name: PseudoClass#name.
  SimpleSelector.attributes: SimpleSelector#attributes.
  Combined.left: Combined#left.
  Combined.right: Combined#right.
  Combined.combinator: Combined#combinator.
  AttributeSelector.name: AttributeSelector#name.
  AttributeSelector.value: AttributeSelector#value.
---
# Module: [`tree_sitter_analyzer/hyphae/ast.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py)

## Classes
### `AttributeSelector`
- def: [`tree_sitter_analyzer/hyphae/ast.py:13`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L13)
- doc: An `[name=value]` filter, e.g. `[file=src/lib.rs]`.
- signature: `class AttributeSelector:`
- members:
  - `name` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L16)
  - `value` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L17)
- used by: [`_parse_simple`](parser.md#_Parser._parse_simple), [`_eval_simple`](evaluator.md#Evaluator._eval_simple), [`_parse_attribute`](parser.md#_Parser._parse_attribute), [`attributes`](ast.md#SimpleSelector.attributes)  (1 test-only)

### `Combined`
- def: [`tree_sitter_analyzer/hyphae/ast.py:48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L48)
- doc: Two selectors joined by a combinator (`>` child, `~` sibling, descendant).
- signature: `class Combined:`
- members:
  - `combinator` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L52)
  - `left` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L51)
  - `right` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L53)
- uses (calls/refs, reference-scoped): [`Selector`](ast.md#Selector)
- used by: [`_parse_selector`](parser.md#_Parser._parse_selector), [`_eval_combined`](evaluator.md#Evaluator._eval_combined), [`_eval_selector`](evaluator.md#Evaluator._eval_selector), [`Selector`](ast.md#Selector)  (2 test-only)

### `PseudoClass`
- def: [`tree_sitter_analyzer/hyphae/ast.py:21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L21)
- doc: A pseudo-class filter such as `:calls(#x)`, `:not(.struct)`, `:in(src/)`.
- signature: `class PseudoClass:`
- members:
  - `arg` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L31)
  - `name` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L30)
- uses (calls/refs, reference-scoped): [`SelectorList`](ast.md#SelectorList)
- used by: [`_apply_pseudo`](evaluator.md#Evaluator._apply_pseudo), [`_parse_simple`](parser.md#_Parser._parse_simple), [`_parse_pseudo`](parser.md#_Parser._parse_pseudo), [`pseudo_classes`](ast.md#SimpleSelector.pseudo_classes)  (4 test-only)

### `SelectorList`
- def: [`tree_sitter_analyzer/hyphae/ast.py:60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L60)
- members:
  - `selectors` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L63)
- uses (calls/refs, reference-scoped): [`Selector`](ast.md#Selector)
- used by: [`parse`](parser.md#parse), [`eval`](evaluator.md#Evaluator.eval), [`_apply_pseudo`](evaluator.md#Evaluator._apply_pseudo), [`parse`](parser.md#_Parser.parse), [`arg`](ast.md#PseudoClass.arg), [`_target_names`](evaluator.md#Evaluator._target_names), [`_parse_pseudo_arg`](parser.md#_Parser._parse_pseudo_arg), [`_filter_edge`](evaluator.md#Evaluator._filter_edge), [`_filter_has`](evaluator.md#Evaluator._filter_has), [`_filter_imports`](evaluator.md#Evaluator._filter_imports)  (10 test-only)

### `SimpleSelector`
- def: [`tree_sitter_analyzer/hyphae/ast.py:35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L35)
- doc: A single selector unit: a base plus attribute and pseudo-class filters.
- signature: `class SimpleSelector:`
- members:
  - `attributes` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L43)
  - `base` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L42)
  - `pseudo_classes` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L44)
- uses (calls/refs, reference-scoped): [`PseudoClass`](ast.md#PseudoClass), [`AttributeSelector`](ast.md#AttributeSelector)
- used by: [`_parse_simple`](parser.md#_Parser._parse_simple), [`_eval_simple`](evaluator.md#Evaluator._eval_simple), [`_target_names`](evaluator.md#Evaluator._target_names), [`Selector`](ast.md#Selector)  (8 test-only)

## Module values
- `Selector` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/ast.py#L56)

