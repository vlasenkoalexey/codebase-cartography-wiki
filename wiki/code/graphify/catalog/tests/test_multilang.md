---
title: 'Module: tests/test_multilang.py'
type: catalog
provenance: extracted
module: tests/test_multilang.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_multilang`/
symbols:
  FIXTURES: FIXTURES.
  _edge_labels: _edge_labels().
  _extract_sql_or_skip: _extract_sql_or_skip().
  _labels: _labels().
  test_ts_finds_class: test_ts_finds_class().
  test_ts_finds_methods: test_ts_finds_methods().
  test_ts_finds_function: test_ts_finds_function().
  test_ts_emits_calls: test_ts_emits_calls().
  test_ts_import_edges_have_import_context: test_ts_import_edges_have_import_context().
  test_ts_call_edges_have_call_context: test_ts_call_edges_have_call_context().
  test_go_finds_struct: test_go_finds_struct().
  test_go_finds_methods: test_go_finds_methods().
  test_go_finds_constructor: test_go_finds_constructor().
  test_go_emits_calls: test_go_emits_calls().
  test_go_has_extracted_calls: test_go_has_extracted_calls().
  test_go_import_edges_have_import_context: test_go_import_edges_have_import_context().
  test_go_call_edges_have_call_context: test_go_call_edges_have_call_context().
  test_go_embeds_struct_field: test_go_embeds_struct_field().
  test_go_interface_embedding_emits_embeds: test_go_interface_embedding_emits_embeds().
  test_go_struct_named_field_emits_field_context: test_go_struct_named_field_emits_field_context().
  test_go_method_parameter_return_contexts: test_go_method_parameter_return_contexts().
  test_go_method_declaration_emits_refs_only_when_name_present: test_go_method_declaration_emits_refs_only_when_name_present().
  test_rust_finds_struct: test_rust_finds_struct().
  test_rust_finds_impl_methods: test_rust_finds_impl_methods().
  test_rust_finds_function: test_rust_finds_function().
  test_rust_emits_calls: test_rust_emits_calls().
  test_rust_import_edges_have_import_context: test_rust_import_edges_have_import_context().
  test_rust_call_edges_have_call_context: test_rust_call_edges_have_call_context().
  test_rust_trait_impl_emits_implements: test_rust_trait_impl_emits_implements().
  test_rust_supertrait_emits_inherits: test_rust_supertrait_emits_inherits().
  test_rust_enum_variant_references: test_rust_enum_variant_references().
  test_rust_struct_field_emits_field_context: test_rust_struct_field_emits_field_context().
  test_rust_tuple_struct_field_references: test_rust_tuple_struct_field_references().
  test_rust_method_parameter_return_and_generic_contexts: test_rust_method_parameter_return_and_generic_contexts().
  _edges_with_relation: _edges_with_relation().
  test_go_method_declaration_emits_refs_only_when_name_present._guarded_by_name_node._is_guarded: test_go_method_declaration_emits_refs_only_when_name_present()._guarded_by_name_node()._is_guarded().
  test_go_method_declaration_emits_refs_only_when_name_present._guarded_by_name_node: test_go_method_declaration_emits_refs_only_when_name_present()._guarded_by_name_node().
  test_ts_calls_are_extracted: test_ts_calls_are_extracted().
  test_ts_no_dangling_edges: test_ts_no_dangling_edges().
  test_go_no_dangling_edges: test_go_no_dangling_edges().
  test_rust_calls_are_extracted: test_rust_calls_are_extracted().
  test_rust_no_dangling_edges: test_rust_no_dangling_edges().
  test_rust_no_cross_crate_spurious_edges: test_rust_no_cross_crate_spurious_edges().
  test_extract_dispatches_all_languages: test_extract_dispatches_all_languages().
  test_cache_hit_returns_same_result: test_cache_hit_returns_same_result().
  _call_pairs: _call_pairs().
  test_go_method_declaration_emits_refs_only_when_name_present._find_branch: test_go_method_declaration_emits_refs_only_when_name_present()._find_branch().
  test_cache_miss_after_file_change: test_cache_miss_after_file_change().
  test_sql_finds_tables: test_sql_finds_tables().
  test_sql_finds_view: test_sql_finds_view().
  test_sql_finds_function: test_sql_finds_function().
  test_sql_emits_foreign_key_edge: test_sql_emits_foreign_key_edge().
  test_sql_emits_reads_from_edge: test_sql_emits_reads_from_edge().
  test_sql_no_dangling_edges: test_sql_no_dangling_edges().
  test_sql_alter_table_fk_edge: test_sql_alter_table_fk_edge().
  test_sql_schema_qualified_names: test_sql_schema_qualified_names().
  test_sql_schema_qualified_alter_fk: test_sql_schema_qualified_alter_fk().
  _confidences: _confidences().
  _normalize_symbol_label: _normalize_symbol_label().
  test_go_method_declaration_emits_refs_only_when_name_present._is_early_return_on_falsy_name_node: test_go_method_declaration_emits_refs_only_when_name_present()._is_early_return_on_falsy_name_node().
  test_go_method_declaration_emits_refs_only_when_name_present._guarded_by_name_node._stmt_chain: test_go_method_declaration_emits_refs_only_when_name_present()._guarded_by_name_node()._stmt_chain().
---
# Module: [`tests/test_multilang.py`](../../../../../raw/code/graphify/tests/test_multilang.py)

## Functions
- `_call_pairs(result)` — [`L16`](../../../../../raw/code/graphify/tests/test_multilang.py#L16)
- `_confidences(result)` — [`L23`](../../../../../raw/code/graphify/tests/test_multilang.py#L23)
- `_edge_labels(result, relation, context=None)` — [`L35`](../../../../../raw/code/graphify/tests/test_multilang.py#L35)
- `_edges_with_relation(result, *relations)` — [`L27`](../../../../../raw/code/graphify/tests/test_multilang.py#L27)
- `_extract_sql_or_skip(fixture: str = "sample.sql")` — [`L453`](../../../../../raw/code/graphify/tests/test_multilang.py#L453)
- `_find_branch(root: ast.AST, type_literal: str)` — [`L181`](../../../../../raw/code/graphify/tests/test_multilang.py#L181) — Return the `if t == '<type_literal>':` branch inside the walk function.
- `_guarded_by_name_node(branch: ast.If, var_name: str)` — [`L215`](../../../../../raw/code/graphify/tests/test_multilang.py#L215) — True iff every read of `var_name` in `branch` is guarded by a
- `_is_early_return_on_falsy_name_node(stmt: ast.AST)` — [`L199`](../../../../../raw/code/graphify/tests/test_multilang.py#L199) — True iff `stmt` is `if not name_node: return` (or raise/continue/break).
- `_is_guarded(use: ast.AST)` — [`L241`](../../../../../raw/code/graphify/tests/test_multilang.py#L241)
- `_labels(result)` — [`L13`](../../../../../raw/code/graphify/tests/test_multilang.py#L13)
- `_normalize_symbol_label(label: str)` — [`L31`](../../../../../raw/code/graphify/tests/test_multilang.py#L31)
- `_stmt_chain(start: ast.AST)` — [`L224`](../../../../../raw/code/graphify/tests/test_multilang.py#L224) — Walk up to each enclosing statement-list, returning (stmt, siblings).
- `test_cache_hit_returns_same_result(tmp_path)` — [`L429`](../../../../../raw/code/graphify/tests/test_multilang.py#L429)
- `test_cache_miss_after_file_change(tmp_path)` — [`L439`](../../../../../raw/code/graphify/tests/test_multilang.py#L439)
- `test_extract_dispatches_all_languages()` — [`L411`](../../../../../raw/code/graphify/tests/test_multilang.py#L411)
- `test_go_call_edges_have_call_context()` — [`L132`](../../../../../raw/code/graphify/tests/test_multilang.py#L132)
- `test_go_embeds_struct_field()` — [`L146`](../../../../../raw/code/graphify/tests/test_multilang.py#L146)
- `test_go_emits_calls()` — [`L115`](../../../../../raw/code/graphify/tests/test_multilang.py#L115)
- `test_go_finds_constructor()` — [`L111`](../../../../../raw/code/graphify/tests/test_multilang.py#L111)
- `test_go_finds_methods()` — [`L105`](../../../../../raw/code/graphify/tests/test_multilang.py#L105)
- `test_go_finds_struct()` — [`L100`](../../../../../raw/code/graphify/tests/test_multilang.py#L100)
- `test_go_has_extracted_calls()` — [`L120`](../../../../../raw/code/graphify/tests/test_multilang.py#L120)
- `test_go_import_edges_have_import_context()` — [`L125`](../../../../../raw/code/graphify/tests/test_multilang.py#L125)
- `test_go_interface_embedding_emits_embeds()` — [`L151`](../../../../../raw/code/graphify/tests/test_multilang.py#L151)
- `test_go_method_declaration_emits_refs_only_when_name_present()` — [`L167`](../../../../../raw/code/graphify/tests/test_multilang.py#L167) — Regression: review feedback flagged a hypothetical UnboundLocalError in
- `test_go_method_parameter_return_contexts()` — [`L161`](../../../../../raw/code/graphify/tests/test_multilang.py#L161)
- `test_go_no_dangling_edges()` — [`L138`](../../../../../raw/code/graphify/tests/test_multilang.py#L138)
- `test_go_struct_named_field_emits_field_context()` — [`L156`](../../../../../raw/code/graphify/tests/test_multilang.py#L156)
- `test_rust_call_edges_have_call_context()` — [`L325`](../../../../../raw/code/graphify/tests/test_multilang.py#L325)
- `test_rust_calls_are_extracted()` — [`L311`](../../../../../raw/code/graphify/tests/test_multilang.py#L311)
- `test_rust_emits_calls()` — [`L306`](../../../../../raw/code/graphify/tests/test_multilang.py#L306)
- `test_rust_enum_variant_references()` — [`L349`](../../../../../raw/code/graphify/tests/test_multilang.py#L349) — Enum variant payload types must emit `references` edges.
- `test_rust_finds_function()` — [`L302`](../../../../../raw/code/graphify/tests/test_multilang.py#L302)
- `test_rust_finds_impl_methods()` — [`L296`](../../../../../raw/code/graphify/tests/test_multilang.py#L296)
- `test_rust_finds_struct()` — [`L291`](../../../../../raw/code/graphify/tests/test_multilang.py#L291)
- `test_rust_import_edges_have_import_context()` — [`L318`](../../../../../raw/code/graphify/tests/test_multilang.py#L318)
- `test_rust_method_parameter_return_and_generic_contexts()` — [`L381`](../../../../../raw/code/graphify/tests/test_multilang.py#L381)
- `test_rust_no_cross_crate_spurious_edges()` — [`L388`](../../../../../raw/code/graphify/tests/test_multilang.py#L388) — Scoped calls (Type::method) and blocklisted names must not produce
- `test_rust_no_dangling_edges()` — [`L331`](../../../../../raw/code/graphify/tests/test_multilang.py#L331)
- `test_rust_struct_field_emits_field_context()` — [`L362`](../../../../../raw/code/graphify/tests/test_multilang.py#L362)
- `test_rust_supertrait_emits_inherits()` — [`L344`](../../../../../raw/code/graphify/tests/test_multilang.py#L344)
- `test_rust_trait_impl_emits_implements()` — [`L339`](../../../../../raw/code/graphify/tests/test_multilang.py#L339)
- `test_rust_tuple_struct_field_references()` — [`L368`](../../../../../raw/code/graphify/tests/test_multilang.py#L368) — Tuple struct fields (`struct Wrapper(A, B);`) nest their positional types
- `test_sql_alter_table_fk_edge()` — [`L490`](../../../../../raw/code/graphify/tests/test_multilang.py#L490) — ALTER TABLE ... FOREIGN KEY ... REFERENCES produces a references edge.
- `test_sql_emits_foreign_key_edge()` — [`L474`](../../../../../raw/code/graphify/tests/test_multilang.py#L474)
- `test_sql_emits_reads_from_edge()` — [`L479`](../../../../../raw/code/graphify/tests/test_multilang.py#L479)
- `test_sql_finds_function()` — [`L469`](../../../../../raw/code/graphify/tests/test_multilang.py#L469)
- `test_sql_finds_tables()` — [`L458`](../../../../../raw/code/graphify/tests/test_multilang.py#L458)
- `test_sql_finds_view()` — [`L464`](../../../../../raw/code/graphify/tests/test_multilang.py#L464)
- `test_sql_no_dangling_edges()` — [`L484`](../../../../../raw/code/graphify/tests/test_multilang.py#L484)
- `test_sql_schema_qualified_alter_fk()` — [`L507`](../../../../../raw/code/graphify/tests/test_multilang.py#L507) — ALTER TABLE with schema-qualified names produces correct edges.
- `test_sql_schema_qualified_names()` — [`L500`](../../../../../raw/code/graphify/tests/test_multilang.py#L500) — Schema-qualified table names (Schema.Table) are preserved.
- `test_ts_call_edges_have_call_context()` — [`L84`](../../../../../raw/code/graphify/tests/test_multilang.py#L84)
- `test_ts_calls_are_extracted()` — [`L70`](../../../../../raw/code/graphify/tests/test_multilang.py#L70)
- `test_ts_emits_calls()` — [`L64`](../../../../../raw/code/graphify/tests/test_multilang.py#L64)
- `test_ts_finds_class()` — [`L49`](../../../../../raw/code/graphify/tests/test_multilang.py#L49)
- `test_ts_finds_function()` — [`L60`](../../../../../raw/code/graphify/tests/test_multilang.py#L60)
- `test_ts_finds_methods()` — [`L54`](../../../../../raw/code/graphify/tests/test_multilang.py#L54)
- `test_ts_import_edges_have_import_context()` — [`L77`](../../../../../raw/code/graphify/tests/test_multilang.py#L77)
- `test_ts_no_dangling_edges()` — [`L90`](../../../../../raw/code/graphify/tests/test_multilang.py#L90)

## Module values
- `FIXTURES` — [`L8`](../../../../../raw/code/graphify/tests/test_multilang.py#L8)

