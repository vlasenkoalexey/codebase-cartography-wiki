---
title: 'Module: scripts/monitor_coverage.py'
type: catalog
provenance: extracted
module: scripts/monitor_coverage.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.monitor_coverage`/
symbols:
  main: main().
  CoverageMonitor.generate_report: CoverageMonitor#generate_report().
  CoverageMonitor.get_overall_coverage: CoverageMonitor#get_overall_coverage().
  CoverageMonitor.get_coverage_data: CoverageMonitor#get_coverage_data().
  CoverageMonitor.print_summary: CoverageMonitor#print_summary().
  CoverageMonitor.get_low_coverage_files: CoverageMonitor#get_low_coverage_files().
  CoverageMonitor.trend_file: CoverageMonitor#trend_file.
  CoverageMonitor.get_trend: CoverageMonitor#get_trend().
  CoverageMonitor.run_coverage: CoverageMonitor#run_coverage().
  CoverageMonitor.save_trend: CoverageMonitor#save_trend().
  CoverageMonitor.check_threshold: CoverageMonitor#check_threshold().
  CoverageMonitor.get_module_coverage: CoverageMonitor#get_module_coverage().
  CoverageMonitor.get_uncovered_lines: CoverageMonitor#get_uncovered_lines().
  CoverageMonitor.coverage_json: CoverageMonitor#coverage_json.
  CoverageMonitor: CoverageMonitor#
  CoverageMonitor.project_root: CoverageMonitor#project_root.
  CoverageMonitor.__init__: CoverageMonitor#__init__().
  CoverageMonitor.coverage_file: CoverageMonitor#coverage_file.
---
# Module: [`scripts/monitor_coverage.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py)

## Classes
### `CoverageMonitor`
- def: [`scripts/monitor_coverage.py:16`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L16)
- doc: 覆盖率监控器。
- signature: `class CoverageMonitor:`
- members:
  - `__init__(self, project_root: Path)` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L19) — 初始化覆盖率监控器。
  - `check_threshold(self, threshold: float = 80)` — [`L275`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L275) — 检查覆盖率是否达到阈值。
  - `generate_report(self, output_file: Path | None = None)` — [`L184`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L184) — 生成覆盖率报告。
  - `get_coverage_data(self)` — [`L58`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L58) — 获取覆盖率数据。
  - `get_low_coverage_files(self, threshold: float = 80)` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L97) — 获取低覆盖率文件列表。
  - `get_module_coverage(self, module_name: str)` — [`L79`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L79) — 获取特定模块的覆盖率。
  - `get_overall_coverage(self)` — [`L70`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L70) — 获取总体覆盖率。
  - `get_trend(self)` — [`L172`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L172) — 获取覆盖率趋势数据。
  - `get_uncovered_lines(self, file_path: str)` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L127) — 获取文件的未覆盖行号。
  - `print_summary(self)` — [`L287`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L287) — 打印覆盖率摘要。
  - `run_coverage(self, target: str | None = None, verbose: bool = False)` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L30) — 运行覆盖率检查。
  - `save_trend(self, coverage: float)` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L146) — 保存覆盖率趋势数据。
  - `coverage_file` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L26)
  - `coverage_json` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L27)
  - `project_root` — [`L25`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L25)
  - `trend_file` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L28)
- used by: [`main`](monitor_coverage.md#main)

## Functions
- `main()` — [`L312`](../../../../../raw/code/tree-sitter-analyzer/scripts/monitor_coverage.py#L312) — 主函数。

