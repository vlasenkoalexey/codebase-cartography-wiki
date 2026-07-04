---
title: 'Module: tree_sitter_analyzer/hyphae/parser.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/hyphae/parser.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.hyphae.parser`/
symbols:
  parse: parse().
  _Parser._parse_simple: _Parser#_parse_simple().
  _Parser._parse_attribute: _Parser#_parse_attribute().
  _Parser._parse_pseudo: _Parser#_parse_pseudo().
  _Parser._advance: _Parser#_advance().
  HyphaeSyntaxError: HyphaeSyntaxError#
  _Parser._peek: _Parser#_peek().
  _Parser.parse: _Parser#parse().
  _Parser._parse_selector: _Parser#_parse_selector().
  _Parser._next_combinator: _Parser#_next_combinator().
  _Parser._expect: _Parser#_expect().
  _Parser._parse_pseudo_arg: _Parser#_parse_pseudo_arg().
  _Parser._skip_ws: _Parser#_skip_ws().
  _Parser._read_value_text: _Parser#_read_value_text().
  _Parser._pos: _Parser#_pos.
  _COMBINATORS: _COMBINATORS.
  _Parser.__init__: _Parser#__init__().
  _Parser._tokens: _Parser#_tokens.
  _BASE_TOKENS: _BASE_TOKENS.
  _Parser: _Parser#
---
# Module: [`tree_sitter_analyzer/hyphae/parser.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py)

## Classes
### `HyphaeSyntaxError`  ·  implements/extends ValueError
- def: [`tree_sitter_analyzer/hyphae/parser.py:30`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L30)
- doc: Raised when a Hyphae selector string is malformed.
- signature: `class HyphaeSyntaxError(ValueError):`
- used by: [`execute`](../mcp/tools/hyphae_select_tool.md#HyphaeSelectTool.execute), [`_apply_pseudo`](evaluator.md#Evaluator._apply_pseudo), [`_parse_simple`](parser.md#_Parser._parse_simple), [`_parse_attribute`](parser.md#_Parser._parse_attribute), [`parse`](parser.md#_Parser.parse), [`_expect`](parser.md#_Parser._expect), [`_filter_edge`](evaluator.md#Evaluator._filter_edge), [`_filter_has`](evaluator.md#Evaluator._filter_has), [`_filter_imports`](evaluator.md#Evaluator._filter_imports), [`_read_value_text`](parser.md#_Parser._read_value_text), [`_filter_position`](evaluator.md#Evaluator._filter_position)  (3 test-only)

### `_Parser`
- def: [`tree_sitter_analyzer/hyphae/parser.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L34)
- signature: `class _Parser:`
- members:
  - `_next_combinator(self)` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L85) — Return the combinator joining the current and next simple selector.
  - `_read_value_text(self)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L157) — Read an attribute value: IDENT path, or a #name / .kind literal.
  - `parse(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L58)
- protocol/private: `__init__`[`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L35), `_advance`[`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L42), `_expect`[`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L47), `_parse_attribute`[`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L144), `_parse_pseudo`[`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L171), `_parse_pseudo_arg`[`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L183), `_parse_selector`[`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L75), `_parse_simple`[`L114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L114), `_peek`[`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L39), `_pos`[`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L37), `_skip_ws`[`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L53), `_tokens`[`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L36)
- uses (calls/refs, reference-scoped): [`HyphaeSyntaxError`](parser.md#HyphaeSyntaxError), [`SelectorList`](ast.md#SelectorList), [`arg`](ast.md#PseudoClass.arg), [`Token`](lexer.md#Token), [`value`](lexer.md#Token.value), [`Selector`](ast.md#Selector), [`base`](ast.md#SimpleSelector.base), [`Combined`](ast.md#Combined), [`SimpleSelector`](ast.md#SimpleSelector), [`pseudo_classes`](ast.md#SimpleSelector.pseudo_classes), [`PseudoClass`](ast.md#PseudoClass), [`AttributeSelector`](ast.md#AttributeSelector), [`name`](ast.md#PseudoClass.name), [`attributes`](ast.md#SimpleSelector.attributes), [`left`](ast.md#Combined.left), [`right`](ast.md#Combined.right), [`combinator`](ast.md#Combined.combinator), [`_COMBINATORS`](parser.md#_COMBINATORS), [`name`](ast.md#AttributeSelector.name), [`value`](ast.md#AttributeSelector.value), [`_BASE_TOKENS`](parser.md#_BASE_TOKENS)
- used by: [`parse`](parser.md#parse)

## Functions
- `parse(text: str)` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L195) — Parse a Hyphae selector string into a :class:`SelectorList`.

## Module values
- `_BASE_TOKENS` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L26)
- `_COMBINATORS` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/hyphae/parser.py#L27)

