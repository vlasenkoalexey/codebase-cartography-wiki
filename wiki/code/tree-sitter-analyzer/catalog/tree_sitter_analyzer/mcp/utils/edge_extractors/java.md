---
title: 'Module: tree_sitter_analyzer/mcp/utils/edge_extractors/java.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/utils/edge_extractors/java.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.utils.edge_extractors.java`/
symbols:
  _detect_java_root_packages: _detect_java_root_packages().
  JavaEdgeExtractor.extract: JavaEdgeExtractor#extract().
  _scan_pom_file: _scan_pom_file().
  _scan_gradle_file: _scan_gradle_file().
  _is_implements_target_keep: _is_implements_target_keep().
  _is_extends_target_keep: _is_extends_target_keep().
  _scan_extends_edges: _scan_extends_edges().
  _scan_implements_edges: _scan_implements_edges().
  JavaEdgeExtractor: JavaEdgeExtractor#
  _build_import_map: _build_import_map().
  _root_cache._root_cache: _root_cache._root_cache.
  JavaEdgeExtractor.detect_root_packages: JavaEdgeExtractor#detect_root_packages().
  _read_group_id: _read_group_id().
  _any_prefix_match: _any_prefix_match().
  _JAVA_LANG_CLASSES._JAVA_LANG_CLASSES: _JAVA_LANG_CLASSES._JAVA_LANG_CLASSES.
  _POM_GROUP_PATTERN._POM_GROUP_PATTERN: _POM_GROUP_PATTERN._POM_GROUP_PATTERN.
  _GRADLE_GROUP_PATTERN._GRADLE_GROUP_PATTERN: _GRADLE_GROUP_PATTERN._GRADLE_GROUP_PATTERN.
  _EXTENDS_RE._EXTENDS_RE: _EXTENDS_RE._EXTENDS_RE.
  _IMPLEMENTS_RE._IMPLEMENTS_RE: _IMPLEMENTS_RE._IMPLEMENTS_RE.
  _IMPORT_RE._IMPORT_RE: _IMPORT_RE._IMPORT_RE.
---
# Module: [`tree_sitter_analyzer/mcp/utils/edge_extractors/java.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py)

## Classes
### `JavaEdgeExtractor`  ·  implements/extends EdgeExtractor
- def: [`tree_sitter_analyzer/mcp/utils/edge_extractors/java.py:224`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L224)
- doc: Java: only extends/implements edges. Import map used for package resolution.
- signature: `class JavaEdgeExtractor(EdgeExtractor):`
- members:
  - `detect_root_packages(self, project_root: str)` — [`L239`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L239)
  - `extract(self, source: str, src_name: str, project_root: str)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L227)
- uses (calls/refs, reference-scoped): [`_detect_java_root_packages`](java.md#_detect_java_root_packages), [`EdgeExtractor`](base.md#EdgeExtractor), [`_scan_extends_edges`](java.md#_scan_extends_edges), [`_scan_implements_edges`](java.md#_scan_implements_edges), [`_build_import_map`](java.md#_build_import_map)
- used by: [`EdgeExtractor`](base.md#EdgeExtractor), [`REGISTRY`](__init__.md#REGISTRY.REGISTRY), [`extract`](base.md#EdgeExtractor.extract), [`detect_root_packages`](base.md#EdgeExtractor.detect_root_packages)

## Functions
- `_any_prefix_match(pkg: str, root_packages: frozenset[str])` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L79) — Return True if pkg starts with any root package prefix.
- `_build_import_map(source: str)` — [`L177`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L177) — Build class-name → package map from Java import statements.
- `_detect_java_root_packages(project_root: str)` — [`L106`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L106) — Read project root packages from pom.xml/build.gradle.
- `_is_extends_target_keep(cls: str, import_map: dict[str, str], root_packages: frozenset[str])` — [`L153`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L153) — Decide whether ``cls`` should appear as an ``extends`` edge target.
- `_is_implements_target_keep(cls: str, import_map: dict[str, str], root_packages: frozenset[str])` — [`L122`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L122) — Decide whether ``cls`` should appear as an ``implements`` edge target.
- `_read_group_id(pattern: re.Pattern[str], text: str)` — [`L70`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L70) — Extract a groupId/group value from text; return stripped value or None.
- `_scan_extends_edges(source: str, src_name: str, import_map: dict[str, str], root_packages: frozenset[str])` — [`L187`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L187) — Return (src_name, cls) pairs for every ``extends`` relationship in source.
- `_scan_gradle_file(gradle: Path, roots: set[str])` — [`L95`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L95) — Extract group from a build.gradle / build.gradle.kts file and add to roots.
- `_scan_implements_edges(source: str, src_name: str, import_map: dict[str, str], root_packages: frozenset[str])` — [`L203`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L203) — Return (src_name, cls) pairs for every ``implements`` relationship in source.
- `_scan_pom_file(pom: Path, roots: set[str])` — [`L84`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L84) — Extract groupId from a pom.xml file and add to roots.

## Module values
- `_EXTENDS_RE` — [`L65`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L65)
- `_GRADLE_GROUP_PATTERN` — [`L64`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L64)
- `_IMPLEMENTS_RE` — [`L66`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L66)
- `_IMPORT_RE` — [`L67`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L67)
- `_JAVA_LANG_CLASSES` — [`L11`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L11)
- `_POM_GROUP_PATTERN` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L63)
- `_root_cache` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/utils/edge_extractors/java.py#L60)

