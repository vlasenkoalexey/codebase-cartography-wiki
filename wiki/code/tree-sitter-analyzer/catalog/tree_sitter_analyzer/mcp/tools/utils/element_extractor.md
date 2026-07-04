---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/element_extractor.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/element_extractor.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.element_extractor`/
symbols:
  extract_elements: extract_elements().
  get_all_exports: get_all_exports().
  get_functions: get_functions().
  get_classes: get_classes().
  get_structure: get_structure().
  _split_top_level_commas: _split_top_level_commas().
  get_functions_in_class: get_functions_in_class().
  get_imports: get_imports().
  _enum_members_from_raw_text: _enum_members_from_raw_text().
  _extract_all_reexports: _extract_all_reexports().
  _read_all_assignment: _read_all_assignment().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/element_extractor.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py)

## Functions
- `_enum_members_from_raw_text(raw_text: str)` — [`L232`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L232)
- `_extract_all_reexports(file_path: str)` — [`L246`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L246) — Parse a module-level ``__all__`` list literal and return reexports.
- `_read_all_assignment(node: ast.stmt)` — [`L273`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L273) — Return ``(names, lineno)`` if ``node`` is ``__all__ = [...]``.
- `_split_top_level_commas(body: str)` — [`L190`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L190) — Split ``body`` on commas that are NOT inside quotes or brackets.
- `extract_elements(file_path: str, project_root: str | None = None)` — [`L28`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L28) — Analyze a file with tree-sitter and return structured elements. — documented in [tree_sitter_analyzer-core-request](../../../../../concepts/tree_sitter_analyzer-core-request.md)
- `get_all_exports(result: AnalysisResult)` — [`L123`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L123) — Extract all exported symbols (classes, functions, constants, __all__). — documented in [tree_sitter_analyzer-models-result](../../../../../concepts/tree_sitter_analyzer-models-result.md)
- `get_classes(result: AnalysisResult)` — [`L77`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L77) — Extract class elements from an AnalysisResult.
- `get_functions(result: AnalysisResult)` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L58) — Extract function/method elements from an AnalysisResult. — documented in [tree_sitter_analyzer-models-result](../../../../../concepts/tree_sitter_analyzer-models-result.md)
- `get_functions_in_class(result: AnalysisResult, class_name: str)` — [`L320`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L320) — Get functions that belong to a specific class.
- `get_imports(result: AnalysisResult)` — [`L114`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L114) — Extract import/module names from an AnalysisResult.
- `get_structure(result: AnalysisResult)` — [`L296`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/element_extractor.py#L296) — Extract a lightweight structure outline.

