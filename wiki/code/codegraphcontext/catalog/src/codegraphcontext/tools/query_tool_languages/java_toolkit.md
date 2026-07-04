---
title: 'Module: src/codegraphcontext/tools/query_tool_languages/java_toolkit.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/query_tool_languages/java_toolkit.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.query_tool_languages.java_toolkit`/JavaToolkit#
symbols:
  JavaToolkit._run: _run().
  JavaToolkit.find_spring_endpoints: find_spring_endpoints().
  JavaToolkit.find_beans_by_stereotype: find_beans_by_stereotype().
  JavaToolkit.find_spring_injection_targets: find_spring_injection_targets().
  JavaToolkit.find_transactional_methods: find_transactional_methods().
  JavaToolkit.find_maven_module_deps: find_maven_module_deps().
  JavaToolkit.find_ambiguous_calls: find_ambiguous_calls().
  JavaToolkit: ''
  JavaToolkit._driver: _driver.
  JavaToolkit.__init__: __init__().
  JavaToolkit._cf: _cf.
  JavaToolkit.get_cypher_query: get_cypher_query().
---
# Module: [`src/codegraphcontext/tools/query_tool_languages/java_toolkit.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py)

## Classes
### `JavaToolkit`
- def: [`src/codegraphcontext/tools/query_tool_languages/java_toolkit.py:14`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L14)
- doc: Spring-aware Java analysis methods backed by CodeFinder / raw Cypher.
- signature: `class JavaToolkit:`
- members:
  - `__init__(self, code_finder: Any)` — [`L17`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L17) — Args:
  - `find_ambiguous_calls(self, repo_path: Optional[str] = None, limit: int = 50)` — [`L216`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L216) — Return CALLS edges with AMBIGUOUS confidence — potential mis-resolutions.
  - `find_beans_by_stereotype(self, stereotype: Optional[str] = None, repo_path: Optional[str] = None)` — [`L79`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L79) — Return Spring bean classes, optionally filtered by stereotype.
  - `find_maven_module_deps(self, artifact_id: str)` — [`L184`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L184) — Return internal and external dependencies of a Maven module.
  - `find_spring_endpoints(self, http_method: Optional[str] = None, path_pattern: Optional[str] = None, repo_path: Optional[str] = None)` — [`L37`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L37) — Return Spring HTTP endpoint functions.
  - `find_spring_injection_targets(self, class_name: str, repo_path: Optional[str] = None)` — [`L120`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L120) — Return all classes that inject *class_name* via @Autowired / @Inject.
  - `find_transactional_methods(self, repo_path: Optional[str] = None)` — [`L153`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L153) — Return all @Transactional-annotated functions.
  - `get_cypher_query(self, query: str)` — [`L250`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L250)
- protocol/private: `_cf`[`L22`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L22), `_driver`[`L23`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L23), `_run`[`L27`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/query_tool_languages/java_toolkit.py#L27)
- used by: [`TOOLKITS`](../advanced_language_query_tool.md#Advanced_language_query.TOOLKITS)

