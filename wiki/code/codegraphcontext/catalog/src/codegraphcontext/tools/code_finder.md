---
title: 'Module: src/codegraphcontext/tools/code_finder.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/code_finder.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.code_finder`/
symbols:
  CodeFinder.driver: CodeFinder#driver.
  CodeFinder.analyze_code_relationships: CodeFinder#analyze_code_relationships().
  CodeFinder: CodeFinder#
  CodeFinder.find_related_code: CodeFinder#find_related_code().
  CodeFinder.find_by_function_name: CodeFinder#find_by_function_name().
  CodeFinder.find_by_class_name: CodeFinder#find_by_class_name().
  CodeFinder._find_by_name_fuzzy_portable: CodeFinder#_find_by_name_fuzzy_portable().
  CodeFinder.find_by_content: CodeFinder#find_by_content().
  CodeFinder._lacks_native_fulltext: CodeFinder#_lacks_native_fulltext.
  CodeFinder.find_dead_code: CodeFinder#find_dead_code().
  CodeFinder.find_most_complex_functions: CodeFinder#find_most_complex_functions().
  CodeFinder._find_by_content_falkordb: CodeFinder#_find_by_content_falkordb().
  CodeFinder.find_all_callers: CodeFinder#find_all_callers().
  CodeFinder.find_all_callees: CodeFinder#find_all_callees().
  CodeFinder.find_module_dependencies: CodeFinder#find_module_dependencies().
  CodeFinder.list_indexed_repositories: CodeFinder#list_indexed_repositories().
  _levenshtein_distance: _levenshtein_distance().
  CodeFinder.audit_kotlin_call_ambiguity: CodeFinder#audit_kotlin_call_ambiguity().
  _sanitize_depth: _sanitize_depth().
  CodeFinder.format_query: CodeFinder#format_query().
  CodeFinder.db_manager: CodeFinder#db_manager.
  CodeFinder.find_by_variable_name: CodeFinder#find_by_variable_name().
  CodeFinder.find_functions_by_argument: CodeFinder#find_functions_by_argument().
  CodeFinder.find_functions_by_decorator: CodeFinder#find_functions_by_decorator().
  CodeFinder.who_calls_function: CodeFinder#who_calls_function().
  CodeFinder.what_does_function_call: CodeFinder#what_does_function_call().
  CodeFinder.who_imports_module: CodeFinder#who_imports_module().
  CodeFinder.who_modifies_variable: CodeFinder#who_modifies_variable().
  CodeFinder.find_class_hierarchy: CodeFinder#find_class_hierarchy().
  CodeFinder.find_function_overrides: CodeFinder#find_function_overrides().
  CodeFinder.find_function_call_chain: CodeFinder#find_function_call_chain().
  CodeFinder.find_variable_usage_scope: CodeFinder#find_variable_usage_scope().
  CodeFinder.get_cyclomatic_complexity: CodeFinder#get_cyclomatic_complexity().
  CodeFinder.__init__: CodeFinder#__init__().
  CodeFinder.find_by_module_name: CodeFinder#find_by_module_name().
  CodeFinder.find_imports: CodeFinder#find_imports().
  CodeFinder.find_by_type: CodeFinder#find_by_type().
  CodeFinder.find_most_complex_functions_in_file: CodeFinder#find_most_complex_functions_in_file().
  logger: logger.
  _normalize_identifier: _normalize_identifier().
  _MAX_TRAVERSAL_DEPTH: _MAX_TRAVERSAL_DEPTH.
  summarize_kotlin_call_ambiguity: summarize_kotlin_call_ambiguity().
---
# Module: [`src/codegraphcontext/tools/code_finder.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py)

## Classes
### `CodeFinder`
- def: [`src/codegraphcontext/tools/code_finder.py:144`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L144) — documented in [codegraphcontext-cli-cli_helpers](../../../../concepts/codegraphcontext-cli-cli_helpers.md)
- doc: Module for finding relevant code snippets and analyzing relationships.
- signature: `class CodeFinder:`
- members:
  - `_find_by_content_falkordb(self, search_term: str, repo_path: Optional[str] = None)` — [`L367`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L367) — FalkorDB-compatible content search using pure Cypher CONTAINS matching. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `_find_by_name_fuzzy_portable(self, label: Literal["Function", "Class"], search_term: str, edit_distance: int, repo_path: Optional[str])` — [`L206`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L206) — Fuzzy name match for backends without Lucene fuzzy syntax (Kùzu, FalkorDB, …). — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `analyze_code_relationships(self, query_type: str, target: str, context: Optional[str] = None, repo_path: Optional[str] = None, depth: Optional[int] = None)` — [`L1200`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1200) — Main method to analyze different types of code relationships with fixed return types — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
  - `audit_kotlin_call_ambiguity(self, repo_path: Optional[str] = None, limit: int = 20)` — [`L152`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L152) — Audit Kotlin function-to-function CALLS edges for multi-target callsites. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_all_callees(self, function_name: str, path: Optional[str] = None, repo_path: Optional[str] = None, depth: int = 3)` — [`L890`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L890) — Find all direct and indirect callees of a specific function, returning edges. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_all_callers(self, function_name: str, path: Optional[str] = None, repo_path: Optional[str] = None, depth: int = 3)` — [`L848`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L848) — Find all direct and indirect callers of a specific function, returning edges. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_by_class_name(self, search_term: str, fuzzy_search: bool, repo_path: Optional[str] = None, edit_distance: int = 2)` — [`L296`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L296) — Find classes by name matching. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_by_content(self, search_term: str, repo_path: Optional[str] = None)` — [`L343`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L343) — Find code by content matching in source or docstrings using the full-text index. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_by_function_name(self, search_term: str, fuzzy_search: bool, repo_path: Optional[str] = None, edit_distance: int = 2)` — [`L263`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L263) — Find functions by name matching. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_by_module_name(self, search_term: str)` — [`L395`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L395) — Find modules by name matching
  - `find_by_type(self, element_type: str, limit: int = 50)` — [`L1020`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1020) — Find all elements of a specific type (Function, Class, File, Module).
  - `find_by_variable_name(self, search_term: str, repo_path: Optional[str] = None)` — [`L329`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L329) — Find variables by name matching — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_class_hierarchy(self, class_name: str, path: Optional[str] = None, repo_path: Optional[str] = None)` — [`L705`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L705) — Find class inheritance relationships using INHERITS relationships — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_dead_code(self, exclude_decorated_with: Optional[List[str]] = None, repo_path: Optional[str] = None)` — [`L791`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L791) — Find potentially unused functions (not called by other functions in the project), optionally excluding those with specific decorators. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_function_call_chain(self, start_function: str, end_function: str, max_depth: int = 5, start_file: Optional[str] = None, end_file: Optional[str] = None, repo_path: Optional[str] = None)` — [`L927`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L927) — Find call chains between two functions — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_function_overrides(self, function_name: str, repo_path: Optional[str] = None)` — [`L768`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L768) — Find all implementations of a function across different classes — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_functions_by_argument(self, argument_name: str, path: Optional[str] = None, repo_path: Optional[str] = None)` — [`L487`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L487) — Find functions that take a specific argument name. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_functions_by_decorator(self, decorator_name: str, path: Optional[str] = None, repo_path: Optional[str] = None)` — [`L513`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L513) — Find functions that have a specific decorator applied to them. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_imports(self, search_term: str)` — [`L407`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L407) — Find imported symbols (aliases or original names).
  - `find_module_dependencies(self, module_name: str, repo_path: Optional[str] = None)` — [`L1064`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1064) — Find all dependencies and dependents of a module — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_most_complex_functions(self, limit: int = 10, repo_path: Optional[str] = None)` — [`L1367`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1367) — Find the most complex functions based on cyclomatic complexity. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_most_complex_functions_in_file(self, file_path: str, limit: int = 20, repo_path: Optional[str] = None)` — [`L1382`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1382) — Find the most complex functions in a specific file.
  - `find_related_code(self, user_query: str, fuzzy_search: bool, edit_distance: int, repo_path: Optional[str] = None)` — [`L424`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L424) — Find code related to a query using multiple search strategies — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `find_variable_usage_scope(self, variable_name: str, path: Optional[str] = None, repo_path: Optional[str] = None)` — [`L1137`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1137) — Find the scope and usage patterns of a variable, optional file path filtering — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `format_query(self, find_by: Literal["Class", "Function"], fuzzy_search: bool, repo_path: Optional[str] = None)` — [`L181`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L181) — Format the search query based on the search type and fuzzy search settings. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `get_cyclomatic_complexity(self, function_name: str, path: Optional[str] = None, repo_path: Optional[str] = None)` — [`L1340`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1340) — Get the cyclomatic complexity of a function. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `list_indexed_repositories(self)` — [`L1399`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L1399) — List all indexed repositories. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `what_does_function_call(self, function_name: str, path: Optional[str] = None, repo_path: Optional[str] = None)` — [`L604`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L604) — Find what functions a specific function calls using CALLS relationships — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `who_calls_function(self, function_name: str, path: Optional[str] = None, repo_path: Optional[str] = None)` — [`L539`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L539) — Find what functions call a specific function using CALLS relationships with improved matching — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `who_imports_module(self, module_name: str, repo_path: Optional[str] = None)` — [`L647`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L647) — Find what files import a specific module using IMPORTS relationships — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `who_modifies_variable(self, variable_name: str, repo_path: Optional[str] = None)` — [`L673`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L673) — Find what functions contain or modify a specific variable — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `db_manager` — [`L148`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L148) — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
  - `driver` — [`L149`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L149) — documented in [codegraphcontext-server](../../../../concepts/codegraphcontext-server.md)
- protocol/private: `__init__`[`L147`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L147), `_lacks_native_fulltext`[`L150`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L150)
- uses (calls/refs, reference-scoped): [`get_driver`](../core/database.md#DatabaseManager.get_driver), [`DatabaseManager`](../core/database.md#DatabaseManager), [`cypher_path_not_under_ignore_dirs`](../utils/path_ignore.md#cypher_path_not_under_ignore_dirs), [`_levenshtein_distance`](code_finder.md#_levenshtein_distance), [`_sanitize_depth`](code_finder.md#_sanitize_depth), [`_normalize_identifier`](code_finder.md#_normalize_identifier), [`logger`](code_finder.md#logger), [`summarize_kotlin_call_ambiguity`](code_finder.md#summarize_kotlin_call_ambiguity)
- used by: [`_initialize_services`](../cli/cli_helpers.md#_initialize_services), [`switch_context_tool`](../server.md#MCPServer.switch_context_tool), [`load_bundle`](handlers/management_handlers.md#load_bundle), [`code_finder`](../server.md#MCPServer.code_finder), [`search_registry_bundles`](handlers/management_handlers.md#search_registry_bundles), [`analyze_code_relationships`](handlers/analysis_handlers.md#analyze_code_relationships), [`find_code`](handlers/analysis_handlers.md#find_code), [`find_dead_code`](handlers/analysis_handlers.md#find_dead_code), [`find_most_complex_functions`](handlers/analysis_handlers.md#find_most_complex_functions), [`get_repository_stats`](handlers/management_handlers.md#get_repository_stats), [`calculate_cyclomatic_complexity`](handlers/analysis_handlers.md#calculate_cyclomatic_complexity), [`find_datasource_nodes`](handlers/analysis_handlers.md#find_datasource_nodes), [`find_java_spring_beans`](handlers/analysis_handlers.md#find_java_spring_beans), [`find_java_spring_endpoints`](handlers/analysis_handlers.md#find_java_spring_endpoints), [`list_indexed_repositories`](handlers/management_handlers.md#list_indexed_repositories)

## Functions
- `_levenshtein_distance(a: str, b: str)` — [`L31`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L31) — Levenshtein distance for short identifiers (typo-tolerant name search).
- `_normalize_identifier(s: str)` — [`L46`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L46) — Lowercase and strip separator chars so camelCase / snake_case / spaces
- `_sanitize_depth(depth, default: int = 3)` — [`L18`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L18) — Coerce and clamp a traversal depth before interpolating it into Cypher. — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
- `summarize_kotlin_call_ambiguity(rows: List[Dict[str, Any]], limit: int = 20)` — [`L60`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L60) — Summarize multi-target Kotlin function CALLS edges by callsite/name group.

## Module values
- `_MAX_TRAVERSAL_DEPTH` — [`L15`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L15)
- `logger` — [`L13`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/code_finder.py#L13)

