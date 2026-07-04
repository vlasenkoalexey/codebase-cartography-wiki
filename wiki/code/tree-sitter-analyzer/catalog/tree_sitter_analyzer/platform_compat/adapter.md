---
title: 'Module: tree_sitter_analyzer/platform_compat/adapter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/platform_compat/adapter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.platform_compat.adapter`/
symbols:
  RecoverViewsFromErrorsRule.generate_elements: RecoverViewsFromErrorsRule#generate_elements().
  CompatibilityAdapter._load_rules: CompatibilityAdapter#_load_rules().
  RemovePhantomTriggersRule.apply: RemovePhantomTriggersRule#apply().
  CompatibilityAdapter: CompatibilityAdapter#
  FixFunctionNameKeywordsRule.apply: FixFunctionNameKeywordsRule#apply().
  FixTriggerNameDescriptionRule.apply: FixTriggerNameDescriptionRule#apply().
  CompatibilityAdapter.adapt_elements: CompatibilityAdapter#adapt_elements().
  CompatibilityAdapter.rules: CompatibilityAdapter#rules.
  RemovePhantomFunctionsRule.apply: RemovePhantomFunctionsRule#apply().
  AdaptationRule.apply: AdaptationRule#apply().
  FixFunctionNameKeywordsRule: FixFunctionNameKeywordsRule#
  FixTriggerNameDescriptionRule: FixTriggerNameDescriptionRule#
  RemovePhantomTriggersRule: RemovePhantomTriggersRule#
  RecoverViewsFromErrorsRule: RecoverViewsFromErrorsRule#
  T: T.
  CompatibilityAdapter.__init__: CompatibilityAdapter#__init__().
  RecoverViewsFromErrorsRule.apply: RecoverViewsFromErrorsRule#apply().
  AdaptationRule: AdaptationRule#
  CompatibilityAdapter.profile: CompatibilityAdapter#profile.
  logger: logger.
  RemovePhantomFunctionsRule: RemovePhantomFunctionsRule#
  AdaptationRule.rule_id: AdaptationRule#rule_id().
  AdaptationRule.description: AdaptationRule#description().
  FixFunctionNameKeywordsRule.rule_id: FixFunctionNameKeywordsRule#rule_id().
  FixFunctionNameKeywordsRule.description: FixFunctionNameKeywordsRule#description().
  FixTriggerNameDescriptionRule.rule_id: FixTriggerNameDescriptionRule#rule_id().
  FixTriggerNameDescriptionRule.description: FixTriggerNameDescriptionRule#description().
  RemovePhantomTriggersRule.rule_id: RemovePhantomTriggersRule#rule_id().
  RemovePhantomTriggersRule.description: RemovePhantomTriggersRule#description().
  RemovePhantomFunctionsRule.rule_id: RemovePhantomFunctionsRule#rule_id().
  RemovePhantomFunctionsRule.description: RemovePhantomFunctionsRule#description().
  RecoverViewsFromErrorsRule.rule_id: RecoverViewsFromErrorsRule#rule_id().
  RecoverViewsFromErrorsRule.description: RecoverViewsFromErrorsRule#description().
---
# Module: [`tree_sitter_analyzer/platform_compat/adapter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py)

## Classes
### `AdaptationRule`  ·  implements/extends Protocol
- def: [`tree_sitter_analyzer/platform_compat/adapter.py:19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L19)
- doc: Rule for adapting platform-specific behavior.
- signature: `class AdaptationRule(Protocol):`
- members:
  - `apply(self, element: SQLElement, context: dict)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L32) — Applies the rule to an element.
  - `description(self)` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L28) — Description of what the rule does.
  - `rule_id(self)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L23) — Unique identifier for the rule.
- uses (calls/refs, reference-scoped): [`SQLElement`](../models/sql_models.md#SQLElement)
- used by: [`_load_rules`](adapter.md#CompatibilityAdapter._load_rules), [`adapt_elements`](adapter.md#CompatibilityAdapter.adapt_elements), [`rules`](adapter.md#CompatibilityAdapter.rules)

### `CompatibilityAdapter`
- def: [`tree_sitter_analyzer/platform_compat/adapter.py:47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L47)
- doc: Applies platform-specific adaptations to SQL parsing results.
- signature: `class CompatibilityAdapter:`
- members:
  - `_load_rules(self)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L55) — Loads adaptation rules based on the profile.
  - `adapt_elements(self, elements: list[SQLElement], source_code: str)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L81) — Main entry point for adapting elements.
  - `profile` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L51)
  - `rules` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L52)
- protocol/private: `__init__`[`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L50)
- uses (calls/refs, reference-scoped): [`SQLElement`](../models/sql_models.md#SQLElement), [`BehaviorProfile`](profiles.md#BehaviorProfile), [`adaptation_rules`](profiles.md#BehaviorProfile.adaptation_rules), [`apply`](adapter.md#AdaptationRule.apply), [`FixFunctionNameKeywordsRule`](adapter.md#FixFunctionNameKeywordsRule), [`FixTriggerNameDescriptionRule`](adapter.md#FixTriggerNameDescriptionRule), [`RecoverViewsFromErrorsRule`](adapter.md#RecoverViewsFromErrorsRule), [`RemovePhantomTriggersRule`](adapter.md#RemovePhantomTriggersRule), [`AdaptationRule`](adapter.md#AdaptationRule), [`RemovePhantomFunctionsRule`](adapter.md#RemovePhantomFunctionsRule)
- used by: [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/plugin.md#TREE_SITTER_AVAILABLE), [`_adapt_sql_elements`](../languages/sql_plugin/extractor.md#SQLElementExtractor._adapt_sql_elements), [`adapter`](../languages/sql_plugin/plugin.md#SQLPlugin.adapter), [`set_adapter`](../languages/sql_plugin/extractor.md#SQLElementExtractor.set_adapter), [`adapter`](../languages/sql_plugin/extractor.md#SQLElementExtractor.adapter)  (4 test-only)

### `FixFunctionNameKeywordsRule`
- def: [`tree_sitter_analyzer/platform_compat/adapter.py:133`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L133)
- members:
  - `apply(self, element: SQLElement, context: dict)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L147)
  - `description(self)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L144)
  - `rule_id(self)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L140)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`raw_text`](../models/base.md#CodeElement.raw_text), [`SQLElement`](../models/sql_models.md#SQLElement), [`SQLFunction`](../models/sql_models.md#SQLFunction)
- used by: [`_load_rules`](adapter.md#CompatibilityAdapter._load_rules)  (1 test-only)

### `FixTriggerNameDescriptionRule`
- def: [`tree_sitter_analyzer/platform_compat/adapter.py:189`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L189)
- members:
  - `apply(self, element: SQLElement, context: dict)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L203)
  - `description(self)` — [`L200`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L200)
  - `rule_id(self)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L196)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`raw_text`](../models/base.md#CodeElement.raw_text), [`SQLElement`](../models/sql_models.md#SQLElement), [`SQLTrigger`](../models/sql_models.md#SQLTrigger)
- used by: [`_load_rules`](adapter.md#CompatibilityAdapter._load_rules)  (1 test-only)

### `RecoverViewsFromErrorsRule`
- def: [`tree_sitter_analyzer/platform_compat/adapter.py:271`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L271)
- members:
  - `apply(self, element: SQLElement, context: dict)` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L285)
  - `description(self)` — [`L282`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L282)
  - `generate_elements(self, context: dict)` — [`L289`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L289) — documented in [tree_sitter_analyzer-models-sql_models](../../../concepts/tree_sitter_analyzer-models-sql_models.md)
  - `rule_id(self)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L278)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`raw_text`](../models/base.md#CodeElement.raw_text), [`SQLElementType`](../models/sql_models.md#SQLElementType), [`SQLElement`](../models/sql_models.md#SQLElement), [`SQLView`](../models/sql_models.md#SQLView), [`VIEW`](../models/sql_models.md#SQLElementType.VIEW), [`sql_element_type`](../models/sql_models.md#SQLView.sql_element_type), [`element_type`](../models/sql_models.md#SQLView.element_type)
- used by: [`_load_rules`](adapter.md#CompatibilityAdapter._load_rules)  (1 test-only)

### `RemovePhantomFunctionsRule`
- def: [`tree_sitter_analyzer/platform_compat/adapter.py:246`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L246)
- members:
  - `apply(self, element: SQLElement, context: dict)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L260)
  - `description(self)` — [`L257`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L257)
  - `rule_id(self)` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L253)
- uses (calls/refs, reference-scoped): [`raw_text`](../models/base.md#CodeElement.raw_text), [`SQLElement`](../models/sql_models.md#SQLElement), [`SQLFunction`](../models/sql_models.md#SQLFunction)
- used by: [`_load_rules`](adapter.md#CompatibilityAdapter._load_rules)

### `RemovePhantomTriggersRule`
- def: [`tree_sitter_analyzer/platform_compat/adapter.py:218`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L218)
- members:
  - `apply(self, element: SQLElement, context: dict)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L232)
  - `description(self)` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L229)
  - `rule_id(self)` — [`L225`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L225)
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`raw_text`](../models/base.md#CodeElement.raw_text), [`SQLElement`](../models/sql_models.md#SQLElement), [`SQLTrigger`](../models/sql_models.md#SQLTrigger), [`logger`](adapter.md#logger)
- used by: [`_load_rules`](adapter.md#CompatibilityAdapter._load_rules)  (1 test-only)

## Module values
- `T` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L16)
- `logger` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/platform_compat/adapter.py#L14)

