---
title: 'Module: tests/integration/cli/test_cli_commands.py'
type: catalog
provenance: extracted
module: tests/integration/cli/test_cli_commands.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.integration.cli.test_cli_commands`/
symbols:
  cli_test_stubs: cli_test_stubs().
  test_find_content_surfaces_query_errors: test_find_content_surfaces_query_errors().
  test_all_canonical_cli_commands_run_with_kuzudb: test_all_canonical_cli_commands_run_with_kuzudb().
  test_db_flag_kuzudb_not_overwritten_by_context_database: test_db_flag_kuzudb_not_overwritten_by_context_database().
  runner: runner.
  _inventory_from_main_source: _inventory_from_main_source().
  _matrix_command_set: _matrix_command_set().
  test_db_flag_kuzudb_not_overwritten_by_context_database._fake_get_database_manager: test_db_flag_kuzudb_not_overwritten_by_context_database()._fake_get_database_manager().
  _FakeDriver.session: _FakeDriver#session().
  _FakeDBManager.get_driver: _FakeDBManager#get_driver().
  test_cli_inventory_grouped_from_source: test_cli_inventory_grouped_from_source().
  test_config_db_rejects_invalid_backend_with_clear_error: test_config_db_rejects_invalid_backend_with_clear_error().
  test_config_show_with_empty_config_does_not_crash: test_config_show_with_empty_config_does_not_crash().
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeSession.run: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeSession#run().
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeDriver.session: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeDriver#session().
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeManager.get_driver: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeManager#get_driver().
  TestNeo4jDatabaseNameCLI.test_doctor_passes_database_to_test_connection: TestNeo4jDatabaseNameCLI#test_doctor_passes_database_to_test_connection().
  test_load_credentials_utf8_decoding_robustness._Ctx.cgcignore_path: test_load_credentials_utf8_decoding_robustness()._Ctx#cgcignore_path.
  test_load_credentials_resolves_context_database: test_load_credentials_resolves_context_database().
  _FakeGraphBuilder: _FakeGraphBuilder#
  _command_name_from_decorator: _command_name_from_decorator().
  _FakeSession: _FakeSession#
  _FakeDriver: _FakeDriver#
  _FakeDBManager: _FakeDBManager#
  _FakeCodeFinder: _FakeCodeFinder#
  cli_test_stubs._FakeMCPServer: cli_test_stubs()._FakeMCPServer#
  cli_test_stubs._FakeCGCBundle: cli_test_stubs()._FakeCGCBundle#
  test_find_content_surfaces_query_errors._FakeDBManager: test_find_content_surfaces_query_errors()._FakeDBManager#
  test_find_content_surfaces_query_errors._FailingFinder: test_find_content_surfaces_query_errors()._FailingFinder#
  test_db_flag_kuzudb_not_overwritten_by_context_database._Ctx: test_db_flag_kuzudb_not_overwritten_by_context_database()._Ctx#
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeResult: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeResult#
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeSession: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeSession#
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeDriver: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeDriver#
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeManager: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeManager#
  test_load_credentials_utf8_decoding_robustness._Ctx: test_load_credentials_utf8_decoding_robustness()._Ctx#
  test_load_credentials_resolves_context_database._Ctx: test_load_credentials_resolves_context_database()._Ctx#
  _FakeSession.__enter__: _FakeSession#__enter__().
  _FakeSession.__exit__: _FakeSession#__exit__().
  _FakeSession.run: _FakeSession#run().
  _FakeDBManager.close_driver: _FakeDBManager#close_driver().
  _FakeGraphBuilder.delete_repository_from_graph: _FakeGraphBuilder#delete_repository_from_graph().
  _FakeCodeFinder.find_by_function_name: _FakeCodeFinder#find_by_function_name().
  _FakeCodeFinder.find_by_class_name: _FakeCodeFinder#find_by_class_name().
  _FakeCodeFinder.find_by_variable_name: _FakeCodeFinder#find_by_variable_name().
  _FakeCodeFinder.find_by_module_name: _FakeCodeFinder#find_by_module_name().
  _FakeCodeFinder.find_imports: _FakeCodeFinder#find_imports().
  _FakeCodeFinder.find_by_type: _FakeCodeFinder#find_by_type().
  _FakeCodeFinder.find_by_content: _FakeCodeFinder#find_by_content().
  _FakeCodeFinder.find_functions_by_decorator: _FakeCodeFinder#find_functions_by_decorator().
  _FakeCodeFinder.find_functions_by_argument: _FakeCodeFinder#find_functions_by_argument().
  _FakeCodeFinder.what_does_function_call: _FakeCodeFinder#what_does_function_call().
  _FakeCodeFinder.who_calls_function: _FakeCodeFinder#who_calls_function().
  _FakeCodeFinder.find_function_call_chain: _FakeCodeFinder#find_function_call_chain().
  _FakeCodeFinder.find_module_dependencies: _FakeCodeFinder#find_module_dependencies().
  _FakeCodeFinder.find_class_hierarchy: _FakeCodeFinder#find_class_hierarchy().
  _FakeCodeFinder.get_cyclomatic_complexity: _FakeCodeFinder#get_cyclomatic_complexity().
  _FakeCodeFinder.find_most_complex_functions: _FakeCodeFinder#find_most_complex_functions().
  _FakeCodeFinder.find_most_complex_functions_in_file: _FakeCodeFinder#find_most_complex_functions_in_file().
  _FakeCodeFinder.find_dead_code: _FakeCodeFinder#find_dead_code().
  _FakeCodeFinder.find_function_overrides: _FakeCodeFinder#find_function_overrides().
  _FakeCodeFinder.find_variable_usage_scope: _FakeCodeFinder#find_variable_usage_scope().
  _FakeCodeFinder.audit_kotlin_call_ambiguity: _FakeCodeFinder#audit_kotlin_call_ambiguity().
  _FakeCodeFinder.list_indexed_repositories: _FakeCodeFinder#list_indexed_repositories().
  kuzudb_env: kuzudb_env().
  cli_test_stubs._FakeMCPServer.__init__: cli_test_stubs()._FakeMCPServer#__init__().
  _FakeMCPServer.tools: _FakeMCPServer#tools.
  cli_test_stubs._FakeMCPServer.run: cli_test_stubs()._FakeMCPServer#run().
  cli_test_stubs._FakeMCPServer.shutdown: cli_test_stubs()._FakeMCPServer#shutdown().
  cli_test_stubs._FakeCGCBundle.__init__: cli_test_stubs()._FakeCGCBundle#__init__().
  cli_test_stubs._FakeCGCBundle.export_to_bundle: cli_test_stubs()._FakeCGCBundle#export_to_bundle().
  cli_test_stubs._FakeCGCBundle.import_from_bundle: cli_test_stubs()._FakeCGCBundle#import_from_bundle().
  test_find_content_surfaces_query_errors._FakeDBManager.close_driver: test_find_content_surfaces_query_errors()._FakeDBManager#close_driver().
  test_find_content_surfaces_query_errors._FailingFinder.find_by_content: test_find_content_surfaces_query_errors()._FailingFinder#find_by_content().
  test_db_flag_kuzudb_not_overwritten_by_context_database._Ctx.mode: test_db_flag_kuzudb_not_overwritten_by_context_database()._Ctx#mode.
  test_db_flag_kuzudb_not_overwritten_by_context_database._Ctx.context_name: test_db_flag_kuzudb_not_overwritten_by_context_database()._Ctx#context_name.
  test_db_flag_kuzudb_not_overwritten_by_context_database._Ctx.database: test_db_flag_kuzudb_not_overwritten_by_context_database()._Ctx#database.
  test_db_flag_kuzudb_not_overwritten_by_context_database._Ctx.db_path: test_db_flag_kuzudb_not_overwritten_by_context_database()._Ctx#db_path.
  test_db_flag_kuzudb_not_overwritten_by_context_database._Ctx.cgcignore_path: test_db_flag_kuzudb_not_overwritten_by_context_database()._Ctx#cgcignore_path.
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeResult.single: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeResult#single().
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeResult.__iter__: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeResult#__iter__().
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeSession.__enter__: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeSession#__enter__().
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeSession.__exit__: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeSession#__exit__().
  test_db_flag_kuzudb_not_overwritten_by_context_database._FakeManager.close_driver: test_db_flag_kuzudb_not_overwritten_by_context_database()._FakeManager#close_driver().
  TestNeo4jDatabaseNameCLI: TestNeo4jDatabaseNameCLI#
  TestNeo4jDatabaseNameCLI.test_load_credentials_displays_database_name: TestNeo4jDatabaseNameCLI#test_load_credentials_displays_database_name().
  TestNeo4jDatabaseNameCLI.test_load_credentials_no_database_name: TestNeo4jDatabaseNameCLI#test_load_credentials_no_database_name().
  test_load_credentials_displays_kuzudb_backend: test_load_credentials_displays_kuzudb_backend().
  test_load_credentials_normalizes_tilde_paths_from_mcp_json: test_load_credentials_normalizes_tilde_paths_from_mcp_json().
  test_load_credentials_utf8_decoding_robustness: test_load_credentials_utf8_decoding_robustness().
  test_load_credentials_utf8_decoding_robustness._Ctx.mode: test_load_credentials_utf8_decoding_robustness()._Ctx#mode.
  test_load_credentials_utf8_decoding_robustness._Ctx.context_name: test_load_credentials_utf8_decoding_robustness()._Ctx#context_name.
  test_load_credentials_utf8_decoding_robustness._Ctx.database: test_load_credentials_utf8_decoding_robustness()._Ctx#database.
  test_load_credentials_utf8_decoding_robustness._Ctx.db_path: test_load_credentials_utf8_decoding_robustness()._Ctx#db_path.
  test_load_credentials_resolves_context_database._Ctx.mode: test_load_credentials_resolves_context_database()._Ctx#mode.
  test_load_credentials_resolves_context_database._Ctx.context_name: test_load_credentials_resolves_context_database()._Ctx#context_name.
  test_load_credentials_resolves_context_database._Ctx.database: test_load_credentials_resolves_context_database()._Ctx#database.
  test_load_credentials_resolves_context_database._Ctx.db_path: test_load_credentials_resolves_context_database()._Ctx#db_path.
  test_load_credentials_resolves_context_database._Ctx.cgcignore_path: test_load_credentials_resolves_context_database()._Ctx#cgcignore_path.
---
# Module: [`tests/integration/cli/test_cli_commands.py`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py)

## Classes
### `TestNeo4jDatabaseNameCLI`
- def: [`tests/integration/cli/test_cli_commands.py:609`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L609)
- doc: Integration tests for NEO4J_DATABASE display in CLI commands.
- signature: `class TestNeo4jDatabaseNameCLI:`
- members:
  - `test_doctor_passes_database_to_test_connection(self, mock_test_conn, mock_config_mgr)` — [`L614`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L614) — Test that the doctor command passes NEO4J_DATABASE to test_connection.
  - `test_load_credentials_displays_database_name(self, mock_config_mgr, monkeypatch, tmp_path)` — [`L638`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L638) — Test _load_credentials prints database name when NEO4J_DATABASE is set.
  - `test_load_credentials_no_database_name(self, mock_config_mgr, monkeypatch, tmp_path)` — [`L674`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L674) — Test _load_credentials prints Neo4j without database when NEO4J_DATABASE is not set.
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `_Ctx`
- def: [`tests/integration/cli/test_cli_commands.py:821`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L821)
- signature: `class _Ctx:`
- members:
  - `cgcignore_path` — [`L559`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L559)
  - `cgcignore_path` — [`L784`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L784)
  - `cgcignore_path` — [`L826`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L826)
  - `context_name` — [`L556`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L556)
  - `context_name` — [`L781`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L781)
  - `context_name` — [`L823`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L823)
  - `database` — [`L557`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L557)
  - `database` — [`L782`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L782)
  - `database` — [`L824`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L824)
  - `db_path` — [`L558`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L558)
  - `db_path` — [`L783`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L783)
  - `db_path` — [`L825`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L825)
  - `mode` — [`L555`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L555)
  - `mode` — [`L780`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L780)
  - `mode` — [`L822`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L822)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FailingFinder`
- def: [`tests/integration/cli/test_cli_commands.py:536`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L536)
- signature: `class _FailingFinder:`
- members:
  - `find_by_content(self, _query)` — [`L537`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L537)
- used by: (1 test-only callers)

### `_FakeCGCBundle`
- def: [`tests/integration/cli/test_cli_commands.py:296`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L296)
- signature: `class _FakeCGCBundle:`
- members:
  - `export_to_bundle(self, *_args, **_kwargs)` — [`L300`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L300)
  - `import_from_bundle(self, *_args, **_kwargs)` — [`L303`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L303)
- protocol/private: `__init__`[`L297`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L297)
- used by: (1 test-only callers)

### `_FakeCodeFinder`
- def: [`tests/integration/cli/test_cli_commands.py:126`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L126)
- signature: `class _FakeCodeFinder:`
- members:
  - `audit_kotlin_call_ambiguity(self, *_args, **_kwargs)` — [`L212`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L212)
  - `find_by_class_name(self, *_args, **_kwargs)` — [`L130`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L130)
  - `find_by_content(self, *_args, **_kwargs)` — [`L145`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L145)
  - `find_by_function_name(self, *_args, **_kwargs)` — [`L127`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L127)
  - `find_by_module_name(self, *_args, **_kwargs)` — [`L136`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L136)
  - `find_by_type(self, *_args, **_kwargs)` — [`L142`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L142)
  - `find_by_variable_name(self, *_args, **_kwargs)` — [`L133`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L133)
  - `find_class_hierarchy(self, *_args, **_kwargs)` — [`L176`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L176)
  - `find_dead_code(self, *_args, **_kwargs)` — [`L192`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L192)
  - `find_function_call_chain(self, *_args, **_kwargs)` — [`L160`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L160)
  - `find_function_overrides(self, *_args, **_kwargs)` — [`L198`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L198)
  - `find_functions_by_argument(self, *_args, **_kwargs)` — [`L151`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L151)
  - `find_functions_by_decorator(self, *_args, **_kwargs)` — [`L148`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L148)
  - `find_imports(self, *_args, **_kwargs)` — [`L139`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L139)
  - `find_module_dependencies(self, *_args, **_kwargs)` — [`L170`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L170)
  - `find_most_complex_functions(self, *_args, **_kwargs)` — [`L186`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L186)
  - `find_most_complex_functions_in_file(self, *_args, **_kwargs)` — [`L189`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L189)
  - `find_variable_usage_scope(self, *_args, **_kwargs)` — [`L201`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L201)
  - `get_cyclomatic_complexity(self, *_args, **_kwargs)` — [`L183`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L183)
  - `list_indexed_repositories(self)` — [`L221`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L221)
  - `what_does_function_call(self, *_args, **_kwargs)` — [`L154`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L154)
  - `who_calls_function(self, *_args, **_kwargs)` — [`L157`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L157)
- used by: (1 test-only callers)

### `_FakeDBManager`
- def: [`tests/integration/cli/test_cli_commands.py:532`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L532)
- signature: `class _FakeDBManager:`
- members:
  - `close_driver(self)` — [`L117`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L117)
  - `close_driver(self)` — [`L533`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L533)
  - `get_driver(self)` — [`L114`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L114)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeDriver`
- def: [`tests/integration/cli/test_cli_commands.py:578`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L578)
- signature: `class _FakeDriver:`
- members:
  - `session(self)` — [`L109`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L109)
  - `session(self)` — [`L579`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L579)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (1 test-only callers)

### `_FakeGraphBuilder`
- def: [`tests/integration/cli/test_cli_commands.py:121`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L121)
- signature: `class _FakeGraphBuilder:`
- members:
  - `delete_repository_from_graph(self, _)` — [`L122`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L122)
- used by: (2 test-only callers)

### `_FakeMCPServer`
- def: [`tests/integration/cli/test_cli_commands.py:270`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L270)
- signature: `class _FakeMCPServer:`
- members:
  - `run(self)` — [`L276`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L276)
  - `shutdown(self)` — [`L279`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L279)
  - `tools` — [`L272`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L272)
- protocol/private: `__init__`[`L271`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L271)
- used by: (1 test-only callers)

### `_FakeManager`
- def: [`tests/integration/cli/test_cli_commands.py:582`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L582)
- signature: `class _FakeManager:`
- members:
  - `close_driver(self)` — [`L586`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L586)
  - `get_driver(self)` — [`L583`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L583)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

### `_FakeResult`
- def: [`tests/integration/cli/test_cli_commands.py:561`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L561)
- signature: `class _FakeResult:`
- members:
  - `single(self)` — [`L562`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L562)
- protocol/private: `__iter__`[`L565`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L565)
- used by: (1 test-only callers)

### `_FakeSession`
- def: [`tests/integration/cli/test_cli_commands.py:568`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L568)
- signature: `class _FakeSession:`
- members:
  - `run(self, query, **kwargs)` — [`L102`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L102)
  - `run(self, *_args, **_kwargs)` — [`L575`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L575)
- protocol/private: `__enter__`[`L96`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L96), `__enter__`[`L569`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L569), `__exit__`[`L99`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L99), `__exit__`[`L572`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L572)
- uses (calls/refs, reference-scoped): (1 test-only callers)
- used by: (1 test-only callers)

## Functions
- `_command_name_from_decorator(decorator: ast.Call, func_name: str)` — [`L21`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L21)
- `_fake_get_database_manager(*_args, **_kwargs)` — [`L593`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L593)
- `_inventory_from_main_source()` — [`L32`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L32)
- `_matrix_command_set(entries: list[list[str]])` — [`L370`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L370)
- `cli_test_stubs(monkeypatch, tmp_path)` — [`L236`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L236)
- `kuzudb_env()` — [`L226`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L226)
- `test_all_canonical_cli_commands_run_with_kuzudb(kuzudb_env, cli_test_stubs)` — [`L412`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L412)
- `test_cli_inventory_grouped_from_source()` — [`L381`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L381)
- `test_config_db_rejects_invalid_backend_with_clear_error(kuzudb_env)` — [`L513`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L513)
- `test_config_show_with_empty_config_does_not_crash(monkeypatch, tmp_path)` — [`L521`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L521)
- `test_db_flag_kuzudb_not_overwritten_by_context_database(monkeypatch)` — [`L553`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L553)
- `test_find_content_surfaces_query_errors(monkeypatch)` — [`L531`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L531)
- `test_load_credentials_displays_kuzudb_backend(monkeypatch, tmp_path)` — [`L709`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L709)
- `test_load_credentials_normalizes_tilde_paths_from_mcp_json(monkeypatch, tmp_path)` — [`L735`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L735)
- `test_load_credentials_resolves_context_database(monkeypatch, tmp_path)` — [`L819`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L819) — Test that _load_credentials resolves context database and sets DEFAULT_DATABASE accordingly.
- `test_load_credentials_utf8_decoding_robustness(monkeypatch, tmp_path)` — [`L777`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L777) — Test that _load_credentials successfully handles .env files with invalid UTF-8 bytes.

## Module values
- `runner` — [`L18`](../../../../../../../raw/code/codegraphcontext/tests/integration/cli/test_cli_commands.py#L18)

