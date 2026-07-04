---
title: 'Module: tree_sitter_analyzer/code_similarity.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/code_similarity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.code_similarity`/
symbols:
  detect_structural_clones_cached: detect_structural_clones_cached().
  detect_structural_clones: detect_structural_clones().
  detect_textual_clones_cached: detect_textual_clones_cached().
  detect_textual_clones: detect_textual_clones().
  analyze_code_similarity: analyze_code_similarity().
  _extract_function_bodies: _extract_function_bodies().
  SimilarityGroup.functions: SimilarityGroup#functions.
  SimilarityResult.groups: SimilarityResult#groups.
  SimilarFunction.to_dict: SimilarFunction#to_dict().
  _extract_cached_functions: _extract_cached_functions().
  SimilarityGroup: SimilarityGroup#
  SimilarityGroup.to_dict: SimilarityGroup#to_dict().
  _matches_path_filter: _matches_path_filter().
  SimilarFunction: SimilarFunction#
  SimilarityGroup.method: SimilarityGroup#method.
  SimilarityResult.stats: SimilarityResult#stats.
  _text_fingerprint: _text_fingerprint().
  SimilarFunction.file: SimilarFunction#file.
  SimilarityResult.to_dict: SimilarityResult#to_dict().
  SimilarityGroup.fingerprint: SimilarityGroup#fingerprint.
  _extract_from_tree: _extract_from_tree().
  _body_snippet: _body_snippet().
  SimilarFunction.name: SimilarFunction#name.
  SimilarityGroup.similarity: SimilarityGroup#similarity.
  SimilarityResult: SimilarityResult#
  SimilarFunction.line: SimilarFunction#line.
  SimilarFunction.end_line: SimilarFunction#end_line.
  SimilarFunction.language: SimilarFunction#language.
  SimilarFunction.body_snippet: SimilarFunction#body_snippet.
  _ast_fingerprint: _ast_fingerprint().
  _ast_fingerprint._walk: _ast_fingerprint()._walk().
  _should_visit_dir: _should_visit_dir().
  logger: logger.
  _read_file_content: _read_file_content().
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  _FUNC_DEF_TYPES: _FUNC_DEF_TYPES.
  _source_hash: _source_hash().
  _split_path_filter: _split_path_filter().
---
# Module: [`tree_sitter_analyzer/code_similarity.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py)

## Classes
### `SimilarFunction`
- def: [`tree_sitter_analyzer/code_similarity.py:71`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L71)
- signature: `class SimilarFunction:`
- members:
  - `to_dict(self, include_snippet: bool = False)` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L79)
  - `body_snippet` — [`L77`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L77)
  - `end_line` — [`L75`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L75)
  - `file` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L72)
  - `language` — [`L76`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L76)
  - `line` — [`L74`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L74)
  - `name` — [`L73`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L73)
- used by: [`detect_structural_clones_cached`](code_similarity.md#detect_structural_clones_cached), [`detect_structural_clones`](code_similarity.md#detect_structural_clones), [`detect_textual_clones_cached`](code_similarity.md#detect_textual_clones_cached), [`detect_textual_clones`](code_similarity.md#detect_textual_clones), [`functions`](code_similarity.md#SimilarityGroup.functions), [`to_dict`](code_similarity.md#SimilarityGroup.to_dict)  (4 test-only)

### `SimilarityGroup`
- def: [`tree_sitter_analyzer/code_similarity.py:93`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L93)
- signature: `class SimilarityGroup:`
- members:
  - `to_dict(self, include_bodies: bool = False)` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L99)
  - `fingerprint` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L94)
  - `functions` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L97)
  - `method` — [`L95`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L95)
  - `similarity` — [`L96`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L96)
- uses (calls/refs, reference-scoped): [`to_dict`](code_similarity.md#SimilarFunction.to_dict), [`SimilarFunction`](code_similarity.md#SimilarFunction)
- used by: [`detect_structural_clones_cached`](code_similarity.md#detect_structural_clones_cached), [`detect_structural_clones`](code_similarity.md#detect_structural_clones), [`detect_textual_clones_cached`](code_similarity.md#detect_textual_clones_cached), [`detect_textual_clones`](code_similarity.md#detect_textual_clones), [`analyze_code_similarity`](code_similarity.md#analyze_code_similarity), [`groups`](code_similarity.md#SimilarityResult.groups), [`to_dict`](code_similarity.md#SimilarityResult.to_dict)  (7 test-only)

### `SimilarityResult`
- def: [`tree_sitter_analyzer/code_similarity.py:112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L112)
- signature: `class SimilarityResult:`
- members:
  - `to_dict(self, include_bodies: bool = False)` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L116)
  - `groups` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L113)
  - `stats` — [`L114`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L114)
- uses (calls/refs, reference-scoped): [`SimilarityGroup`](code_similarity.md#SimilarityGroup), [`to_dict`](code_similarity.md#SimilarityGroup.to_dict)
- used by: [`analyze_code_similarity`](code_similarity.md#analyze_code_similarity), [`execute`](mcp/tools/code_similarity_tool.md#CodeGraphSimilarityTool.execute)  (8 test-only)

## Functions
- `_ast_fingerprint(node: Any, source: str, max_depth: int = 15)` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L124) — Compute a structural fingerprint from an AST node.
- `_body_snippet(body: str, max_len: int = 200)` — [`L304`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L304)
- `_extract_cached_functions(cache: Any, project_root: str, min_lines: int = 5, path_filter: str | None = None)` — [`L430`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L430) — Extract function bodies using pre-indexed AST cache.
- `_extract_from_tree(node: Any, source: str, file_path: str, language: str, min_lines: int, results: list[tuple[str, str, int, int, str, str]])` — [`L273`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L273) — Walk AST and extract function bodies.
- `_extract_function_bodies(project_root: str, *, min_lines: int = 5, max_files: int = 1000, path_filter: str | None = None)` — [`L216`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L216) — Extract function bodies from source files.
- `_matches_path_filter(file_path: str, path_filter: str | None)` — [`L199`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L199) — Return True when file_path is allowed by the optional glob filter.
- `_read_file_content(path: str)` — [`L173`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L173) — Read file content as text, returning None on OSError.
- `_should_visit_dir(d: str)` — [`L168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L168) — Return True if directory should be walked (not excluded, not hidden).
- `_source_hash(source: str)` — [`L182`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L182) — Return the same content hash format used by the AST cache.
- `_split_path_filter(path_filter: str | None)` — [`L187`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L187) — Return normalized glob patterns from a comma/semicolon separated filter.
- `_text_fingerprint(source_text: str)` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L146) — Compute a normalized text fingerprint.
- `_walk(n: Any, depth: int)` — [`L133`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L133)
- `analyze_code_similarity(project_root: str, *, mode: str = "all", min_lines: int = 5, min_group_size: int = 2, max_files: int = 1000, max_groups: int = 30, use_cache: bool = True, path_filter: str | None = None)` — [`L633`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L633) — Comprehensive code similarity analysis.
- `detect_structural_clones(project_root: str, *, min_lines: int = 5, min_group_size: int = 2, max_files: int = 1000, max_groups: int = 30, path_filter: str | None = None)` — [`L311`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L311) — Find functions with identical AST structure.
- `detect_structural_clones_cached(cache: Any, project_root: str, *, min_lines: int = 5, min_group_size: int = 2, max_groups: int = 30, path_filter: str | None = None)` — [`L503`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L503) — Find structural clones using pre-indexed AST cache (no re-parsing).
- `detect_textual_clones(project_root: str, *, min_lines: int = 5, min_group_size: int = 2, max_files: int = 1000, max_groups: int = 30, path_filter: str | None = None)` — [`L375`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L375) — Find functions with nearly identical normalized text.
- `detect_textual_clones_cached(cache: Any, project_root: str, *, min_lines: int = 5, min_group_size: int = 2, max_groups: int = 30, path_filter: str | None = None)` — [`L572`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L572) — Find textual clones using pre-indexed AST cache (no parsing at all).

## Module values
- `_EXCLUDE_DIRS` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L34)
- `_FUNC_DEF_TYPES` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L54)
- `logger` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/code_similarity.py#L32)

