---
title: 'Module: src/codegraphcontext/tools/handlers/analysis_handlers.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/handlers/analysis_handlers.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.handlers.analysis_handlers`/
symbols:
  find_dead_code: find_dead_code().
  find_most_complex_functions: find_most_complex_functions().
  analyze_code_relationships: analyze_code_relationships().
  find_code: find_code().
  calculate_cyclomatic_complexity: calculate_cyclomatic_complexity().
  find_java_spring_endpoints: find_java_spring_endpoints().
  find_java_spring_beans: find_java_spring_beans().
  find_datasource_nodes: find_datasource_nodes().
---
# Module: [`src/codegraphcontext/tools/handlers/analysis_handlers.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py)

## Functions
- `analyze_code_relationships(code_finder: CodeFinder, **args)` — [`L75`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L75) — Tool to analyze code relationships — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)
- `calculate_cyclomatic_complexity(code_finder: CodeFinder, **args)` — [`L34`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L34) — Tool to calculate cyclomatic complexity for a given function. — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)
- `find_code(code_finder: CodeFinder, **args)` — [`L123`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L123) — Tool to find relevant code snippets — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)
- `find_datasource_nodes(code_finder: CodeFinder, **args)` — [`L242`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L242) — Return Datasource nodes and their tables / key-patterns from the code graph (#843). — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)
- `find_dead_code(code_finder: CodeFinder, **args)` — [`L8`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L8) — Tool to find potentially dead code across the entire project. — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)
- `find_java_spring_beans(code_finder: CodeFinder, **args)` — [`L204`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L204) — Return Spring bean classes, optionally filtered by stereotype. — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)
- `find_java_spring_endpoints(code_finder: CodeFinder, **args)` — [`L163`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L163) — Return all Spring HTTP endpoint functions, optionally filtered by method or path. — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)
- `find_most_complex_functions(code_finder: CodeFinder, **args)` — [`L58`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/handlers/analysis_handlers.py#L58) — Tool to find the most complex functions. — documented in [codegraphcontext-tools-code_finder](../../../../../concepts/codegraphcontext-tools-code_finder.md)

