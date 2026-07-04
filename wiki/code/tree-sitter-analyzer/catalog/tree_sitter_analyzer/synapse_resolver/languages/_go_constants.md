---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages._go_constants`/
symbols:
  parse_go_import_block: parse_go_import_block().
  _strip_go_comments: _strip_go_comments().
  STDLIB_IMPORT_PATHS_GO.STDLIB_IMPORT_PATHS_GO: STDLIB_IMPORT_PATHS_GO.STDLIB_IMPORT_PATHS_GO.
  STDLIB_PACKAGES_GO.STDLIB_PACKAGES_GO: STDLIB_PACKAGES_GO.STDLIB_PACKAGES_GO.
  _GO_IMPORT_SPEC: _GO_IMPORT_SPEC.
  _GO_IMPORT_KEYWORD: _GO_IMPORT_KEYWORD.
  _GO_STRING_OR_COMMENT: _GO_STRING_OR_COMMENT.
  _strip_go_comments._repl: _strip_go_comments()._repl().
  __all__: __all__.
  EXTERNAL_PACKAGES_GO.EXTERNAL_PACKAGES_GO: EXTERNAL_PACKAGES_GO.EXTERNAL_PACKAGES_GO.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py)

## Functions
- `_repl(m: re.Match[str])` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L130)
- `_strip_go_comments(raw: str)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L121) — Remove Go ``//`` and ``/* */`` comments, preserving string literals.
- `parse_go_import_block(raw: str)` — [`L138`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L138) — Parse a Go import-block string into ``{qualifier -> stdlib package}``.

## Module values
- `EXTERNAL_PACKAGES_GO` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L89)
- `STDLIB_IMPORT_PATHS_GO` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L43)
- `STDLIB_PACKAGES_GO` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L82)
- `_GO_IMPORT_KEYWORD` — [`L101`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L101)
- `_GO_IMPORT_SPEC` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L96)
- `_GO_STRING_OR_COMMENT` — [`L112`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L112)
- `__all__` — [`L192`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/_go_constants.py#L192)

