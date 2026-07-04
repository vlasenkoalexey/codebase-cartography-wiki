---
title: 'Module: tests/unit/core/test_models_new_elements.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_models_new_elements.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_models_new_elements`/Test
symbols:
  TestComprehensionModel.test_comprehension_creation_minimal: ComprehensionModel#test_comprehension_creation_minimal().
  TestNewElementsIntegration.test_all_new_types_have_element_type_field: NewElementsIntegration#test_all_new_types_have_element_type_field().
  TestComprehensionModel.test_comprehension_list_type: ComprehensionModel#test_comprehension_list_type().
  TestComprehensionModel.test_comprehension_with_condition: ComprehensionModel#test_comprehension_with_condition().
  TestComprehensionModel.test_comprehension_set_type: ComprehensionModel#test_comprehension_set_type().
  TestComprehensionModel.test_comprehension_dict_type: ComprehensionModel#test_comprehension_dict_type().
  TestComprehensionModel.test_comprehension_generator_type: ComprehensionModel#test_comprehension_generator_type().
  TestComprehensionModel.test_comprehension_serialization: ComprehensionModel#test_comprehension_serialization().
  TestLambdaModel.test_lambda_creation_minimal: LambdaModel#test_lambda_creation_minimal().
  TestExpressionModel.test_expression_creation_minimal: ExpressionModel#test_expression_creation_minimal().
  TestLambdaModel.test_lambda_creation_with_parameters: LambdaModel#test_lambda_creation_with_parameters().
  TestLambdaModel.test_lambda_serialization: LambdaModel#test_lambda_serialization().
  TestLambdaModel.test_lambda_with_empty_parameters: LambdaModel#test_lambda_with_empty_parameters().
  TestExpressionModel.test_expression_conditional: ExpressionModel#test_expression_conditional().
  TestExpressionModel.test_expression_subscript: ExpressionModel#test_expression_subscript().
  TestExpressionModel.test_expression_list_literal: ExpressionModel#test_expression_list_literal().
  TestExpressionModel.test_expression_serialization: ExpressionModel#test_expression_serialization().
  TestExpressionModel.test_expression_long_preview: ExpressionModel#test_expression_long_preview().
  TestNewElementsIntegration.test_all_new_types_have_position_tracking: NewElementsIntegration#test_all_new_types_have_position_tracking().
  TestLambdaModel: LambdaModel#
  TestComprehensionModel: ComprehensionModel#
  TestExpressionModel: ExpressionModel#
  TestNewElementsIntegration: NewElementsIntegration#
---
# Module: [`tests/unit/core/test_models_new_elements.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py)

## Classes
### `TestComprehensionModel`
- def: [`tests/unit/core/test_models_new_elements.py:80`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L80)
- doc: Tests for Comprehension dataclass
- signature: `class TestComprehensionModel:`
- members:
  - `test_comprehension_creation_minimal(self)` — [`L83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L83) — Test creating Comprehension with minimal fields
  - `test_comprehension_dict_type(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L144) — Test dict comprehension
  - `test_comprehension_generator_type(self)` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L159) — Test generator expression
  - `test_comprehension_list_type(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L98) — Test list comprehension
  - `test_comprehension_serialization(self)` — [`L173`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L173) — Test Comprehension can be serialized to dict
  - `test_comprehension_set_type(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L129) — Test set comprehension
  - `test_comprehension_with_condition(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L115) — Test comprehension with condition
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`Comprehension`](../../../tree_sitter_analyzer/models/base.md#Comprehension), [`comprehension_type`](../../../tree_sitter_analyzer/models/base.md#Comprehension.comprehension_type), [`target_variable`](../../../tree_sitter_analyzer/models/base.md#Comprehension.target_variable), [`has_condition`](../../../tree_sitter_analyzer/models/base.md#Comprehension.has_condition), [`iterable_preview`](../../../tree_sitter_analyzer/models/base.md#Comprehension.iterable_preview), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Comprehension.element_type)

### `TestExpressionModel`
- def: [`tests/unit/core/test_models_new_elements.py:195`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L195)
- doc: Tests for Expression dataclass
- signature: `class TestExpressionModel:`
- members:
  - `test_expression_conditional(self)` — [`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L211) — Test conditional expression
  - `test_expression_creation_minimal(self)` — [`L198`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L198) — Test creating Expression with minimal fields
  - `test_expression_list_literal(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L237) — Test list literal expression
  - `test_expression_long_preview(self)` — [`L267`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L267) — Test Expression with long preview text
  - `test_expression_serialization(self)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L250) — Test Expression can be serialized to dict
  - `test_expression_subscript(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L224) — Test subscript expression
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`Expression`](../../../tree_sitter_analyzer/models/base.md#Expression), [`expression_kind`](../../../tree_sitter_analyzer/models/base.md#Expression.expression_kind), [`preview`](../../../tree_sitter_analyzer/models/base.md#Expression.preview), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Expression.element_type)

### `TestLambdaModel`
- def: [`tests/unit/core/test_models_new_elements.py:18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L18)
- doc: Tests for Lambda dataclass
- signature: `class TestLambdaModel:`
- members:
  - `test_lambda_creation_minimal(self)` — [`L21`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L21) — Test creating Lambda with minimal fields
  - `test_lambda_creation_with_parameters(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L34) — Test creating Lambda with parameters
  - `test_lambda_serialization(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L47) — Test Lambda can be serialized to dict
  - `test_lambda_with_empty_parameters(self)` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L66) — Test Lambda with empty parameter list
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`Lambda`](../../../tree_sitter_analyzer/models/base.md#Lambda), [`body_preview`](../../../tree_sitter_analyzer/models/base.md#Lambda.body_preview), [`parameters`](../../../tree_sitter_analyzer/models/base.md#Lambda.parameters), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Lambda.element_type)

### `TestNewElementsIntegration`
- def: [`tests/unit/core/test_models_new_elements.py:282`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L282)
- doc: Integration tests for new element types
- signature: `class TestNewElementsIntegration:`
- members:
  - `test_all_new_types_have_element_type_field(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L285) — Test all new types have element_type field
  - `test_all_new_types_have_position_tracking(self)` — [`L307`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_models_new_elements.py#L307) — Test all new types track position correctly
- uses (calls/refs, reference-scoped): [`name`](../../../tree_sitter_analyzer/models/base.md#CodeElement.name), [`start_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.start_line), [`end_line`](../../../tree_sitter_analyzer/models/base.md#CodeElement.end_line), [`Expression`](../../../tree_sitter_analyzer/models/base.md#Expression), [`Comprehension`](../../../tree_sitter_analyzer/models/base.md#Comprehension), [`Lambda`](../../../tree_sitter_analyzer/models/base.md#Lambda), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Comprehension.element_type), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Expression.element_type), [`element_type`](../../../tree_sitter_analyzer/models/base.md#Lambda.element_type)

