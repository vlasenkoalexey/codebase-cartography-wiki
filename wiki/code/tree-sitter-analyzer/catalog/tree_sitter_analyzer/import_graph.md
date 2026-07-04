---
title: 'Module: tree_sitter_analyzer/import_graph.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/import_graph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.import_graph`/
symbols:
  ImportGraph.build: ImportGraph#build().
  ImportGraph._make_result: ImportGraph#_make_result().
  ImportGraph.summary: ImportGraph#summary().
  _resolve_python_import: _resolve_python_import().
  ImportGraph.dependents_of: ImportGraph#dependents_of().
  ImportGraph.blast_radius: ImportGraph#blast_radius().
  ImportGraphResult.edges: ImportGraphResult#edges.
  ImportGraph.dependencies_of: ImportGraph#dependencies_of().
  ImportGraph: ImportGraph#
  ImportEdge.to_dict: ImportEdge#to_dict().
  ImportGraphResult.to_dict: ImportGraphResult#to_dict().
  ImportGraphResult: ImportGraphResult#
  ImportGraphResult.cycles: ImportGraphResult#cycles.
  _resolve_js_import: _resolve_js_import().
  ImportGraph._resolve_import: ImportGraph#_resolve_import().
  ImportGraph._dfs: ImportGraph#_dfs().
  ImportGraphResult.edge_count: ImportGraphResult#edge_count.
  ImportGraph._reverse: ImportGraph#_reverse.
  ImportGraph._project_files: ImportGraph#_project_files.
  ImportGraph._edges: ImportGraph#_edges.
  ImportGraph._forward: ImportGraph#_forward.
  ImportGraph._built: ImportGraph#_built.
  ImportEdge: ImportEdge#
  ImportEdge.source_file: ImportEdge#source_file.
  ImportEdge.target_file: ImportEdge#target_file.
  ImportGraphResult.file_count: ImportGraphResult#file_count.
  ImportGraph._detect_cycles: ImportGraph#_detect_cycles().
  ImportGraph.project_root: ImportGraph#project_root.
  ImportEdge.import_text: ImportEdge#import_text.
  ImportEdge.line: ImportEdge#line.
  logger: logger.
  _PY_FROM_IMPORT_RE: _PY_FROM_IMPORT_RE.
  _PY_BARE_IMPORT_RE: _PY_BARE_IMPORT_RE.
  _PY_RELATIVE_IMPORT_RE: _PY_RELATIVE_IMPORT_RE.
  _JS_REQUIRE_RE: _JS_REQUIRE_RE.
  _JS_ESM_IMPORT_RE: _JS_ESM_IMPORT_RE.
  _PY_STDLIB_PREFIXES: _PY_STDLIB_PREFIXES.
  ImportGraph.__init__: ImportGraph#__init__().
---
# Module: [`tree_sitter_analyzer/import_graph.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py)

## Classes
### `ImportEdge`
- def: [`tree_sitter_analyzer/import_graph.py:150`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L150)
- signature: `class ImportEdge:`
- members:
  - `to_dict(self)` — [`L156`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L156)
  - `import_text` — [`L153`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L153)
  - `line` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L154)
  - `source_file` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L151)
  - `target_file` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L152)
- used by: [`build`](import_graph.md#ImportGraph.build), [`component_diagram`](uml_export.md#UMLExporter.component_diagram), [`package_diagram`](uml_export.md#UMLExporter.package_diagram), [`blast_radius`](import_graph.md#ImportGraph.blast_radius), [`dependents_of`](import_graph.md#ImportGraph.dependents_of), [`dependencies_of`](import_graph.md#ImportGraph.dependencies_of), [`edges`](import_graph.md#ImportGraphResult.edges), [`to_dict`](import_graph.md#ImportGraphResult.to_dict), [`_dfs`](import_graph.md#ImportGraph._dfs), [`_reverse`](import_graph.md#ImportGraph._reverse), [`_edges`](import_graph.md#ImportGraph._edges), [`_forward`](import_graph.md#ImportGraph._forward)  (2 test-only)

### `ImportGraph`
- def: [`tree_sitter_analyzer/import_graph.py:271`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L271)
- doc: File-level import dependency graph built from cached AST data.
- signature: `class ImportGraph:`
- members:
  - `_detect_cycles(self)` — [`L415`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L415) — Detect import cycles using DFS.
  - `blast_radius(self, file_path: str, max_depth: int = 10)` — [`L377`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L377) — Compute transitive reverse deps — all files affected by changing this file.
  - `build(self)` — [`L288`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L288) — Build the import graph from AST cache data. — documented in [tree_sitter_analyzer-ast_cache](../../concepts/tree_sitter_analyzer-ast_cache.md)
  - `dependencies_of(self, file_path: str)` — [`L365`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L365) — Find all files that the given file imports (forward deps).
  - `dependents_of(self, file_path: str)` — [`L353`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L353) — Find all files that import the given file (reverse deps).
  - `summary(self)` — [`L447`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L447) — Return summary statistics.
  - `project_root` — [`L281`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L281)
- protocol/private: `__init__`[`L280`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L280), `_built`[`L286`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L286), `_dfs`[`L422`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L422), `_edges`[`L282`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L282), `_forward`[`L283`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L283), `_make_result`[`L345`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L345), `_project_files`[`L285`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L285), `_resolve_import`[`L330`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L330), `_reverse`[`L284`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L284)
- uses (calls/refs, reference-scoped): [`ASTCache`](ast_cache.md#ASTCache), [`close`](ast_cache.md#ASTCache.close), [`_resolve_python_import`](import_graph.md#_resolve_python_import), [`edges`](import_graph.md#ImportGraphResult.edges), [`to_dict`](import_graph.md#ImportEdge.to_dict), [`ImportGraphResult`](import_graph.md#ImportGraphResult), [`cycles`](import_graph.md#ImportGraphResult.cycles), [`_resolve_js_import`](import_graph.md#_resolve_js_import), [`edge_count`](import_graph.md#ImportGraphResult.edge_count), [`ImportEdge`](import_graph.md#ImportEdge), [`file_count`](import_graph.md#ImportGraphResult.file_count), [`source_file`](import_graph.md#ImportEdge.source_file), [`target_file`](import_graph.md#ImportEdge.target_file), [`get_imports`](ast_cache.md#ASTCache.get_imports), [`import_text`](import_graph.md#ImportEdge.import_text), [`line`](import_graph.md#ImportEdge.line), [`logger`](import_graph.md#logger)
- used by: [`component_diagram`](uml_export.md#UMLExporter.component_diagram), [`package_diagram`](uml_export.md#UMLExporter.package_diagram), [`execute`](mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool.execute), [`_get_graph`](mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool._get_graph), [`__init__`](mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool.__init__)  (12 test-only)

### `ImportGraphResult`
- def: [`tree_sitter_analyzer/import_graph.py:166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L166)
- signature: `class ImportGraphResult:`
- members:
  - `to_dict(self)` — [`L172`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L172)
  - `cycles` — [`L170`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L170)
  - `edge_count` — [`L169`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L169)
  - `edges` — [`L167`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L167)
  - `file_count` — [`L168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L168)
- uses (calls/refs, reference-scoped): [`to_dict`](import_graph.md#ImportEdge.to_dict), [`ImportEdge`](import_graph.md#ImportEdge)
- used by: [`build`](import_graph.md#ImportGraph.build), [`component_diagram`](uml_export.md#UMLExporter.component_diagram), [`package_diagram`](uml_export.md#UMLExporter.package_diagram), [`execute`](mcp/tools/import_graph_tool.md#CodeGraphImportGraphTool.execute), [`_make_result`](import_graph.md#ImportGraph._make_result)  (9 test-only)

## Functions
- `_resolve_js_import(import_text: str, source_file: str, project_files: set[str], project_root: str)` — [`L242`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L242) — Resolve a JS/TS require/import to a project-relative file path.
- `_resolve_python_import(import_text: str, source_file: str, project_files: set[str], project_root: str)` — [`L181`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L181) — Resolve a Python import statement to a project-relative file path.

## Module values
- `_JS_ESM_IMPORT_RE` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L33)
- `_JS_REQUIRE_RE` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L32)
- `_PY_BARE_IMPORT_RE` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L27)
- `_PY_FROM_IMPORT_RE` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L26)
- `_PY_RELATIVE_IMPORT_RE` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L28)
- `_PY_STDLIB_PREFIXES` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L35)
- `logger` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/import_graph.py#L24)

