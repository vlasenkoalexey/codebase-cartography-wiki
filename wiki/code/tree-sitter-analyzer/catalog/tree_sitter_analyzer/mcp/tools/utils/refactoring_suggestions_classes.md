---
title: 'Module: tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.utils.refactoring_suggestions_classes`/
symbols:
  find_class_extractions: find_class_extractions().
  find_prefix_group_extractions: find_prefix_group_extractions().
  build_extract_class_recipe: build_extract_class_recipe().
  group_methods_by_responsibility: group_methods_by_responsibility().
  build_class_split_recipe: build_class_split_recipe().
  _target_module_name: _target_module_name().
  _target_owner_name: _target_owner_name().
  _responsibility_key: _responsibility_key().
  _GENERIC_METHOD_VERBS: _GENERIC_METHOD_VERBS.
  _primary_group: _primary_group().
  _import_update_instruction: _import_update_instruction().
  _pascal_case: _pascal_case().
  _snake_case: _snake_case().
---
# Module: [`tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py)

## Functions
- `_import_update_instruction(class_name: str, target_owner: str, target_module: str)` — [`L241`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L241) — Return a concise import/composition update instruction.
- `_pascal_case(value: str)` — [`L257`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L257)
- `_primary_group(method_names: list[str], responsibility_groups: list[dict[str, Any]])` — [`L191`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L191) — Return the best method group to move first.
- `_responsibility_key(method_name: str)` — [`L203`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L203) — Infer a stable responsibility key from a method name.
- `_snake_case(value: str)` — [`L261`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L261)
- `_target_module_name(class_name: str, responsibility: str, file_path: str | None)` — [`L227`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L227) — Suggest a sibling module or owner name for extracted responsibility.
- `_target_owner_name(class_name: str, responsibility: str)` — [`L216`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L216) — Suggest the class/mixin that should own extracted methods.
- `build_class_split_recipe(cls: dict[str, Any], responsibility_groups: list[dict[str, Any]], file_path: str | None)` — [`L139`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L139) — Build an agent-friendly recipe for splitting a large class.
- `build_extract_class_recipe(cls: dict[str, Any], responsibility: str, methods: list[str], file_path: str | None)` — [`L162`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L162) — Build a concrete extraction recipe for one responsibility group.
- `find_class_extractions(classes: list[dict[str, Any]], large_class_rule: dict[str, Any], prefix_group_rule: dict[str, Any], file_path: str | None = None)` — [`L43`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L43) — Find extractable class-level patterns.
- `find_prefix_group_extractions(cls: dict[str, Any], extraction_rule: dict[str, Any], responsibility_groups: list[dict[str, Any]] | None = None, file_path: str | None = None)` — [`L79`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L79) — Find method groups sharing a common prefix for class extraction.
- `group_methods_by_responsibility(method_names: list[str])` — [`L115`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L115) — Group method names by likely responsibility for extraction recipes.

## Module values
- `_GENERIC_METHOD_VERBS` — [`L10`](../../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/utils/refactoring_suggestions_classes.py#L10)

