---
title: 'Module: tests/test_pascal.py'
type: catalog
provenance: extracted
module: tests/test_pascal.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_pascal`/
symbols:
  FIXTURES: FIXTURES.
  _labels: _labels().
  test_pascal_finds_unit: test_pascal_finds_unit().
  test_pascal_finds_classes: test_pascal_finds_classes().
  test_pascal_finds_interface: test_pascal_finds_interface().
  test_pascal_finds_methods: test_pascal_finds_methods().
  test_pascal_finds_imports: test_pascal_finds_imports().
  test_pascal_import_edges_have_import_context: test_pascal_import_edges_have_import_context().
  test_pascal_finds_inherits: test_pascal_finds_inherits().
  test_pascal_finds_calls: test_pascal_finds_calls().
  test_pascal_call_edges_have_call_context: test_pascal_call_edges_have_call_context().
  test_lfm_finds_root_form_class: test_lfm_finds_root_form_class().
  test_lfm_finds_component_classes: test_lfm_finds_component_classes().
  test_lfm_finds_event_handlers: test_lfm_finds_event_handlers().
  test_lfm_contains_edges_form_hierarchy: test_lfm_contains_edges_form_hierarchy().
  test_lpk_finds_package_name: test_lpk_finds_package_name().
  test_lpk_finds_required_packages: test_lpk_finds_required_packages().
  test_lpk_imports_edges_have_import_context: test_lpk_imports_edges_have_import_context().
  test_lpk_contains_listed_units: test_lpk_contains_listed_units().
  test_dfm_finds_root_form_class: test_dfm_finds_root_form_class().
  test_dfm_finds_component_classes: test_dfm_finds_component_classes().
  test_dfm_finds_event_handlers: test_dfm_finds_event_handlers().
  test_dfm_contains_edges_form_hierarchy: test_dfm_contains_edges_form_hierarchy().
  _relations: _relations().
  test_pascal_no_error: test_pascal_no_error().
  test_pascal_inherits_from_base: test_pascal_inherits_from_base().
  test_pascal_all_edges_extracted: test_pascal_all_edges_extracted().
  test_pascal_no_dangling_edges: test_pascal_no_dangling_edges().
  test_lfm_no_error: test_lfm_no_error().
  test_lfm_event_edges_have_event_context: test_lfm_event_edges_have_event_context().
  test_lfm_no_dangling_edges: test_lfm_no_dangling_edges().
  test_lpk_no_error: test_lpk_no_error().
  test_lpk_no_dangling_edges: test_lpk_no_dangling_edges().
  test_dfm_no_error: test_dfm_no_error().
  test_dfm_event_edges_have_event_context: test_dfm_event_edges_have_event_context().
  test_dfm_no_dangling_edges: test_dfm_no_dangling_edges().
  _edges_with_relation: _edges_with_relation().
  test_pascal_dispatch_registered: test_pascal_dispatch_registered().
  test_pascal_detect_extensions_registered: test_pascal_detect_extensions_registered().
  test_dfm_binary_returns_empty_not_crash: test_dfm_binary_returns_empty_not_crash().
  test_dfm_dispatch_registered: test_dfm_dispatch_registered().
  test_dfm_detect_extension_registered: test_dfm_detect_extension_registered().
---
# Module: [`tests/test_pascal.py`](../../../../../raw/code/graphify/tests/test_pascal.py)

## Functions
- `_edges_with_relation(r, *relations)` — [`L16`](../../../../../raw/code/graphify/tests/test_pascal.py#L16)
- `_labels(r)` — [`L8`](../../../../../raw/code/graphify/tests/test_pascal.py#L8)
- `_relations(r)` — [`L12`](../../../../../raw/code/graphify/tests/test_pascal.py#L12)
- `test_dfm_binary_returns_empty_not_crash()` — [`L299`](../../../../../raw/code/graphify/tests/test_pascal.py#L299)
- `test_dfm_contains_edges_form_hierarchy()` — [`L285`](../../../../../raw/code/graphify/tests/test_pascal.py#L285)
- `test_dfm_detect_extension_registered()` — [`L320`](../../../../../raw/code/graphify/tests/test_pascal.py#L320)
- `test_dfm_dispatch_registered()` — [`L315`](../../../../../raw/code/graphify/tests/test_pascal.py#L315)
- `test_dfm_event_edges_have_event_context()` — [`L277`](../../../../../raw/code/graphify/tests/test_pascal.py#L277)
- `test_dfm_finds_component_classes()` — [`L259`](../../../../../raw/code/graphify/tests/test_pascal.py#L259)
- `test_dfm_finds_event_handlers()` — [`L269`](../../../../../raw/code/graphify/tests/test_pascal.py#L269)
- `test_dfm_finds_root_form_class()` — [`L253`](../../../../../raw/code/graphify/tests/test_pascal.py#L253)
- `test_dfm_no_dangling_edges()` — [`L291`](../../../../../raw/code/graphify/tests/test_pascal.py#L291)
- `test_dfm_no_error()` — [`L247`](../../../../../raw/code/graphify/tests/test_pascal.py#L247)
- `test_lfm_contains_edges_form_hierarchy()` — [`L185`](../../../../../raw/code/graphify/tests/test_pascal.py#L185)
- `test_lfm_event_edges_have_event_context()` — [`L177`](../../../../../raw/code/graphify/tests/test_pascal.py#L177)
- `test_lfm_finds_component_classes()` — [`L159`](../../../../../raw/code/graphify/tests/test_pascal.py#L159)
- `test_lfm_finds_event_handlers()` — [`L169`](../../../../../raw/code/graphify/tests/test_pascal.py#L169)
- `test_lfm_finds_root_form_class()` — [`L153`](../../../../../raw/code/graphify/tests/test_pascal.py#L153)
- `test_lfm_no_dangling_edges()` — [`L191`](../../../../../raw/code/graphify/tests/test_pascal.py#L191)
- `test_lfm_no_error()` — [`L147`](../../../../../raw/code/graphify/tests/test_pascal.py#L147)
- `test_lpk_contains_listed_units()` — [`L229`](../../../../../raw/code/graphify/tests/test_pascal.py#L229)
- `test_lpk_finds_package_name()` — [`L207`](../../../../../raw/code/graphify/tests/test_pascal.py#L207)
- `test_lpk_finds_required_packages()` — [`L213`](../../../../../raw/code/graphify/tests/test_pascal.py#L213)
- `test_lpk_imports_edges_have_import_context()` — [`L221`](../../../../../raw/code/graphify/tests/test_pascal.py#L221)
- `test_lpk_no_dangling_edges()` — [`L237`](../../../../../raw/code/graphify/tests/test_pascal.py#L237)
- `test_lpk_no_error()` — [`L201`](../../../../../raw/code/graphify/tests/test_pascal.py#L201)
- `test_pascal_all_edges_extracted()` — [`L102`](../../../../../raw/code/graphify/tests/test_pascal.py#L102)
- `test_pascal_call_edges_have_call_context()` — [`L94`](../../../../../raw/code/graphify/tests/test_pascal.py#L94)
- `test_pascal_detect_extensions_registered()` — [`L135`](../../../../../raw/code/graphify/tests/test_pascal.py#L135)
- `test_pascal_dispatch_registered()` — [`L123`](../../../../../raw/code/graphify/tests/test_pascal.py#L123)
- `test_pascal_finds_calls()` — [`L88`](../../../../../raw/code/graphify/tests/test_pascal.py#L88)
- `test_pascal_finds_classes()` — [`L32`](../../../../../raw/code/graphify/tests/test_pascal.py#L32)
- `test_pascal_finds_imports()` — [`L56`](../../../../../raw/code/graphify/tests/test_pascal.py#L56)
- `test_pascal_finds_inherits()` — [`L70`](../../../../../raw/code/graphify/tests/test_pascal.py#L70)
- `test_pascal_finds_interface()` — [`L40`](../../../../../raw/code/graphify/tests/test_pascal.py#L40)
- `test_pascal_finds_methods()` — [`L46`](../../../../../raw/code/graphify/tests/test_pascal.py#L46)
- `test_pascal_finds_unit()` — [`L26`](../../../../../raw/code/graphify/tests/test_pascal.py#L26)
- `test_pascal_import_edges_have_import_context()` — [`L62`](../../../../../raw/code/graphify/tests/test_pascal.py#L62)
- `test_pascal_inherits_from_base()` — [`L76`](../../../../../raw/code/graphify/tests/test_pascal.py#L76)
- `test_pascal_no_dangling_edges()` — [`L111`](../../../../../raw/code/graphify/tests/test_pascal.py#L111)
- `test_pascal_no_error()` — [`L20`](../../../../../raw/code/graphify/tests/test_pascal.py#L20)

## Module values
- `FIXTURES` — [`L5`](../../../../../raw/code/graphify/tests/test_pascal.py#L5)

