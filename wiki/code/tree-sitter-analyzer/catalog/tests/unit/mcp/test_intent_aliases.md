---
title: 'Module: tests/unit/mcp/test_intent_aliases.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/test_intent_aliases.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.test_intent_aliases`/Test
symbols:
  TestIntentAliasResolution.test_resolve_locate_usage_to_search_content: IntentAliasResolution#test_resolve_locate_usage_to_search_content().
  TestIntentAliasResolution.test_resolve_map_structure_to_list_files: IntentAliasResolution#test_resolve_map_structure_to_list_files().
  TestIntentAliasResolution.test_resolve_find_impacted_code_to_find_and_grep: IntentAliasResolution#test_resolve_find_impacted_code_to_find_and_grep().
  TestIntentAliasResolution.test_resolve_extract_structure_to_analyze_code_structure: IntentAliasResolution#test_resolve_extract_structure_to_analyze_code_structure().
  TestIntentAliasResolution.test_resolve_navigate_structure_to_get_code_outline: IntentAliasResolution#test_resolve_navigate_structure_to_get_code_outline().
  TestIntentAliasResolution.test_resolve_discover_files_to_list_files: IntentAliasResolution#test_resolve_discover_files_to_list_files().
  TestIntentAliasResolution.test_resolve_find_usage_to_search_content: IntentAliasResolution#test_resolve_find_usage_to_search_content().
  TestBackwardCompatibility.test_original_tool_name_returns_itself: BackwardCompatibility#test_original_tool_name_returns_itself().
  TestBackwardCompatibility.test_all_original_tool_names_pass_through: BackwardCompatibility#test_all_original_tool_names_pass_through().
  TestInvalidAliases.test_unknown_alias_raises_error: InvalidAliases#test_unknown_alias_raises_error().
  TestInvalidAliases.test_empty_alias_raises_error: InvalidAliases#test_empty_alias_raises_error().
  TestInvalidAliases.test_none_alias_raises_error: InvalidAliases#test_none_alias_raises_error().
  TestCaseSensitivity.test_alias_is_case_sensitive: CaseSensitivity#test_alias_is_case_sensitive().
  TestCaseSensitivity.test_original_tool_name_is_case_sensitive: CaseSensitivity#test_original_tool_name_is_case_sensitive().
  TestAliasMetadata.test_get_all_aliases_returns_dict: AliasMetadata#test_get_all_aliases_returns_dict().
  TestAliasMetadata.test_is_valid_alias_for_known_alias: AliasMetadata#test_is_valid_alias_for_known_alias().
  TestAliasMetadata.test_is_valid_alias_for_original_tool: AliasMetadata#test_is_valid_alias_for_original_tool().
  TestAliasMetadata.test_is_valid_alias_for_unknown_name: AliasMetadata#test_is_valid_alias_for_unknown_name().
  TestHelperFunction.test_get_tool_name_from_alias_with_alias: HelperFunction#test_get_tool_name_from_alias_with_alias().
  TestHelperFunction.test_get_tool_name_from_alias_with_original: HelperFunction#test_get_tool_name_from_alias_with_original().
  TestHelperFunction.test_get_tool_name_from_alias_with_invalid: HelperFunction#test_get_tool_name_from_alias_with_invalid().
  TestIntentAliasResolution: IntentAliasResolution#
  TestBackwardCompatibility: BackwardCompatibility#
  TestInvalidAliases: InvalidAliases#
  TestCaseSensitivity: CaseSensitivity#
  TestAliasMetadata: AliasMetadata#
  TestHelperFunction: HelperFunction#
---
# Module: [`tests/unit/mcp/test_intent_aliases.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py)

## Classes
### `TestAliasMetadata`
- def: [`tests/unit/mcp/test_intent_aliases.py:165`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L165)
- doc: 测试 Alias 元数据和查询功能
- signature: `class TestAliasMetadata:`
- members:
  - `test_get_all_aliases_returns_dict(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L168) — get_all_aliases 应该返回完整的 alias 映射
  - `test_is_valid_alias_for_known_alias(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L177) — is_valid_alias 对已知 alias 返回 True
  - `test_is_valid_alias_for_original_tool(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L182) — is_valid_alias 对原始工具名返回 True
  - `test_is_valid_alias_for_unknown_name(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L187) — is_valid_alias 对未知名称返回 False
- uses (calls/refs, reference-scoped): [`is_valid_alias`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#is_valid_alias), [`get_all_aliases`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#get_all_aliases)

### `TestBackwardCompatibility`
- def: [`tests/unit/mcp/test_intent_aliases.py:87`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L87)
- doc: 测试向后兼容性 - 原始工具名仍然有效
- signature: `class TestBackwardCompatibility:`
- members:
  - `test_all_original_tool_names_pass_through(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L98) — 所有原始工具名都应该 pass through
  - `test_original_tool_name_returns_itself(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L90) — 原始工具名应该返回自己（不变）
- uses (calls/refs, reference-scoped): [`resolve`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver.resolve), [`IntentAliasResolver`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver)

### `TestCaseSensitivity`
- def: [`tests/unit/mcp/test_intent_aliases.py:139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L139)
- doc: 测试大小写敏感性
- signature: `class TestCaseSensitivity:`
- members:
  - `test_alias_is_case_sensitive(self)` — [`L142`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L142) — Alias 应该区分大小写
  - `test_original_tool_name_is_case_sensitive(self)` — [`L153`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L153) — 原始工具名应该区分大小写
- uses (calls/refs, reference-scoped): [`resolve`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver.resolve), [`IntentAliasResolver`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver)

### `TestHelperFunction`
- def: [`tests/unit/mcp/test_intent_aliases.py:193`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L193)
- doc: 测试辅助函数 get_tool_name_from_alias
- signature: `class TestHelperFunction:`
- members:
  - `test_get_tool_name_from_alias_with_alias(self)` — [`L196`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L196) — get_tool_name_from_alias 应该解析 alias
  - `test_get_tool_name_from_alias_with_invalid(self)` — [`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L208) — get_tool_name_from_alias 对无效名称抛出错误
  - `test_get_tool_name_from_alias_with_original(self)` — [`L202`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L202) — get_tool_name_from_alias 对原始名称返回自身
- uses (calls/refs, reference-scoped): [`get_tool_name_from_alias`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#get_tool_name_from_alias)

### `TestIntentAliasResolution`
- def: [`tests/unit/mcp/test_intent_aliases.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L27)
- doc: 测试 Intent Alias 解析逻辑
- signature: `class TestIntentAliasResolution:`
- members:
  - `test_resolve_discover_files_to_list_files(self)` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L70) — discover_files 应该解析为 list_files (multiple aliases)
  - `test_resolve_extract_structure_to_analyze_code_structure(self)` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L54) — extract_structure 应该解析为 analyze_code_structure
  - `test_resolve_find_impacted_code_to_find_and_grep(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L46) — find_impacted_code 应该解析为 find_and_grep
  - `test_resolve_find_usage_to_search_content(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L78) — find_usage 应该解析为 search_content (multiple aliases)
  - `test_resolve_locate_usage_to_search_content(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L30) — locate_usage 应该解析为 search_content
  - `test_resolve_map_structure_to_list_files(self)` — [`L38`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L38) — map_structure 应该解析为 list_files
  - `test_resolve_navigate_structure_to_get_code_outline(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L62) — navigate_structure 应该解析为 get_code_outline
- uses (calls/refs, reference-scoped): [`resolve`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver.resolve), [`IntentAliasResolver`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver)

### `TestInvalidAliases`
- def: [`tests/unit/mcp/test_intent_aliases.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L114)
- doc: 测试无效 alias 处理
- signature: `class TestInvalidAliases:`
- members:
  - `test_empty_alias_raises_error(self)` — [`L124`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L124) — 空字符串应该抛出 ValueError
  - `test_none_alias_raises_error(self)` — [`L131`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L131) — None 应该抛出 TypeError
  - `test_unknown_alias_raises_error(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/test_intent_aliases.py#L117) — 未知的 alias 应该抛出 ValueError
- uses (calls/refs, reference-scoped): [`resolve`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver.resolve), [`IntentAliasResolver`](../../../tree_sitter_analyzer/mcp/intent_aliases.md#IntentAliasResolver)

