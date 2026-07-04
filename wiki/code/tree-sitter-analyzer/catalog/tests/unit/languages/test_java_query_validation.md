---
title: 'Module: tests/unit/languages/test_java_query_validation.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_query_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_query_validation`/
symbols:
  query: query().
  PETCLINIC_BASE: PETCLINIC_BASE.
  OWNER_CONTROLLER: OWNER_CONTROLLER.
  SPRING_BASE: SPRING_BASE.
  petclinic_server: petclinic_server().
  spring_server: spring_server().
  caffeine_server: caffeine_server().
  TestMatchPredicateFix.test_spring_controller_finds_owner_controller: TestMatchPredicateFix#test_spring_controller_finds_owner_controller().
  TestMatchPredicateFix.test_jpa_entity_finds_vet: TestMatchPredicateFix#test_jpa_entity_finds_vet().
  TestMatchPredicateFix.test_jpa_entity_finds_owner: TestMatchPredicateFix#test_jpa_entity_finds_owner().
  TestMatchPredicateFix.test_spring_service_not_in_controller: TestMatchPredicateFix#test_spring_service_not_in_controller().
  TestMatchPredicateFix.test_spring_controller_count_all_petclinic_controllers: TestMatchPredicateFix#test_spring_controller_count_all_petclinic_controllers().
  TestSpringBeanQuery.test_spring_bean_finds_cache_advisor: TestSpringBeanQuery#test_spring_bean_finds_cache_advisor().
  TestSpringBeanQuery.test_spring_configuration_finds_proxy_caching: TestSpringBeanQuery#test_spring_configuration_finds_proxy_caching().
  TestSpringBeanQuery.test_spring_transactional_finds_transactional_methods: TestSpringBeanQuery#test_spring_transactional_finds_transactional_methods().
  TestJUnit5Queries.test_junit5_test_finds_test_methods: TestJUnit5Queries#test_junit5_test_finds_test_methods().
  TestConcurrencyQueries.test_volatile_field_finds_caffeine_fields: TestConcurrencyQueries#test_volatile_field_finds_caffeine_fields().
  PROXY_CACHING: PROXY_CACHING.
  CAFFEINE_BASE: CAFFEINE_BASE.
  VET: VET.
  OWNER: OWNER.
  BOUNDED_LOCAL_CACHE: BOUNDED_LOCAL_CACHE.
  pytestmark_petclinic: pytestmark_petclinic.
  pytestmark_spring: pytestmark_spring.
  pytestmark_caffeine: pytestmark_caffeine.
  TestMatchPredicateFix: TestMatchPredicateFix#
  TestSpringBeanQuery: TestSpringBeanQuery#
  TestJUnit5Queries: TestJUnit5Queries#
  TestConcurrencyQueries: TestConcurrencyQueries#
  TestJava16RecordQuery.test_record_declaration_unit: TestJava16RecordQuery#test_record_declaration_unit().
  run: run().
  TestJava16RecordQuery: TestJava16RecordQuery#
---
# Module: [`tests/unit/languages/test_java_query_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py)

## Classes
### `TestConcurrencyQueries`
- def: [`tests/unit/languages/test_java_query_validation.py:237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L237)
- doc: volatile_field and other concurrency queries.
- signature: `class TestConcurrencyQueries:`
- members:
  - `test_volatile_field_finds_caffeine_fields(self, caffeine_server)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L240) — volatile_field must find volatile fields in BoundedLocalCache.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestJUnit5Queries`
- def: [`tests/unit/languages/test_java_query_validation.py:216`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L216)
- doc: junit5_test and related testing queries.
- signature: `class TestJUnit5Queries:`
- members:
  - `test_junit5_test_finds_test_methods(self, petclinic_server)` — [`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L219) — junit5_test must find @Test annotated methods in test files.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestJava16RecordQuery`
- def: [`tests/unit/languages/test_java_query_validation.py:251`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L251)
- doc: record_declaration query for Java 16+ records.
- signature: `class TestJava16RecordQuery:`
- members:
  - `test_record_declaration_unit(self)` — [`L254`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L254) — record_declaration must find Java record declarations.
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer)

### `TestMatchPredicateFix`
- def: [`tests/unit/languages/test_java_query_validation.py:105`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L105)
- doc: These queries use #match? — all return 0 before fix, correct count after.
- signature: `class TestMatchPredicateFix:`
- members:
  - `test_jpa_entity_finds_owner(self, petclinic_server)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L133) — jpa_entity must find @Entity annotated Owner class.
  - `test_jpa_entity_finds_vet(self, petclinic_server)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L123) — jpa_entity must find @Entity annotated Vet class.
  - `test_spring_controller_count_all_petclinic_controllers(self, petclinic_server)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L149) — spring_controller finds exactly 1 controller class in OwnerController.java.
  - `test_spring_controller_finds_owner_controller(self, petclinic_server)` — [`L108`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L108) — spring_controller must find @Controller annotated OwnerController.
  - `test_spring_service_not_in_controller(self, petclinic_server)` — [`L141`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L141) — spring_service must NOT find @Service in OwnerController (it's @Controller).
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestSpringBeanQuery`
- def: [`tests/unit/languages/test_java_query_validation.py:167`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L167)
- doc: spring_bean query: @Bean annotated methods in @Configuration classes.
- signature: `class TestSpringBeanQuery:`
- members:
  - `test_spring_bean_finds_cache_advisor(self, spring_server)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L170) — spring_bean must find @Bean methods in ProxyCachingConfiguration.
  - `test_spring_configuration_finds_proxy_caching(self, spring_server)` — [`L186`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L186) — spring_configuration must find @Configuration classes.
  - `test_spring_transactional_finds_transactional_methods(self, spring_server)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L196) — spring_transactional query must find @Transactional annotated methods.
- uses (calls/refs, reference-scoped): (3 test-only callers)

## Functions
- `caffeine_server()` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L74)
- `petclinic_server()` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L60)
- `query(server, file_path, query_key)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L86)
- `run(coro)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L80)
- `spring_server()` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L67)

## Module values
- `BOUNDED_LOCAL_CACHE` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L43)
- `CAFFEINE_BASE` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L26)
- `OWNER` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L35)
- `OWNER_CONTROLLER` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L28)
- `PETCLINIC_BASE` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L24)
- `PROXY_CACHING` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L39)
- `SPRING_BASE` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L25)
- `VET` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L32)
- `pytestmark_caffeine` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L54)
- `pytestmark_petclinic` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L48)
- `pytestmark_spring` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_query_validation.py#L51)

