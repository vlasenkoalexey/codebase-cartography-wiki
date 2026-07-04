---
title: 'Module: tree_sitter_analyzer/test_gap_analyzer.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/test_gap_analyzer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.test_gap_analyzer`/
symbols:
  analyze_coverage_gaps: analyze_coverage_gaps().
  _get_complexity_cached: _get_complexity_cached().
  _build_test_symbols: _build_test_symbols().
  _extract_symbols_from_tree: _extract_symbols_from_tree().
  _classify_gaps: _classify_gaps().
  ProductionSymbol: ProductionSymbol#
  _priority_score: _priority_score().
  _make_reason: _make_reason().
  _scan_file: _scan_file().
  _collect_files: _collect_files().
  ProductionSymbol.name: ProductionSymbol#name.
  _build_coverage_summary: _build_coverage_summary().
  _make_suggestion: _make_suggestion().
  _enrich_gaps_with_static_graph: _enrich_gaps_with_static_graph().
  ProductionSymbol.file_path: ProductionSymbol#file_path.
  CoverageGap.symbol: CoverageGap#symbol.
  _extract_test_targets: _extract_test_targets().
  _build_file_class_map: _build_file_class_map().
  _is_covered: _is_covered().
  _enrich_blast_radius: _enrich_blast_radius().
  _enrich_who_should_test: _enrich_who_should_test().
  _symbol_covered_by_coverage: _symbol_covered_by_coverage().
  _is_test_file: _is_test_file().
  CoverageGapResult.total_production_symbols: CoverageGapResult#total_production_symbols.
  ProductionSymbol.language: ProductionSymbol#language.
  ProductionSymbol.class_name: ProductionSymbol#class_name.
  CoverageGap: CoverageGap#
  _risk_band: _risk_band().
  ProductionSymbol.kind: ProductionSymbol#kind.
  ProductionSymbol.complexity: ProductionSymbol#complexity.
  ProductionSymbol.risk: ProductionSymbol#risk.
  ProductionSymbol.line: ProductionSymbol#line.
  CoverageGapResult.summary: CoverageGapResult#summary.
  CoverageGapResult.gaps: CoverageGapResult#gaps.
  logger: logger.
  _extract_name: _extract_name().
  ProductionSymbol.end_line: ProductionSymbol#end_line.
  CoverageGapResult.gap_count: CoverageGapResult#gap_count.
  CoverageGapResult.covered: CoverageGapResult#covered.
  _strip_prefix: _strip_prefix().
  CoverageGap.priority: CoverageGap#priority.
  CoverageGapResult: CoverageGapResult#
  CoverageGapResult.coverage_pct: CoverageGapResult#coverage_pct.
  _load_coverage_json: _load_coverage_json().
  _NON_PROD_DIRS: _NON_PROD_DIRS.
  TestSymbol: TestSymbol#
  CoverageGap.reason: CoverageGap#reason.
  CoverageGap.suggestion: CoverageGap#suggestion.
  TestSymbol.likely_targets: TestSymbol#likely_targets.
  CoverageGap.blast_radius: CoverageGap#blast_radius.
  _FUNCTION_NODE_TYPES._FUNCTION_NODE_TYPES: _FUNCTION_NODE_TYPES._FUNCTION_NODE_TYPES.
  _EXCLUDE_DIRS: _EXCLUDE_DIRS.
  _SOURCE_EXTENSIONS: _SOURCE_EXTENSIONS.
  _TEST_FILE_PATTERNS: _TEST_FILE_PATTERNS.
  _NAME_CHILD_TYPES: _NAME_CHILD_TYPES.
  TestSymbol.name: TestSymbol#name.
  TestSymbol.file_path: TestSymbol#file_path.
  TestSymbol.language: TestSymbol#language.
  TestSymbol.line: TestSymbol#line.
  CoverageGap.who_should_test: CoverageGap#who_should_test.
  CoverageGapResult.total_test_symbols: CoverageGapResult#total_test_symbols.
  CoverageGapResult.covered_count: CoverageGapResult#covered_count.
  CoverageGapResult.source: CoverageGapResult#source.
  _TEST_PREFIXES: _TEST_PREFIXES.
  _KW_SEPARATORS: _KW_SEPARATORS.
  _compute_complexity: _compute_complexity().
  _classify_priority: _classify_priority().
  _discover_coverage_json: _discover_coverage_json().
  _build_executed_lines_index: _build_executed_lines_index().
  _CLASS_NODE_TYPES._CLASS_NODE_TYPES: _CLASS_NODE_TYPES._CLASS_NODE_TYPES.
---
# Module: [`tree_sitter_analyzer/test_gap_analyzer.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py)

## Classes
### `CoverageGap`
- def: [`tree_sitter_analyzer/test_gap_analyzer.py:173`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L173)
- signature: `class CoverageGap:`
- members:
  - `blast_radius` — [`L182`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L182)
  - `priority` — [`L175`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L175)
  - `reason` — [`L176`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L176)
  - `suggestion` — [`L177`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L177)
  - `symbol` — [`L174`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L174)
  - `who_should_test` — [`L179`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L179)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (9 test-only callers)

### `CoverageGapResult`
- def: [`tree_sitter_analyzer/test_gap_analyzer.py:186`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L186)
- signature: `class CoverageGapResult:`
- members:
  - `coverage_pct` — [`L191`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L191)
  - `covered` — [`L193`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L193)
  - `covered_count` — [`L189`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L189)
  - `gap_count` — [`L190`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L190)
  - `gaps` — [`L192`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L192)
  - `source` — [`L195`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L195)
  - `summary` — [`L194`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L194)
  - `total_production_symbols` — [`L187`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L187)
  - `total_test_symbols` — [`L188`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L188)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (18 test-only callers)

### `ProductionSymbol`
- def: [`tree_sitter_analyzer/test_gap_analyzer.py:151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L151)
- signature: `class ProductionSymbol:`
- members:
  - `class_name` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L158)
  - `complexity` — [`L159`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L159)
  - `end_line` — [`L157`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L157)
  - `file_path` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L154)
  - `kind` — [`L153`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L153)
  - `language` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L155)
  - `line` — [`L156`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L156)
  - `name` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L152)
  - `risk` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L160)
- used by: (20 test-only callers)

### `TestSymbol`
- def: [`tree_sitter_analyzer/test_gap_analyzer.py:164`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L164)
- signature: `class TestSymbol:`
- members:
  - `file_path` — [`L166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L166)
  - `language` — [`L167`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L167)
  - `likely_targets` — [`L169`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L169)
  - `line` — [`L168`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L168)
  - `name` — [`L165`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L165)
- used by: (1 test-only callers)

## Functions
- `_build_coverage_summary(prod_symbols: list[ProductionSymbol], gaps: list[CoverageGap], project_root: str, prod_files: list[tuple[str, str]], test_files: list[tuple[str, str]])` — [`L566`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L566) — Compute summary statistics for *CoverageGapResult*.
- `_build_executed_lines_index(coverage_data: dict[str, Any], project_root: str)` — [`L697`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L697) — Build {relative_file_path: frozenset(executed_line_numbers)} from coverage.json.
- `_build_file_class_map(prod_symbols: list[ProductionSymbol], project_root: str)` — [`L471`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L471) — Build map: rel_path -> set of class names (lowercased).
- `_build_test_symbols(test_files: list[tuple[str, str]])` — [`L450`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L450) — Scan test files and return (test_symbols, covered_test_names).
- `_classify_gaps(prod_symbols: list[ProductionSymbol], covered_test_names: set[str], file_class_map: dict[str, set[str]], project_root: str)` — [`L541`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L541) — Partition *prod_symbols* into gaps and covered lists.
- `_classify_priority(score: int)` — [`L530`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L530) — Map a numeric priority score to a band label.
- `_collect_files(project_root: str, language_filter: str | None = None, max_files: int = 1000, target_file: str | None = None)` — [`L268`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L268) — Collect source files under *project_root*.
- `_compute_complexity(node: Any, language: str)` — [`L387`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L387)
- `_discover_coverage_json(project_root: str)` — [`L691`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L691) — Auto-discover coverage.json at the project root. Returns path or None.
- `_enrich_blast_radius(gaps: list[CoverageGap], cache: Any)` — [`L633`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L633) — Populate blast_radius from the AST cache's call edges.
- `_enrich_gaps_with_static_graph(gaps: list[CoverageGap], project_root: str, test_files: list[tuple[str, str]])` — [`L606`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L606) — RFC-0003 criterion 6: attach static-graph context to each gap.
- `_enrich_who_should_test(gaps: list[CoverageGap], test_files: list[tuple[str, str]], project_root: str)` — [`L652`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L652) — Suggest test files that are likely responsible for testing each gap.
- `_extract_name(node: Any)` — [`L202`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L202)
- `_extract_symbols_from_tree(tree: Any, language: str, file_path: str)` — [`L210`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L210)
- `_extract_test_targets(test_name: str)` — [`L359`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L359)
- `_get_complexity_cached(sym: ProductionSymbol, parser_cache: dict[str, Any])` — [`L502`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L502) — Return cyclomatic complexity of *sym*, using *parser_cache* to avoid re-parsing.
- `_is_covered(sym: ProductionSymbol, covered_test_names: set[str], file_class_map: dict[str, set[str]], project_root: str)` — [`L484`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L484) — Return True if *sym* has matching test coverage.
- `_is_test_file(file_path: str)` — [`L198`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L198)
- `_load_coverage_json(path: str)` — [`L677`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L677) — Load and parse a coverage.py JSON report. Returns None on failure.
- `_make_reason(sym: ProductionSymbol)` — [`L868`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L868)
- `_make_suggestion(sym: ProductionSymbol)` — [`L884`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L884)
- `_priority_score(symbol: ProductionSymbol)` — [`L433`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L433)
- `_risk_band(complexity: int)` — [`L423`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L423)
- `_scan_file(file_path: str, language: str)` — [`L260`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L260)
- `_strip_prefix(name: str)` — [`L350`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L350) — Remove a test prefix from *name*; return stripped remainder, or None if no match.
- `_symbol_covered_by_coverage(sym: ProductionSymbol, executed_index: dict[str, frozenset[int]], project_root: str)` — [`L724`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L724) — True when at least one **body** line of the symbol is in executed_lines.
- `analyze_coverage_gaps(project_root: str, *, coverage_json: str | None = None, language_filter: str | None = None, max_files: int = 1000, max_gaps: int = 50, include_covered: bool = False, target_file: str | None = None)` — [`L750`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L750) — Analyse test coverage gaps. — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)

## Module values
- `_CLASS_NODE_TYPES` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L125)
- `_EXCLUDE_DIRS` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L30)
- `_FUNCTION_NODE_TYPES` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L104)
- `_KW_SEPARATORS` — [`L338`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L338)
- `_NAME_CHILD_TYPES` — [`L140`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L140)
- `_NON_PROD_DIRS` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L62)
- `_SOURCE_EXTENSIONS` — [`L82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L82)
- `_TEST_FILE_PATTERNS` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L99)
- `_TEST_PREFIXES` — [`L337`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L337)
- `logger` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/test_gap_analyzer.py#L28)

