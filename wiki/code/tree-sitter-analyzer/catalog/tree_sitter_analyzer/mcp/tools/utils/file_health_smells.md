---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.file_health_smells`/
symbols:
  detect_code_smells: detect_code_smells().
  _check_element_smells: _check_element_smells().
  canonical_smell_type: canonical_smell_type().
  _check_god_class: _check_god_class().
  _check_deep_nesting: _check_deep_nesting().
  _check_technical_debt: _check_technical_debt().
  _add_low_complexity_smell: _add_low_complexity_smell().
  _has_technical_debt_marker: _has_technical_debt_marker().
  _check_dimension_smells: _check_dimension_smells().
  _check_long_functions: _check_long_functions().
  _comment_text: _comment_text().
  _check_anti_pattern_smells: _check_anti_pattern_smells().
  _check_long_lines: _check_long_lines().
  _check_oversized_file: _check_oversized_file().
  _annotate_complexity_smell: _annotate_complexity_smell().
  _add_low_structure_smell: _add_low_structure_smell().
  _add_high_coupling_smell: _add_high_coupling_smell().
  _check_heuristic_long_methods: _check_heuristic_long_methods().
  _anti_pattern_fix_hint: _anti_pattern_fix_hint().
  _check_single_line_file: _check_single_line_file().
  _check_security_smells: _check_security_smells().
  _SECURITY_SMELL_PREFIX: _SECURITY_SMELL_PREFIX.
  TECH_DEBT_MARKERS: TECH_DEBT_MARKERS.
  LONG_LINE_THRESHOLD: LONG_LINE_THRESHOLD.
  COMMENT_DELIMITERS: COMMENT_DELIMITERS.
  SINGLE_LINE_FILE_THRESHOLD: SINGLE_LINE_FILE_THRESHOLD.
  LONG_LINE_REPORT_LIMIT: LONG_LINE_REPORT_LIMIT.
  _base_complexity_smell: _base_complexity_smell().
  _ANTI_PATTERN_FIX_HINTS._ANTI_PATTERN_FIX_HINTS: _ANTI_PATTERN_FIX_HINTS._ANTI_PATTERN_FIX_HINTS.
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py)

## Functions
- `_add_high_coupling_smell(smells: list[dict[str, Any]], dimensions: dict[str, float], lines: list[str])` — [`L326`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L326) — Add a smell for very low dependency scores.
- `_add_low_complexity_smell(smells: list[dict[str, Any]], dimensions: dict[str, float], lines: list[str], analysis: Any)` — [`L284`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L284) — Add a smell for very low complexity scores.
- `_add_low_structure_smell(smells: list[dict[str, Any]], dimensions: dict[str, float], lines: list[str])` — [`L262`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L262) — Add a smell for very low structure scores.
- `_annotate_complexity_smell(smell: dict[str, Any], lines: list[str], analysis: Any)` — [`L309`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L309) — Attach the best available location evidence to a complexity smell.
- `_anti_pattern_fix_hint(anti_type: str | None)` — [`L143`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L143) — Return a one-line fix hint for an anti-pattern smell.
- `_base_complexity_smell(complexity: float)` — [`L299`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L299) — Build the generic high-complexity smell payload.
- `_check_anti_pattern_smells(smells: list[dict[str, Any]], file_path: str, language: str | None)` — [`L103`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L103) — Emit anti-pattern findings (mutable_default_argument, bare_except, …).
- `_check_deep_nesting(smells: list[dict[str, Any]], lines: list[str])` — [`L234`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L234) — Detect deep nesting based on indentation levels.
- `_check_dimension_smells(smells: list[dict[str, Any]], dimensions: dict[str, float], lines: list[str], analysis: Any)` — [`L250`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L250) — Flag low scores in structure, complexity, and dependency dimensions.
- `_check_element_smells(smells: list[dict[str, Any]], lines: list[str], line_count: int, analysis: Any)` — [`L346`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L346) — Detect god_class and long_method smells from tree-sitter elements.
- `_check_god_class(smells: list[dict[str, Any]], line_count: int, classes: list[dict[str, Any]])` — [`L370`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L370) — Flag files that look like a single oversized class/module.
- `_check_heuristic_long_methods(smells: list[dict[str, Any]], lines: list[str])` — [`L412`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L412) — Flag long methods when tree-sitter analysis is unavailable.
- `_check_long_functions(smells: list[dict[str, Any]], functions: list[dict[str, Any]])` — [`L393`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L393) — Flag tree-sitter functions longer than the recommended limit.
- `_check_long_lines(smells: list[dict[str, Any]], lines: list[str])` — [`L150`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L150) — Flag individual lines that exceed ``LONG_LINE_THRESHOLD``.
- `_check_oversized_file(smells: list[dict[str, Any]], line_count: int)` — [`L220`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L220) — Flag files exceeding recommended line count.
- `_check_security_smells(smells: list[dict[str, Any]], source: str, language: str | None, file_path: str)` — [`L475`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L475) — Add security scanner issues as file-health smells.
- `_check_single_line_file(smells: list[dict[str, Any]], source: str)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L189) — Flag files that have no newlines but substantial content.
- `_check_technical_debt(smells: list[dict[str, Any]], lines: list[str])` — [`L430`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L430) — Count TODO/FIXME/HACK markers as technical debt.
- `_comment_text(line: str)` — [`L464`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L464) — Return probable comment text while avoiding string literals.
- `_has_technical_debt_marker(line: str)` — [`L451`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L451) — Return whether a line has a TODO-like marker in comment text.
- `canonical_smell_type(smell: dict[str, Any])` — [`L30`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L30) — Return the canonical type name for a smell.
- `detect_code_smells(file_path: str, dimensions: dict[str, float], analysis: Any, language: str | None = None)` — [`L63`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L63) — Detect specific code smells using tree-sitter elements.

## Module values
- `COMMENT_DELIMITERS` — [`L46`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L46)
- `LONG_LINE_REPORT_LIMIT` — [`L60`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L60)
- `LONG_LINE_THRESHOLD` — [`L58`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L58)
- `SINGLE_LINE_FILE_THRESHOLD` — [`L59`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L59)
- `TECH_DEBT_MARKERS` — [`L45`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L45)
- `_ANTI_PATTERN_FIX_HINTS` — [`L130`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L130)
- `_SECURITY_SMELL_PREFIX` — [`L27`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/file_health_smells.py#L27)

