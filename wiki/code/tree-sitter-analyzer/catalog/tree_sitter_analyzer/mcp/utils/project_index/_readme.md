---
title: 'Module: tree_sitter_analyzer/mcp/utils/project_index/_readme.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/project_index/_readme.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.project_index._readme`/_
symbols:
  _excerpt_from_blockquotes: excerpt_from_blockquotes().
  _excerpt_from_paragraphs: excerpt_from_paragraphs().
  _is_language_count_excluded: is_language_count_excluded().
  _clean_readme_line: clean_readme_line().
  _is_readme_noise_line: is_readme_noise_line().
  _read_directory_readme_title: read_directory_readme_title().
---
# Module: [`tree_sitter_analyzer/mcp/utils/project_index/_readme.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_readme.py)

## Functions
- `_clean_readme_line(line: str)` — [`L26`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_readme.py#L26) — Strip markdown formatting and HTML tags from a README line.
- `_excerpt_from_blockquotes(text: str)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_readme.py#L63) — First non-noise blockquote line in ``text``, cleaned and truncated.
- `_excerpt_from_paragraphs(text: str)` — [`L81`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_readme.py#L81) — First non-noise non-blockquote line in ``text``, cleaned and truncated.
- `_is_language_count_excluded(filepath: str)` — [`L14`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_readme.py#L14) — True if ``filepath`` should not influence language_distribution.
- `_is_readme_noise_line(line: str)` — [`L37`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_readme.py#L37) — Return True for README lines that are not useful descriptions.
- `_read_directory_readme_title(readme_path: Path)` — [`L98`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/project_index/_readme.py#L98) — Return the first meaningful line from a directory's README.md.

