---
title: 'Module: tree_sitter_analyzer/rename_symbol.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/rename_symbol.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.rename_symbol`/
symbols:
  rename_symbol: rename_symbol().
  RenameSite: RenameSite#
  _apply_rename_to_file: _apply_rename_to_file().
  RenameSite.line: RenameSite#line.
  RenameSite.column: RenameSite#column.
  RenameSite.file: RenameSite#file.
  RenameSite.site_type: RenameSite#site_type.
  RenameResult.to_dict: RenameResult#to_dict().
  RenameSite.old_text: RenameSite#old_text.
  _collect_rename_sites_from_resolver: _collect_rename_sites_from_resolver().
  _sites_from_defn: _sites_from_defn().
  _sites_from_ref: _sites_from_ref().
  _deduplicate_sites: _deduplicate_sites().
  RenameSite.to_dict: RenameSite#to_dict().
  _is_word_boundary: _is_word_boundary().
  _scan_line_for_name: _scan_line_for_name().
  RenameResult.sites: RenameResult#sites.
  _group_sites_by_file: _group_sites_by_file().
  _find_identifier_at_or_near: _find_identifier_at_or_near().
  RenameResult.files_changed: RenameResult#files_changed.
  RenameResult: RenameResult#
  RenameResult.symbol: RenameResult#symbol.
  RenameResult.new_name: RenameResult#new_name.
  RenameResult.dry_run: RenameResult#dry_run.
  RenameResult.sites_renamed: RenameResult#sites_renamed.
  RenameResult.errors: RenameResult#errors.
  _WORD_CHARS: _WORD_CHARS.
  _has_unknown_cols: _has_unknown_cols().
  _apply_col_rename: _apply_col_rename().
  _read_backup: _read_backup().
  _rollback_file: _rollback_file().
  logger: logger.
---
# Module: [`tree_sitter_analyzer/rename_symbol.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py)

## Classes
### `RenameResult`
- def: [`tree_sitter_analyzer/rename_symbol.py:48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L48)
- signature: `class RenameResult:`
- members:
  - `to_dict(self)` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L57)
  - `dry_run` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L51)
  - `errors` — [`L55`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L55)
  - `files_changed` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L52)
  - `new_name` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L50)
  - `sites` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L54)
  - `sites_renamed` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L53)
  - `symbol` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L49)
- uses (calls/refs, reference-scoped): [`RenameSite`](rename_symbol.md#RenameSite), [`to_dict`](rename_symbol.md#RenameSite.to_dict)
- used by: [`rename_symbol`](rename_symbol.md#rename_symbol), [`execute`](mcp/tools/codegraph_refactor_tool.md#CodeGraphRefactorTool.execute)  (6 test-only)

### `RenameSite`
- def: [`tree_sitter_analyzer/rename_symbol.py:30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L30)
- signature: `class RenameSite:`
- members:
  - `to_dict(self)` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L37)
  - `column` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L33)
  - `file` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L31)
  - `line` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L32)
  - `old_text` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L34)
  - `site_type` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L35)
- used by: [`execute`](mcp/tools/codegraph_refactor_tool.md#CodeGraphRefactorTool.execute), [`_apply_rename_to_file`](rename_symbol.md#_apply_rename_to_file), [`to_dict`](rename_symbol.md#RenameResult.to_dict), [`_collect_rename_sites_from_resolver`](rename_symbol.md#_collect_rename_sites_from_resolver), [`_sites_from_defn`](rename_symbol.md#_sites_from_defn), [`_sites_from_ref`](rename_symbol.md#_sites_from_ref), [`_deduplicate_sites`](rename_symbol.md#_deduplicate_sites), [`sites`](rename_symbol.md#RenameResult.sites), [`_group_sites_by_file`](rename_symbol.md#_group_sites_by_file)  (17 test-only)

## Functions
- `_apply_col_rename(line_text: str, col: int, name_len: int, old_name: str, new_name: str)` — [`L218`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L218) — Apply a single-column rename to line_text if the candidate matches.
- `_apply_rename_to_file(file_path: str, sites: list[RenameSite], old_name: str, new_name: str)` — [`L231`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L231)
- `_collect_rename_sites_from_resolver(resolve_result: Any, old_name: str, project_root: str)` — [`L182`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L182)
- `_deduplicate_sites(sites: list[RenameSite])` — [`L193`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L193)
- `_find_identifier_at_or_near(line_text: str, column: int, target_name: str)` — [`L80`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L80)
- `_group_sites_by_file(sites: list[RenameSite])` — [`L204`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L204)
- `_has_unknown_cols(line_sites: list[Any])` — [`L213`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L213) — Return True if any site has an unknown column or line position.
- `_is_word_boundary(text: str, pos: int)` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L74)
- `_read_backup(abs_path: str)` — [`L272`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L272) — Read file content for rollback backup; return None on OSError.
- `_rollback_file(fpath: str, orig_content: str, root: str)` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L281) — Restore a single file to its original content during rollback.
- `_scan_line_for_name(line_text: str, name: str)` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L99)
- `_sites_from_defn(defn: Any, old_name: str, project_root: str)` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L114) — Collect rename sites for a single definition entry.
- `_sites_from_ref(ref: Any, old_name: str, project_root: str)` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L143) — Collect rename sites for a single reference entry.
- `rename_symbol(cache: Any, old_name: str, new_name: str, dry_run: bool = True, project_root: str | None = None)` — [`L291`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L291)

## Module values
- `_WORD_CHARS` — [`L69`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L69)
- `logger` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/rename_symbol.py#L26)

