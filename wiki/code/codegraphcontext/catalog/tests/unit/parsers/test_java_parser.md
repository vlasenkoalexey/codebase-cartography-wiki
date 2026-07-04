---
title: 'Module: tests/unit/parsers/test_java_parser.py'
type: catalog
provenance: extracted
module: tests/unit/parsers/test_java_parser.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.parsers.test_java_parser`/
symbols:
  _write_and_parse: _write_and_parse().
  TestJavaCrossFileResolution.test_di_call_resolves_to_cross_file_path: TestJavaCrossFileResolution#test_di_call_resolves_to_cross_file_path().
  TestJavaDiCrossFileCalls.test_di_field_call_has_inferred_obj_type: TestJavaDiCrossFileCalls#test_di_field_call_has_inferred_obj_type().
  TestJavaDiCrossFileCalls.test_second_di_call_on_same_field_also_inferred: TestJavaDiCrossFileCalls#test_second_di_call_on_same_field_also_inferred().
  TestJavaDiCrossFileCalls.test_calls_without_receiver_have_no_inferred_type: TestJavaDiCrossFileCalls#test_calls_without_receiver_have_no_inferred_type().
  TestJavaDiCrossFileCalls.test_generic_field_strips_type_parameter: TestJavaDiCrossFileCalls#test_generic_field_strips_type_parameter().
  TestJavaCrossFileResolution.test_non_di_call_stays_in_caller_file: TestJavaCrossFileResolution#test_non_di_call_stays_in_caller_file().
  TestOrmMappingExtraction.test_jpa_entity_table_mapping: TestOrmMappingExtraction#test_jpa_entity_table_mapping().
  TestOrmMappingExtraction.test_cassandra_table_mapping: TestOrmMappingExtraction#test_cassandra_table_mapping().
  TestOrmMappingExtraction.test_redis_hash_mapping: TestOrmMappingExtraction#test_redis_hash_mapping().
  TestOrmMappingExtraction.test_spring_query_read_detection: TestOrmMappingExtraction#test_spring_query_read_detection().
  TestOrmMappingExtraction.test_spring_query_write_detection: TestOrmMappingExtraction#test_spring_query_write_detection().
  TestOrmMappingExtraction.test_mybatis_select_annotation: TestOrmMappingExtraction#test_mybatis_select_annotation().
  TestOrmMappingExtraction.test_mybatis_insert_annotation: TestOrmMappingExtraction#test_mybatis_insert_annotation().
  TestOrmMappingExtraction.test_orm_mappings_key_present: TestOrmMappingExtraction#test_orm_mappings_key_present().
  SPRING_DATA_REPO_SRC: SPRING_DATA_REPO_SRC.
  TestSpringDataRepoDetection.test_spring_data_reads_emitted: TestSpringDataRepoDetection#test_spring_data_reads_emitted().
  TestSpringDataRepoDetection.test_spring_data_writes_emitted: TestSpringDataRepoDetection#test_spring_data_writes_emitted().
  TestSpringDataRepoDetection.test_spring_data_entity_class_extracted: TestSpringDataRepoDetection#test_spring_data_entity_class_extracted().
  TestSpringDataRepoDetection.test_spring_data_crud_repo_detected: TestSpringDataRepoDetection#test_spring_data_crud_repo_detected().
  TestSpringDataRepoDetection.test_spring_data_class_name_set: TestSpringDataRepoDetection#test_spring_data_class_name_set().
  CONTROLLER_SRC: CONTROLLER_SRC.
  WORK_SERVICE_SRC: WORK_SERVICE_SRC.
  TestJavaParameterParsing.test_annotation_string_commas_do_not_split_parameters: TestJavaParameterParsing#test_annotation_string_commas_do_not_split_parameters().
  TestJavaParameterParsing.test_annotation_array_values_do_not_split_parameters: TestJavaParameterParsing#test_annotation_array_values_do_not_split_parameters().
  TestJavaParameterParsing.test_final_with_non_space_whitespace_is_stripped: TestJavaParameterParsing#test_final_with_non_space_whitespace_is_stripped().
  SPRING_QUERY_SRC: SPRING_QUERY_SRC.
  MYBATIS_SRC: MYBATIS_SRC.
  GENERIC_FIELD_SRC: GENERIC_FIELD_SRC.
  JPA_ENTITY_SRC: JPA_ENTITY_SRC.
  CASSANDRA_TABLE_SRC: CASSANDRA_TABLE_SRC.
  REDIS_HASH_SRC: REDIS_HASH_SRC.
  parser: parser().
  TestJavaDiCrossFileCalls: TestJavaDiCrossFileCalls#
  TestJavaDiCrossFileCalls.test_strip_generic_static_method: TestJavaDiCrossFileCalls#test_strip_generic_static_method().
  TestJavaParameterParsing: TestJavaParameterParsing#
  TestJavaCrossFileResolution: TestJavaCrossFileResolution#
  TestJavaCrossFileResolution.test_super_call_without_base_context_stays_in_caller_file: TestJavaCrossFileResolution#test_super_call_without_base_context_stays_in_caller_file().
  TestOrmMappingExtraction: TestOrmMappingExtraction#
  TestSpringDataRepoDetection: TestSpringDataRepoDetection#
---
# Module: [`tests/unit/parsers/test_java_parser.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py)

## Classes
### `TestJavaCrossFileResolution`
- def: [`tests/unit/parsers/test_java_parser.py:233`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L233)
- signature: `class TestJavaCrossFileResolution:`
- members:
  - `test_di_call_resolves_to_cross_file_path(self, parser)` — [`L235`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L235) — End-to-end: workService.doWork() resolves to WorkService.java, not self.
  - `test_non_di_call_stays_in_caller_file(self, parser)` — [`L274`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L274) — Calls where the receiver is not a known typed variable stay in the caller file.
  - `test_super_call_without_base_context_stays_in_caller_file(self)` — [`L297`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L297) — Non-Kotlin super.method() calls must not resolve to unrelated same-name symbols.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestJavaDiCrossFileCalls`
- def: [`tests/unit/parsers/test_java_parser.py:112`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L112)
- signature: `class TestJavaDiCrossFileCalls:`
- members:
  - `test_calls_without_receiver_have_no_inferred_type(self, parser)` — [`L137`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L137) — Bare method calls (no object receiver) must have inferred_obj_type=None.
  - `test_di_field_call_has_inferred_obj_type(self, parser)` — [`L114`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L114) — workService.doWork() must carry inferred_obj_type='WorkService' (fix for #823).
  - `test_generic_field_strips_type_parameter(self, parser)` — [`L146`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L146) — List<WorkService> field receiver resolves to 'List', not 'WorkService'.
  - `test_second_di_call_on_same_field_also_inferred(self, parser)` — [`L128`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L128) — workService.computeResult() must also carry inferred_obj_type='WorkService'.
  - `test_strip_generic_static_method(self, parser)` — [`L154`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L154) — Verify _strip_generic handles all common forms correctly.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestJavaParameterParsing`
- def: [`tests/unit/parsers/test_java_parser.py:162`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L162)
- signature: `class TestJavaParameterParsing:`
- members:
  - `test_annotation_array_values_do_not_split_parameters(self, parser)` — [`L186`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L186)
  - `test_annotation_string_commas_do_not_split_parameters(self, parser)` — [`L163`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L163)
  - `test_final_with_non_space_whitespace_is_stripped(self, parser)` — [`L205`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L205)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `TestOrmMappingExtraction`
- def: [`tests/unit/parsers/test_java_parser.py:395`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L395)
- signature: `class TestOrmMappingExtraction:`
- members:
  - `test_cassandra_table_mapping(self, parser)` — [`L405`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L405)
  - `test_jpa_entity_table_mapping(self, parser)` — [`L396`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L396)
  - `test_mybatis_insert_annotation(self, parser)` — [`L443`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L443)
  - `test_mybatis_select_annotation(self, parser)` — [`L437`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L437)
  - `test_orm_mappings_key_present(self, parser)` — [`L449`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L449) — orm_mappings key must always be present in parse() output.
  - `test_redis_hash_mapping(self, parser)` — [`L413`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L413)
  - `test_spring_query_read_detection(self, parser)` — [`L421`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L421)
  - `test_spring_query_write_detection(self, parser)` — [`L429`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L429)
- uses (calls/refs, reference-scoped): (7 test-only callers)

### `TestSpringDataRepoDetection`
- def: [`tests/unit/parsers/test_java_parser.py:492`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L492)
- signature: `class TestSpringDataRepoDetection:`
- members:
  - `test_spring_data_class_name_set(self, parser)` — [`L519`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L519)
  - `test_spring_data_crud_repo_detected(self, parser)` — [`L513`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L513)
  - `test_spring_data_entity_class_extracted(self, parser)` — [`L506`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L506)
  - `test_spring_data_reads_emitted(self, parser)` — [`L493`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L493)
  - `test_spring_data_writes_emitted(self, parser)` — [`L499`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L499)
- uses (calls/refs, reference-scoped): (2 test-only callers)

## Functions
- `_write_and_parse(parser, src: str, suffix: str = ".java")` — [`L40`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L40) — Write src to a temp file and parse it.
- `parser()` — [`L31`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L31)

## Module values
- `CASSANDRA_TABLE_SRC` — [`L343`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L343)
- `CONTROLLER_SRC` — [`L57`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L57)
- `GENERIC_FIELD_SRC` — [`L91`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L91)
- `JPA_ENTITY_SRC` — [`L325`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L325)
- `MYBATIS_SRC` — [`L379`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L379)
- `REDIS_HASH_SRC` — [`L354`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L354)
- `SPRING_DATA_REPO_SRC` — [`L460`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L460)
- `SPRING_QUERY_SRC` — [`L365`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L365)
- `WORK_SERVICE_SRC` — [`L77`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_parser.py#L77)

