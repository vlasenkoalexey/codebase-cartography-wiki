---
title: 'Module: tree_sitter_analyzer/mcp/utils/project_index/_toon.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/project_index/_toon.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.project_index._toon`/
symbols:
  render_toon: render_toon().
  _render_scale: _render_scale().
  _render_core: _render_core().
  _render_tooling: _render_tooling().
  _render_header: _render_header().
  _render_critical: _render_critical().
  _render_entry: _render_entry().
  _append_dir_line: _append_dir_line().
  _TOON_DIR_COL._TOON_DIR_COL: _TOON_DIR_COL._TOON_DIR_COL.
  _classify_top_level_dirs: _classify_top_level_dirs().
  _render_context: _render_context().
  _NON_CODE_LANGUAGES._NON_CODE_LANGUAGES: _NON_CODE_LANGUAGES._NON_CODE_LANGUAGES.
---
# Module: [`tree_sitter_analyzer/mcp/utils/project_index/_toon.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py)

## Functions
- `_append_dir_line(lines: list[str], name: str, desc: str)` — [`L186`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L186) — Append one ``<name>/  <desc>`` line to the TOON output.
- `_classify_top_level_dirs(root_path: Path, structure: list[dict[str, Any]], classify_dir_fn: Any)` — [`L110`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L110) — Partition top-level dirs into (core, context, tooling) buckets.
- `_render_context(lines: list[str], context_dirs: list[dict[str, Any]])` — [`L159`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L159) — Emit ``context:`` section with file counts only (no descriptions).
- `_render_core(lines: list[str], core_dirs: list[dict[str, Any]], index: ProjectIndex)` — [`L135`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L135) — Emit ``core:`` section with first-7 dirs + first-4 subdirs each.
- `_render_critical(lines: list[str], index: ProjectIndex)` — [`L74`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L74) — Emit the ``critical:`` section (top-7 PageRank nodes).
- `_render_entry(lines: list[str], index: ProjectIndex)` — [`L102`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L102) — Emit the ``entry:`` line from the first entry point.
- `_render_header(lines: list[str], root_path: Path, index: ProjectIndex)` — [`L66`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L66) — Emit ``project:`` / ``what:`` lines.
- `_render_scale(lines: list[str], index: ProjectIndex)` — [`L87`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L87) — Emit the ``scale:`` line — total files + top-2 language shares.
- `_render_tooling(lines: list[str], tooling_dirs: list[dict[str, Any]], index: ProjectIndex)` — [`L171`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L171) — Emit ``tooling:`` section with first-3 dirs and descriptions.
- `render_toon(index: ProjectIndex, classify_dir_fn: Any)` — [`L23`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L23) — Render the project index as TOON-format text.

## Module values
- `_NON_CODE_LANGUAGES` — [`L16`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L16)
- `_TOON_DIR_COL` — [`L20`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_toon.py#L20)

