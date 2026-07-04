---
title: 'Module: src/codegraphcontext/tools/report_generator.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/report_generator.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.report_generator`/
symbols:
  generate_report: generate_report().
  _section_god_nodes: _section_god_nodes().
  _section_complexity: _section_complexity().
  _section_cross_module_calls: _section_cross_module_calls().
  _section_dead_code: _section_dead_code().
  _section_spring_endpoints: _section_spring_endpoints().
  _section_spring_beans: _section_spring_beans().
  _section_maven_modules: _section_maven_modules().
  _section_suggested_queries: _section_suggested_queries().
  _h2: _h2().
  _run_cypher: _run_cypher().
  _table: _table().
  resolve_report_repo_scope: resolve_report_repo_scope().
  _h3: _h3().
  _code_block: _code_block().
  _repo_params: _repo_params().
---
# Module: [`src/codegraphcontext/tools/report_generator.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py)

## Functions
- `_code_block(cypher: str)` — [`L106`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L106)
- `_h2(title: str)` — [`L90`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L90)
- `_h3(title: str)` — [`L94`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L94)
- `_repo_params(repo_path: Optional[str])` — [`L74`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L74)
- `_run_cypher(driver: Any, query: str, params: Optional[Dict] = None)` — [`L80`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L80) — Execute a read-only Cypher query and return a list of record dicts.
- `_section_complexity(driver: Any, limit: int = 15, repo_path: Optional[str] = None)` — [`L146`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L146) — Most complex functions by cyclomatic complexity.
- `_section_cross_module_calls(driver: Any, limit: int = 20, repo_path: Optional[str] = None)` — [`L176`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L176) — Cross-directory (cross-module) CALLS edges — potential surprising connections.
- `_section_dead_code(driver: Any, limit: int = 20, repo_path: Optional[str] = None)` — [`L221`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L221) — Functions with no incoming CALLS edges (potential dead code).
- `_section_god_nodes(driver: Any, limit: int = 15, repo_path: Optional[str] = None)` — [`L112`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L112) — Functions / classes with the highest number of incoming CALLS edges.
- `_section_maven_modules(driver: Any)` — [`L303`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L303) — Maven module dependency summary.
- `_section_spring_beans(driver: Any)` — [`L282`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L282) — Spring bean stereotype summary.
- `_section_spring_endpoints(driver: Any)` — [`L251`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L251) — Spring HTTP endpoints — table of method, path, handler function.
- `_section_suggested_queries()` — [`L329`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L329)
- `_table(headers: List[str], rows: List[List[Any]])` — [`L98`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L98) — Render a simple markdown table.
- `generate_report(db_manager: Any, output_path: Optional[Path] = None, include_java: bool = False, repo_path: Optional[str] = None, god_node_limit: int = 15, complexity_limit: int = 15, cross_module_limit: int = 20)` — [`L382`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L382) — Generate a CGC_REPORT.md and return the markdown string. — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- `resolve_report_repo_scope(db_manager: Any, cwd: Optional[Path] = None)` — [`L28`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/report_generator.py#L28) — Pick a single indexed repository to scope report queries.

