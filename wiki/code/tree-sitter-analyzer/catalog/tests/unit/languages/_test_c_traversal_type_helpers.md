---
title: 'Module: tests/unit/languages/_test_c_traversal_type_helpers.py'
type: catalog
provenance: extracted
module: tests/unit/languages/_test_c_traversal_type_helpers.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.languages._test_c_traversal_type_helpers`/
symbols:
  FakeNode: FakeNode#
  FakeNode.children: FakeNode#children.
  TestExtractStructDefinition.test_named_struct: TestExtractStructDefinition#test_named_struct().
  TestExtractEnumDefinition.test_named_enum: TestExtractEnumDefinition#test_named_enum().
  TestExtractEnumDefinition.test_typedef_enum: TestExtractEnumDefinition#test_typedef_enum().
  TestTypeNameAndRange.test_typedef_name: TestTypeNameAndRange#test_typedef_name().
  TestExtractStructDefinition.test_anonymous_struct: TestExtractStructDefinition#test_anonymous_struct().
  TestExtractEnumDefinition.test_anonymous_enum: TestExtractEnumDefinition#test_anonymous_enum().
  _get_node_text: _get_node_text().
  TestTypedefTypeName.test_typedef_parent: TestTypedefTypeName#test_typedef_parent().
  TestDirectTypeName.test_finds_type_identifier: TestDirectTypeName#test_finds_type_identifier().
  TestTypeNameAndRange.test_direct_name: TestTypeNameAndRange#test_direct_name().
  FakeNode.text: FakeNode#text.
  FakeNode.start_point: FakeNode#start_point.
  TestProcessTargetNode.test_new_node_processed: TestProcessTargetNode#test_new_node_processed().
  TestDirectTypeName.test_no_type_identifier: TestDirectTypeName#test_no_type_identifier().
  TestTypedefTypeName.test_non_typedef_parent: TestTypedefTypeName#test_non_typedef_parent().
  TestNodeLineRange.test_basic: TestNodeLineRange#test_basic().
  TestTypeNameAndRange.test_anonymous: TestTypeNameAndRange#test_anonymous().
  TestExtractStructDefinition.test_exception_returns_none: TestExtractStructDefinition#test_exception_returns_none().
  TestExtractEnumDefinition.test_exception_returns_none: TestExtractEnumDefinition#test_exception_returns_none().
  FakeNode.end_point: FakeNode#end_point.
  TestPushChildren.test_pushes_children: TestPushChildren#test_pushes_children().
  TestPushChildren.test_no_children: TestPushChildren#test_no_children().
  TestCTraverseAndExtract.test_single_target_node: TestCTraverseAndExtract#test_single_target_node().
  TestCTraverseAndExtract.test_nested_in_container: TestCTraverseAndExtract#test_nested_in_container().
  TestCTraverseAndExtract.test_multiple_targets: TestCTraverseAndExtract#test_multiple_targets().
  TestCTraverseAndExtract.test_empty_extractors: TestCTraverseAndExtract#test_empty_extractors().
  TestCTraverseAndExtract.test_depth_limit_respected: TestCTraverseAndExtract#test_depth_limit_respected().
  TestTypedefTypeName.test_no_parent: TestTypedefTypeName#test_no_parent().
  FakeNode.parent: FakeNode#parent.
  FakeNode.child_by_field_name: FakeNode#child_by_field_name().
  TestShouldVisitNode.test_root_depth_always_true: TestShouldVisitNode#test_root_depth_always_true().
  TestShouldVisitNode.test_target_node_type: TestShouldVisitNode#test_target_node_type().
  TestShouldVisitNode.test_container_node_type: TestShouldVisitNode#test_container_node_type().
  TestShouldVisitNode.test_irrelevant_node_type: TestShouldVisitNode#test_irrelevant_node_type().
  TestProcessTargetNode.test_already_processed_skipped: TestProcessTargetNode#test_already_processed_skipped().
  TestProcessTargetNode.test_cached_element_reused: TestProcessTargetNode#test_cached_element_reused().
  TestProcessTargetNode.test_list_extractor_result: TestProcessTargetNode#test_list_extractor_result().
  FakeNode.fields: FakeNode#fields.
  TestDepthExceeded.test_within_limit: TestDepthExceeded#test_within_limit().
  TestDepthExceeded.test_at_limit: TestDepthExceeded#test_at_limit().
  TestDepthExceeded.test_over_limit: TestDepthExceeded#test_over_limit().
  TestDepthExceeded.test_zero_depth: TestDepthExceeded#test_zero_depth().
  TestAppendExtractedElement.test_single_element: TestAppendExtractedElement#test_single_element().
  TestAppendExtractedElement.test_list_element: TestAppendExtractedElement#test_list_element().
  TestAppendExtractedElement.test_none_element: TestAppendExtractedElement#test_none_element().
  TestAppendExtractedElement.test_empty_list: TestAppendExtractedElement#test_empty_list().
  TestCTraverseAndExtract.test_none_root: TestCTraverseAndExtract#test_none_root().
  TestRawText.test_basic: TestRawText#test_basic().
  TestRawText.test_empty: TestRawText#test_empty().
  FakeNode.start_byte: FakeNode#start_byte.
  FakeNode.end_byte: FakeNode#end_byte.
  TestDepthExceeded: TestDepthExceeded#
  TestShouldVisitNode: TestShouldVisitNode#
  TestAppendExtractedElement: TestAppendExtractedElement#
  TestProcessTargetNode: TestProcessTargetNode#
  TestPushChildren: TestPushChildren#
  TestCTraverseAndExtract: TestCTraverseAndExtract#
  TestDirectTypeName: TestDirectTypeName#
  TestTypedefTypeName: TestTypedefTypeName#
  TestRawText: TestRawText#
  TestNodeLineRange: TestNodeLineRange#
  TestTypeNameAndRange: TestTypeNameAndRange#
  TestExtractStructDefinition: TestExtractStructDefinition#
  TestExtractEnumDefinition: TestExtractEnumDefinition#
---
# Module: [`tests/unit/languages/_test_c_traversal_type_helpers.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py)

## Classes
### `FakeNode`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L28)
- signature: `class FakeNode:`
- members:
  - `child_by_field_name(self, name: str)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L39)
  - `children` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L31)
  - `end_byte` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L36)
  - `end_point` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L34)
  - `fields` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L32)
  - `parent` — [`L37`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L37)
  - `start_byte` — [`L35`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L35)
  - `start_point` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L33)
  - `text` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L30)
- used by: (31 test-only callers)

### `TestAppendExtractedElement`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L79)
- signature: `class TestAppendExtractedElement:`
- members:
  - `test_empty_list(self)` — [`L95`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L95)
  - `test_list_element(self)` — [`L85`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L85)
  - `test_none_element(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L90)
  - `test_single_element(self)` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L80)
- uses (calls/refs, reference-scoped): [`_append_extracted_element`](../../../tree_sitter_analyzer/languages/_c_traversal_helpers.md#_append_extracted_element)

### `TestCTraverseAndExtract`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L164)
- signature: `class TestCTraverseAndExtract:`
- members:
  - `test_depth_limit_respected(self)` — [`L206`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L206)
  - `test_empty_extractors(self)` — [`L200`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L200)
  - `test_multiple_targets(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L187)
  - `test_nested_in_container(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L178)
  - `test_none_root(self)` — [`L165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L165)
  - `test_single_target_node(self)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L170)
- uses (calls/refs, reference-scoped): [`c_traverse_and_extract`](../../../tree_sitter_analyzer/languages/_c_traversal_helpers.md#c_traverse_and_extract)  (2 test-only)

### `TestDepthExceeded`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L47)
- signature: `class TestDepthExceeded:`
- members:
  - `test_at_limit(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L51)
  - `test_over_limit(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L54)
  - `test_within_limit(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L48)
  - `test_zero_depth(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L57)
- uses (calls/refs, reference-scoped): [`_depth_exceeded`](../../../tree_sitter_analyzer/languages/_c_traversal_helpers.md#_depth_exceeded)

### `TestDirectTypeName`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:219`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L219)
- signature: `class TestDirectTypeName:`
- members:
  - `test_finds_type_identifier(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L220)
  - `test_no_type_identifier(self)` — [`L230`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L230)
- uses (calls/refs, reference-scoped): [`_direct_type_name`](../../../tree_sitter_analyzer/languages/_c_type_definition_helpers.md#_direct_type_name)  (4 test-only)

### `TestExtractEnumDefinition`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:381`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L381)
- signature: `class TestExtractEnumDefinition:`
- members:
  - `test_anonymous_enum(self)` — [`L404`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L404)
  - `test_exception_returns_none(self)` — [`L424`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L424)
  - `test_named_enum(self)` — [`L382`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L382)
  - `test_typedef_enum(self)` — [`L430`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L430)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`extract_enum_definition`](../../../tree_sitter_analyzer/languages/_c_type_definition_helpers.md#extract_enum_definition)  (7 test-only)

### `TestExtractStructDefinition`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:327`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L327)
- signature: `class TestExtractStructDefinition:`
- members:
  - `test_anonymous_struct(self)` — [`L354`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L354)
  - `test_exception_returns_none(self)` — [`L374`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L374)
  - `test_named_struct(self)` — [`L328`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L328)
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`language`](../../../tree_sitter_analyzer/models/base.md#CodeElement.language), [`class_type`](../../../tree_sitter_analyzer/models/base.md#Class.class_type), [`extract_struct_definition`](../../../tree_sitter_analyzer/languages/_c_type_definition_helpers.md#extract_struct_definition)  (6 test-only)

### `TestNodeLineRange`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L278)
- signature: `class TestNodeLineRange:`
- members:
  - `test_basic(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L279)
- uses (calls/refs, reference-scoped): [`_node_line_range`](../../../tree_sitter_analyzer/languages/_c_type_definition_helpers.md#_node_line_range)  (3 test-only)

### `TestProcessTargetNode`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:101`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L101)
- signature: `class TestProcessTargetNode:`
- members:
  - `test_already_processed_skipped(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L115)
  - `test_cached_element_reused(self)` — [`L127`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L127)
  - `test_list_extractor_result(self)` — [`L136`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L136)
  - `test_new_node_processed(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L102)
- uses (calls/refs, reference-scoped): [`_process_target_node`](../../../tree_sitter_analyzer/languages/_c_traversal_helpers.md#_process_target_node)  (3 test-only)

### `TestPushChildren`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:146`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L146)
- signature: `class TestPushChildren:`
- members:
  - `test_no_children(self)` — [`L157`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L157)
  - `test_pushes_children(self)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L147)
- uses (calls/refs, reference-scoped): [`_push_children`](../../../tree_sitter_analyzer/languages/_c_traversal_helpers.md#_push_children)  (2 test-only)

### `TestRawText`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L267)
- signature: `class TestRawText:`
- members:
  - `test_basic(self)` — [`L268`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L268)
  - `test_empty(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L274)
- uses (calls/refs, reference-scoped): [`_raw_text`](../../../tree_sitter_analyzer/languages/_c_type_definition_helpers.md#_raw_text)

### `TestShouldVisitNode`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:61`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L61)
- signature: `class TestShouldVisitNode:`
- members:
  - `test_container_node_type(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L70)
  - `test_irrelevant_node_type(self)` — [`L74`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L74)
  - `test_root_depth_always_true(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L62)
  - `test_target_node_type(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L66)
- uses (calls/refs, reference-scoped): [`_should_visit_node`](../../../tree_sitter_analyzer/languages/_c_traversal_helpers.md#_should_visit_node)  (1 test-only)

### `TestTypeNameAndRange`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L286)
- signature: `class TestTypeNameAndRange:`
- members:
  - `test_anonymous(self)` — [`L314`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L314)
  - `test_direct_name(self)` — [`L287`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L287)
  - `test_typedef_name(self)` — [`L299`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L299)
- uses (calls/refs, reference-scoped): [`_type_name_and_range`](../../../tree_sitter_analyzer/languages/_c_type_definition_helpers.md#_type_name_and_range)  (7 test-only)

### `TestTypedefTypeName`
- def: [`tests/unit/languages/_test_c_traversal_type_helpers.py:241`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L241)
- signature: `class TestTypedefTypeName:`
- members:
  - `test_no_parent(self)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L261)
  - `test_non_typedef_parent(self)` — [`L255`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L255)
  - `test_typedef_parent(self)` — [`L242`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L242)
- uses (calls/refs, reference-scoped): [`_typedef_type_name`](../../../tree_sitter_analyzer/languages/_c_type_definition_helpers.md#_typedef_type_name)  (5 test-only)

## Functions
- `_get_node_text(node: Any)` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/languages/_test_c_traversal_type_helpers.py#L43)

