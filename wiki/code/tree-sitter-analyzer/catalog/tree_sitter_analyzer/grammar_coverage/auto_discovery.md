---
title: 'Module: tree_sitter_analyzer/grammar_coverage/auto_discovery.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/grammar_coverage/auto_discovery.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.grammar_coverage.auto_discovery`/
symbols:
  AutoDiscoveryEngine: AutoDiscoveryEngine#
  AutoDiscoveryEngine._compute_corpus_coverage: AutoDiscoveryEngine#_compute_corpus_coverage().
  AutoDiscoveryEngine.detect_wrapper_nodes: AutoDiscoveryEngine#detect_wrapper_nodes().
  CoverageGapReport: CoverageGapReport#
  _collect_stats_walk: _collect_stats_walk().
  _empty_gap_report: _empty_gap_report().
  _append_language_detail: _append_language_detail().
  AutoDiscoveryEngine.analyze_coverage_gap: AutoDiscoveryEngine#analyze_coverage_gap().
  _score_wrapper_node: _score_wrapper_node().
  AutoDiscoveryEngine.generate_report: AutoDiscoveryEngine#generate_report().
  _collect_node_stats: _collect_node_stats().
  CoverageGapReport.missing_node_types: CoverageGapReport#missing_node_types.
  _no_corpus_report: _no_corpus_report().
  _append_summary_rows: _append_summary_rows().
  AutoDiscoveryEngine.analyze_all_languages: AutoDiscoveryEngine#analyze_all_languages().
  NodeStats: NodeStats#
  AutoDiscoveryEngine.enumerate_syntax_paths: AutoDiscoveryEngine#enumerate_syntax_paths().
  AutoDiscoveryEngine._load_node_types_or_empty: AutoDiscoveryEngine#_load_node_types_or_empty().
  CoverageGapReport.wrapper_candidates: CoverageGapReport#wrapper_candidates.
  CoverageGapReport.is_ok: CoverageGapReport#is_ok().
  AutoDiscoveryEngine.get_all_node_types: AutoDiscoveryEngine#get_all_node_types().
  CoverageGapReport.total_node_types: CoverageGapReport#total_node_types.
  CoverageGapReport.coverage_rate: CoverageGapReport#coverage_rate.
  AutoDiscoveryEngine.get_all_field_names: AutoDiscoveryEngine#get_all_field_names().
  CoverageGapReport.elapsed_ms: CoverageGapReport#elapsed_ms.
  _load_language_objects: _load_language_objects().
  _append_wrapper_lines: _append_wrapper_lines().
  CoverageGapReport.discovered_node_types: CoverageGapReport#discovered_node_types.
  NodeStats.node_type: NodeStats#node_type.
  NodeStats.avg_children: NodeStats#avg_children().
  _record_field_usage: _record_field_usage().
  NodeStats.field_usage: NodeStats#field_usage.
  CoverageGapReport.error: CoverageGapReport#error.
  WrapperCandidate: WrapperCandidate#
  CoverageGapReport.language: CoverageGapReport#language.
  NodeStats.samples: NodeStats#samples.
  NodeStats.child_types: NodeStats#child_types.
  WrapperCandidate.score: WrapperCandidate#score.
  AutoDiscoveryEngine.traverse: AutoDiscoveryEngine#traverse().
  NodeStats.total_children: NodeStats#total_children.
  WrapperCandidate.node_type: WrapperCandidate#node_type.
  WrapperCandidate.stats: WrapperCandidate#stats.
  WrapperCandidate.reasons: WrapperCandidate#reasons.
  AutoDiscoveryEngine.wrapper_threshold: AutoDiscoveryEngine#wrapper_threshold.
  NodeStats.parent_types: NodeStats#parent_types.
  _WRAPPER_FIELDS: _WRAPPER_FIELDS.
  _WRAPPER_NAME_PATTERNS: _WRAPPER_NAME_PATTERNS.
  _overall_totals_lines: _overall_totals_lines().
  _safe_field_name_for_id: _safe_field_name_for_id().
  AutoDiscoveryEngine.__init__: AutoDiscoveryEngine#__init__().
---
# Module: [`tree_sitter_analyzer/grammar_coverage/auto_discovery.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py)

## Classes
### `AutoDiscoveryEngine`
- def: [`tree_sitter_analyzer/grammar_coverage/auto_discovery.py:406`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L406)
- doc: Phase 3 Auto-Discovery Engine.
- signature: `class AutoDiscoveryEngine:`
- members:
  - `__init__(self, wrapper_threshold: float = 30)` — [`L421`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L421) — 初始化引擎.
  - `_compute_corpus_coverage(self, language: str, corpus_code: str, all_types: list[str], start: float)` — [`L602`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L602) — Parse ``corpus_code``, collect node stats, and assemble the gap report.
  - `_load_node_types_or_empty(self, language: str, start: float, empty_report: CoverageGapReport)` — [`L587`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L587) — Return grammar node types or an early ``empty_report`` on failure.
  - `analyze_all_languages(self, languages: list[str] | None = None)` — [`L638`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L638) — 对所有目标语言运行覆盖率缺口分析.
  - `analyze_coverage_gap(self, language: str, corpus_code: str | None = None)` — [`L551`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L551) — 分析 grammar 全量节点 vs corpus 中实际出现节点的覆盖差距.
  - `detect_wrapper_nodes(self, language: str, corpus_code: str)` — [`L470`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L470) — 基于结构特征检测 Wrapper 节点.
  - `enumerate_syntax_paths(self, language: str, corpus_code: str, max_depth: int = 3)` — [`L501`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L501) — BFS 遍历 AST，枚举所有唯一节点类型路径.
  - `generate_report(self, results: dict[str, CoverageGapReport])` — [`L658`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L658) — 生成 Markdown 格式的覆盖率报告.
  - `get_all_field_names(self, language: str)` — [`L444`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L444) — 通过 Language API 枚举所有字段名称.
  - `get_all_node_types(self, language: str)` — [`L429`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L429) — 通过 Language API 枚举所有 named node 类型.
  - `traverse(node: tree_sitter.Node, parent_path: tuple[str, ...])` — [`L529`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L529)
  - `wrapper_threshold` — [`L427`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L427)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_error`](../utils/logging.md#log_error), [`log_warning`](../utils/logging.md#log_warning), [`loader`](../language_loader.md#loader), [`load_language`](../language_loader.md#LanguageLoader.load_language), [`BUILTIN_CORPUS`](corpora/__init__.md#BUILTIN_CORPUS.BUILTIN_CORPUS), [`get_all_node_types`](introspector.md#get_all_node_types), [`create_parser_safely`](../language_loader.md#LanguageLoader.create_parser_safely), [`CoverageGapReport`](auto_discovery.md#CoverageGapReport), [`_append_language_detail`](auto_discovery.md#_append_language_detail), [`_empty_gap_report`](auto_discovery.md#_empty_gap_report), [`_score_wrapper_node`](auto_discovery.md#_score_wrapper_node), [`_collect_node_stats`](auto_discovery.md#_collect_node_stats), [`_append_summary_rows`](auto_discovery.md#_append_summary_rows), [`_no_corpus_report`](auto_discovery.md#_no_corpus_report), [`missing_node_types`](auto_discovery.md#CoverageGapReport.missing_node_types), [`is_ok`](auto_discovery.md#CoverageGapReport.is_ok), [`wrapper_candidates`](auto_discovery.md#CoverageGapReport.wrapper_candidates), [`coverage_rate`](auto_discovery.md#CoverageGapReport.coverage_rate), [`total_node_types`](auto_discovery.md#CoverageGapReport.total_node_types), [`elapsed_ms`](auto_discovery.md#CoverageGapReport.elapsed_ms), [`TARGET_LANGUAGES`](discovery_corpus.md#TARGET_LANGUAGES.TARGET_LANGUAGES), [`discovered_node_types`](auto_discovery.md#CoverageGapReport.discovered_node_types), [`error`](auto_discovery.md#CoverageGapReport.error), [`WrapperCandidate`](auto_discovery.md#WrapperCandidate), [`language`](auto_discovery.md#CoverageGapReport.language), [`score`](auto_discovery.md#WrapperCandidate.score), [`node_type`](auto_discovery.md#WrapperCandidate.node_type), [`stats`](auto_discovery.md#WrapperCandidate.stats), [`reasons`](auto_discovery.md#WrapperCandidate.reasons), [`_overall_totals_lines`](auto_discovery.md#_overall_totals_lines), [`_safe_field_name_for_id`](auto_discovery.md#_safe_field_name_for_id)
- used by: [`print_language_report`](../../scripts/auto_discover.md#print_language_report), [`take_snapshot`](grammar_snapshot.md#take_snapshot), [`diff_snapshot`](grammar_snapshot.md#diff_snapshot), [`main`](../../scripts/auto_discover.md#main), [`_root`](../../scripts/auto_discover.md#_root)  (29 test-only)

### `CoverageGapReport`
- def: [`tree_sitter_analyzer/grammar_coverage/auto_discovery.py:59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L59)
- doc: 单个语言的覆盖率缺口分析结果.
- signature: `class CoverageGapReport:`
- members:
  - `is_ok(self)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L72)
  - `coverage_rate` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L67)
  - `discovered_node_types` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L64)
  - `elapsed_ms` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L68)
  - `error` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L69)
  - `language` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L62)
  - `missing_node_types` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L65)
  - `total_node_types` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L63)
  - `wrapper_candidates` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L66)
- uses (calls/refs, reference-scoped): [`WrapperCandidate`](auto_discovery.md#WrapperCandidate)
- used by: [`print_language_report`](../../scripts/auto_discover.md#print_language_report), [`_compute_corpus_coverage`](auto_discovery.md#AutoDiscoveryEngine._compute_corpus_coverage), [`_append_language_detail`](auto_discovery.md#_append_language_detail), [`_empty_gap_report`](auto_discovery.md#_empty_gap_report), [`analyze_coverage_gap`](auto_discovery.md#AutoDiscoveryEngine.analyze_coverage_gap), [`main`](../../scripts/auto_discover.md#main), [`generate_report`](auto_discovery.md#AutoDiscoveryEngine.generate_report), [`_append_summary_rows`](auto_discovery.md#_append_summary_rows), [`_no_corpus_report`](auto_discovery.md#_no_corpus_report), [`analyze_all_languages`](auto_discovery.md#AutoDiscoveryEngine.analyze_all_languages), [`_load_node_types_or_empty`](auto_discovery.md#AutoDiscoveryEngine._load_node_types_or_empty)  (12 test-only)

### `NodeStats`
- def: [`tree_sitter_analyzer/grammar_coverage/auto_discovery.py:31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L31)
- doc: 单个节点类型的结构统计信息.
- signature: `class NodeStats:`
- members:
  - `avg_children(self)` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L42)
  - `child_types` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L37)
  - `field_usage` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L39)
  - `node_type` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L34)
  - `parent_types` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L38)
  - `samples` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L35)
  - `total_children` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L36)
- used by: [`_collect_stats_walk`](auto_discovery.md#_collect_stats_walk), [`_score_wrapper_node`](auto_discovery.md#_score_wrapper_node), [`_collect_node_stats`](auto_discovery.md#_collect_node_stats), [`_record_field_usage`](auto_discovery.md#_record_field_usage), [`stats`](auto_discovery.md#WrapperCandidate.stats)  (5 test-only)

### `WrapperCandidate`
- def: [`tree_sitter_analyzer/grammar_coverage/auto_discovery.py:49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L49)
- doc: Wrapper 节点候选项及其置信度评分.
- signature: `class WrapperCandidate:`
- members:
  - `node_type` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L52)
  - `reasons` — [`L54`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L54)
  - `score` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L53)
  - `stats` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L55)
- uses (calls/refs, reference-scoped): [`NodeStats`](auto_discovery.md#NodeStats)
- used by: [`print_language_report`](../../scripts/auto_discover.md#print_language_report), [`detect_wrapper_nodes`](auto_discovery.md#AutoDiscoveryEngine.detect_wrapper_nodes), [`wrapper_candidates`](auto_discovery.md#CoverageGapReport.wrapper_candidates), [`_append_wrapper_lines`](auto_discovery.md#_append_wrapper_lines)  (2 test-only)

## Functions
- `_append_language_detail(lines: list[str], lang: str, report: CoverageGapReport)` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L307) — Append the per-language ``### <lang>`` Markdown section.
- `_append_summary_rows(lines: list[str], results: dict[str, CoverageGapReport])` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L259) — Append summary-table rows to ``lines``; return ``(total_types, total_discovered)``.
- `_append_wrapper_lines(lines: list[str], wrapper_candidates: list[WrapperCandidate])` — [`L236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L236) — Append the ``**Wrapper node candidates:**`` block (top-5) to ``lines``.
- `_collect_node_stats(language: str, corpus_code: str)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L97) — 解析 corpus 代码，统计每种节点类型的结构特征.
- `_collect_stats_walk(node: Any, parent_type: str | None, stats_map: dict[str, NodeStats], lang_obj: Any)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L150) — Recursive walker — updates ``stats_map`` in place.
- `_empty_gap_report(language: str)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L205) — Build a zeroed ``CoverageGapReport`` ready for in-place edits.
- `_load_language_objects(language: str)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L135) — Return (lang_obj, parser) for ``language``, both may be ``None``.
- `_no_corpus_report(empty_report: CoverageGapReport, all_types: list[str], start: float)` — [`L223`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L223) — Populate ``empty_report`` for the "grammar loaded, corpus missing" branch.
- `_overall_totals_lines(total_discovered: int, total_types: int)` — [`L296`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L296) — Build the ``**Total**: discovered/total (X.X% overall coverage)`` line.
- `_record_field_usage(node: Any, ns: NodeStats, lang_obj: Any)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L186) — Tally tree-sitter field usage (``_WRAPPER_FIELDS``) on a single node.
- `_safe_field_name_for_id(lang_obj: Any, field_id: int)` — [`L340`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L340) — Return ``lang_obj.field_name_for_id(i)`` or None on lookup error.
- `_score_wrapper_node(node_type: str, stats: NodeStats)` — [`L354`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L354) — 计算 wrapper 节点置信度评分.

## Module values
- `_WRAPPER_FIELDS` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L79)
- `_WRAPPER_NAME_PATTERNS` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/auto_discovery.py#L88)

