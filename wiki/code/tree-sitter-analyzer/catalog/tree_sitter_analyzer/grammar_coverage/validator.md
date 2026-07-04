---
title: 'Module: tree_sitter_analyzer/grammar_coverage/validator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/grammar_coverage/validator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.grammar_coverage.validator`/
symbols:
  _get_covered_node_types_from_plugin: _get_covered_node_types_from_plugin().
  validate_plugin_coverage: validate_plugin_coverage().
  CoverageReport.uncovered_types: CoverageReport#uncovered_types.
  generate_coverage_report: generate_coverage_report().
  CoverageReport.coverage_percentage: CoverageReport#coverage_percentage.
  check_coverage_threshold: check_coverage_threshold().
  validate_plugin_coverage_sync: validate_plugin_coverage_sync().
  CoverageReport.total_node_types: CoverageReport#total_node_types.
  CoverageReport.covered_node_types: CoverageReport#covered_node_types.
  CoverageReport: CoverageReport#
  CoverageReport.language: CoverageReport#language.
  _count_node_types: _count_node_types().
  _parse_corpus_file: _parse_corpus_file().
  CoverageReport.corpus_file: CoverageReport#corpus_file.
  _get_language_extension: _get_language_extension().
  CoverageReport.expected_node_types: CoverageReport#expected_node_types.
  CoverageReport.actual_node_types: CoverageReport#actual_node_types.
  _load_expected_json: _load_expected_json().
  _build_ast_line_index: _build_ast_line_index().
  _match_elements_to_paths: _match_elements_to_paths().
  _walk_ast_into_index: _walk_ast_into_index().
  _LineIndex: _LineIndex.
  _ROOT_NODE_TYPES: _ROOT_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/grammar_coverage/validator.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py)

## Classes
### `CoverageReport`
- def: [`tree_sitter_analyzer/grammar_coverage/validator.py:31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L31)
- doc: Grammar coverage 报告数据结构
- signature: `class CoverageReport:`
- members:
  - `actual_node_types` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L60)
  - `corpus_file` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L58)
  - `coverage_percentage` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L56)
  - `covered_node_types` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L55)
  - `expected_node_types` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L59)
  - `language` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L53)
  - `total_node_types` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L54)
  - `uncovered_types` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L57)
- used by: [`validate_plugin_coverage`](validator.md#validate_plugin_coverage), [`generate_coverage_report`](validator.md#generate_coverage_report), [`validate_plugin_coverage_sync`](validator.md#validate_plugin_coverage_sync), [`main`](example_usage.md#main), [`main`](../../diagnose_coverage.md#main), [`main`](../../diagnose_coverage_sync.md#main)  (15 test-only)

## Functions
- `_build_ast_line_index(root: Any, max_depth: int, max_nodes: int)` — [`L238`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L238) — Recursively walk an AST, building a ``(start_line, end_line)`` → list index.
- `_count_node_types(node: Any)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L63) — 递归统计树中所有命名节点类型的数量
- `_get_covered_node_types_from_plugin(corpus_path: Path, language: str)` — [`L279`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L279) — Return the set of AST node types the plugin actually extracted. — documented in [tree_sitter_analyzer-core-request](../../../concepts/tree_sitter_analyzer-core-request.md)
- `_get_language_extension(language: str)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L81) — 获取语言对应的文件扩展名
- `_load_expected_json(expected_path: Path)` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L157) — 加载 corpus_*_expected.json 文件
- `_match_elements_to_paths(elements: Any, line_index: _LineIndex)` — [`L256`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L256) — Match plugin elements against the line index → covered (type, path) set.
- `_parse_corpus_file(corpus_path: Path, language: str)` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L123) — 使用 tree-sitter 解析 corpus 文件并统计节点类型
- `_walk_ast_into_index(node: Any, parent_path: tuple[str, ...], depth: int, max_depth: int, max_nodes: int, line_index: dict, node_count: list[int])` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L196) — Recursive walker for _build_ast_line_index — module-level to reduce nesting depth.
- `check_coverage_threshold(coverage_percentage: float, threshold: float = 100)` — [`L475`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L475) — 检查覆盖率是否达到阈值（用于 CI 集成）
- `generate_coverage_report(report: CoverageReport)` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L431) — 生成人类可读的覆盖度报告
- `validate_plugin_coverage(language: str)` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L341) — 验证指定语言插件的 grammar coverage (Phase 1: Syntactic Path Coverage)
- `validate_plugin_coverage_sync(language: str)` — [`L492`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L492) — 同步版本的 validate_plugin_coverage（用于测试）

## Module values
- `_LineIndex` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L180)
- `_ROOT_NODE_TYPES` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/validator.py#L184)

