---
title: 'Module: tests/unit/languages/test_java_caffeine_validation.py'
type: catalog
provenance: extracted
module: tests/unit/languages/test_java_caffeine_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages.test_java_caffeine_validation`/
symbols:
  TestImplementsGenerics.test_interface_extends_extracted_as_implements: TestImplementsGenerics#test_interface_extends_extracted_as_implements().
  TestAnnotationAttribution.test_override_never_on_class_unit: TestAnnotationAttribution#test_override_never_on_class_unit().
  TestAnnotationAttribution.test_annotation_attribution_direct_ast: TestAnnotationAttribution#test_annotation_attribution_direct_ast().
  TestImplementsGenerics.test_implements_generic_preserved_unit: TestImplementsGenerics#test_implements_generic_preserved_unit().
  TestImplementsGenerics.test_implements_multiple_generic_interfaces: TestImplementsGenerics#test_implements_multiple_generic_interfaces().
  TestAnnotationAttribution.test_caffeine_no_override_on_any_class: TestAnnotationAttribution#test_caffeine_no_override_on_any_class().
  TestAnnotationAttribution.test_references_inner_classes_clean_annotations: TestAnnotationAttribution#test_references_inner_classes_clean_annotations().
  TestImplementsGenerics.test_caffeine_bounded_local_cache_implements: TestImplementsGenerics#test_caffeine_bounded_local_cache_implements().
  TestBoundedLocalCacheSynthetic.mcp_result: TestBoundedLocalCacheSynthetic#mcp_result().
  _skip_caffeine: _skip_caffeine.
  mcp_server: mcp_server().
  BOUNDED_LOCAL_CACHE: BOUNDED_LOCAL_CACHE.
  CAFFEINE_BASE: CAFFEINE_BASE.
  REFERENCES: REFERENCES.
  call: call().
  TestBoundedLocalCacheSynthetic._classes: TestBoundedLocalCacheSynthetic#_classes().
  TestBoundedLocalCacheSynthetic.test_bounded_local_cache_implements_generics_preserved: TestBoundedLocalCacheSynthetic#test_bounded_local_cache_implements_generics_preserved().
  TestBoundedLocalCacheSynthetic.test_bounded_eviction_no_override_bleed: TestBoundedLocalCacheSynthetic#test_bounded_eviction_no_override_bleed().
  TestBoundedLocalCacheSynthetic.test_legacy_node_has_deprecated_annotation: TestBoundedLocalCacheSynthetic#test_legacy_node_has_deprecated_annotation().
  TestAnnotationAttribution.METHOD_ONLY_ANNOTATIONS: TestAnnotationAttribution#METHOD_ONLY_ANNOTATIONS.
  TestBoundedLocalCacheSynthetic._SRC: TestBoundedLocalCacheSynthetic#_SRC.
  TestImplementsGenerics: TestImplementsGenerics#
  TestAnnotationAttribution: TestAnnotationAttribution#
  TestBoundedLocalCacheSynthetic: TestBoundedLocalCacheSynthetic#
---
# Module: [`tests/unit/languages/test_java_caffeine_validation.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py)

## Classes
### `TestAnnotationAttribution`
- def: [`tests/unit/languages/test_java_caffeine_validation.py:199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L199)
- doc: @Override and other method-only annotations must never appear on classes.
- signature: `class TestAnnotationAttribution:`
- members:
  - `test_annotation_attribution_direct_ast(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L307) — Class annotations should come from AST modifiers, not line proximity.
  - `test_caffeine_no_override_on_any_class(self, mcp_server)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L260) — No class in BoundedLocalCache should have @Override in its annotations.
  - `test_override_never_on_class_unit(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L214) — @Override on a method must not bleed into the next class's annotations.
  - `test_references_inner_classes_clean_annotations(self, mcp_server)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L285) — Inner classes in References.java should have no spurious annotations.
  - `METHOD_ONLY_ANNOTATIONS` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L202)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_classes), [`extract_annotations`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_annotations), [`annotations`](../../../tree_sitter_analyzer/models/base.md#Class.annotations)  (4 test-only)

### `TestBoundedLocalCacheSynthetic`
- def: [`tests/unit/languages/test_java_caffeine_validation.py:351`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L351)
- doc: End-to-end MCP validation of Bug 1 and Bug 2 fixes using a synthetic file.
- signature: `class TestBoundedLocalCacheSynthetic:`
- members:
  - `mcp_result(self, tmp_path_factory)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L404)
  - `test_bounded_eviction_no_override_bleed(self, mcp_result)` — [`L448`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L448) — Bug 2 via MCP: @Override from BoundedLocalCache.run() must not bleed to BoundedEviction.
  - `test_bounded_local_cache_implements_generics_preserved(self, mcp_result)` — [`L427`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L427) — Bug 1 via MCP: LocalCache<K, V> must appear as one item, not split.
  - `test_legacy_node_has_deprecated_annotation(self, mcp_result)` — [`L461`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L461) — Class-level annotation MCP round-trip: @Deprecated must reach LegacyNode.
- protocol/private: `_SRC`[`L362`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L362), `_classes`[`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L423)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerMCPServer`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer), [`call_tool`](../../../tree_sitter_analyzer/mcp/server.md#TreeSitterAnalyzerMCPServer.call_tool)

### `TestImplementsGenerics`
- def: [`tests/unit/languages/test_java_caffeine_validation.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L47)
- doc: implements with generic type parameters must be preserved as complete strings.
- signature: `class TestImplementsGenerics:`
- members:
  - `test_caffeine_bounded_local_cache_implements(self, mcp_server)` — [`L166`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L166) — BoundedLocalCache must show 'LocalCache<K, V>' not split into 3 items.
  - `test_implements_generic_preserved_unit(self)` — [`L50`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L50) — Unit test: LocalCache<K, V> must stay as one item, not split into three.
  - `test_implements_multiple_generic_interfaces(self)` — [`L84`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L84) — Multiple generic interfaces must each be preserved as a complete string.
  - `test_interface_extends_extracted_as_implements(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L121) — [TDD] Java interface extends clause must be captured in implements_interfaces.
- uses (calls/refs, reference-scoped): [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`JavaElementExtractor`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor), [`extract_classes`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_classes), [`extract_annotations`](../../../tree_sitter_analyzer/languages/java_plugin.md#JavaElementExtractor.extract_annotations), [`implements_interfaces`](../../../tree_sitter_analyzer/models/base.md#Class.implements_interfaces)  (3 test-only)

## Functions
- `call(coro)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L40)
- `mcp_server()` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L34)

## Module values
- `BOUNDED_LOCAL_CACHE` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L22)
- `CAFFEINE_BASE` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L19)
- `REFERENCES` — [`L25`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L25)
- `_skip_caffeine` — [`L27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/test_java_caffeine_validation.py#L27)

