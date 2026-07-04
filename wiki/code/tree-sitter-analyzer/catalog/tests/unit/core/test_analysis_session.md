---
title: 'Module: tests/unit/core/test_analysis_session.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_analysis_session.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_analysis_session`/Test
symbols:
  TestAnalysisSessionCreation.test_session_creation_with_minimal_params: AnalysisSessionCreation#test_session_creation_with_minimal_params().
  TestAnalysisSessionCreation.test_session_with_all_optional_params: AnalysisSessionCreation#test_session_with_all_optional_params().
  TestAnalysisSessionCreation.test_token_savings_when_counts_not_provided: AnalysisSessionCreation#test_token_savings_when_counts_not_provided().
  TestSessionPersistence.test_save_writes_json_to_correct_path: SessionPersistence#test_save_writes_json_to_correct_path().
  TestSessionMetadataFields.test_multiple_input_files_preserved: SessionMetadataFields#test_multiple_input_files_preserved().
  TestAnalysisSessionCreation.test_session_id_format_timestamp_plus_uuid: AnalysisSessionCreation#test_session_id_format_timestamp_plus_uuid().
  TestAnalysisSessionCreation.test_session_id_uniqueness_with_rapid_creation: AnalysisSessionCreation#test_session_id_uniqueness_with_rapid_creation().
  TestAnalysisSessionCreation.test_token_savings_calculation: AnalysisSessionCreation#test_token_savings_calculation().
  TestFileHashCalculation.test_file_hash_calculation_sha256: FileHashCalculation#test_file_hash_calculation_sha256().
  TestFileHashCalculation.test_file_hash_missing_file: FileHashCalculation#test_file_hash_missing_file().
  TestFileHashCalculation.test_multiple_files_hash_calculation: FileHashCalculation#test_multiple_files_hash_calculation().
  TestSessionSerialization.test_to_dict_includes_all_fields: SessionSerialization#test_to_dict_includes_all_fields().
  TestSessionSerialization.test_to_dict_serializable_to_json: SessionSerialization#test_to_dict_serializable_to_json().
  TestSessionPersistence.test_save_creates_session_directory_if_not_exists: SessionPersistence#test_save_creates_session_directory_if_not_exists().
  TestSessionPersistence.test_save_skips_mkdir_if_directory_exists: SessionPersistence#test_save_skips_mkdir_if_directory_exists().
  TestSessionPersistence.test_save_writes_valid_json_content: SessionPersistence#test_save_writes_valid_json_content().
  TestSessionValidation.test_valid_output_formats: SessionValidation#test_valid_output_formats().
  TestSessionValidation.test_token_count_after_greater_than_before_warning: SessionValidation#test_token_count_after_greater_than_before_warning().
  TestGitIntegration.test_auto_detect_git_commit: GitIntegration#test_auto_detect_git_commit().
  TestGitIntegration.test_auto_detect_git_commit_not_in_repo: GitIntegration#test_auto_detect_git_commit_not_in_repo().
  TestGitIntegration.test_manual_git_commit_overrides_auto_detect: GitIntegration#test_manual_git_commit_overrides_auto_detect().
  TestSessionRetention.test_default_retention_90_days: SessionRetention#test_default_retention_90_days().
  TestSessionMetadataFields.test_timestamp_format_iso8601: SessionMetadataFields#test_timestamp_format_iso8601().
  TestSessionMetadataFields.test_tools_used_preserves_order: SessionMetadataFields#test_tools_used_preserves_order().
  TestFileHashCalculation.setup_method: FileHashCalculation#setup_method().
  TestSessionValidation.test_empty_input_files_raises_error: SessionValidation#test_empty_input_files_raises_error().
  TestSessionValidation.test_invalid_output_format_raises_error: SessionValidation#test_invalid_output_format_raises_error().
  TestSessionValidation.test_negative_token_count_raises_error: SessionValidation#test_negative_token_count_raises_error().
  TestGitIntegration.setup_method: GitIntegration#setup_method().
  TestSessionRetention.test_custom_retention_from_env_var: SessionRetention#test_custom_retention_from_env_var().
  TestAnalysisSessionCreation: AnalysisSessionCreation#
  TestFileHashCalculation: FileHashCalculation#
  TestSessionSerialization: SessionSerialization#
  TestSessionPersistence: SessionPersistence#
  TestSessionValidation: SessionValidation#
  TestGitIntegration: GitIntegration#
  TestSessionRetention: SessionRetention#
  TestSessionMetadataFields: SessionMetadataFields#
---
# Module: [`tests/unit/core/test_analysis_session.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py)

## Classes
### `TestAnalysisSessionCreation`
- def: [`tests/unit/core/test_analysis_session.py:27`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L27)
- doc: 测试 AnalysisSession 创建和基本属性
- signature: `class TestAnalysisSessionCreation:`
- members:
  - `test_session_creation_with_minimal_params(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L30) — 创建最小参数的 session
  - `test_session_id_format_timestamp_plus_uuid(self)` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L44) — Session ID 格式应为 timestamp-uuid4（防止同一秒内冲突）
  - `test_session_id_uniqueness_with_rapid_creation(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L63) — 快速连续创建 session，ID 应该唯一（uuid4 保证）
  - `test_session_with_all_optional_params(self)` — [`L73`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L73) — 创建包含所有可选参数的 session
  - `test_token_savings_calculation(self)` — [`L90`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L90) — Token 节省百分比计算正确
  - `test_token_savings_when_counts_not_provided(self)` — [`L102`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L102) — Token counts 未提供时，savings_pct 应为 None
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`token_savings_pct`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.token_savings_pct), [`git_commit`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.git_commit), [`token_count_before`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.token_count_before), [`session_id`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.session_id), [`timestamp`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.timestamp), [`token_count_after`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.token_count_after), [`tools_used`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.tools_used), [`input_files`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.input_files), [`output_format`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.output_format)

### `TestFileHashCalculation`
- def: [`tests/unit/core/test_analysis_session.py:114`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L114)
- doc: 测试文件 SHA256 hash 计算
- signature: `class TestFileHashCalculation:`
- members:
  - `setup_method(self)` — [`L117`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L117) — 每个测试前清除文件哈希缓存，避免测试间干扰
  - `test_file_hash_calculation_sha256(self, mock_exists, mock_file, mock_stat)` — [`L125`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L125) — 计算文件 SHA256 hash
  - `test_file_hash_missing_file(self, mock_exists)` — [`L137`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L137) — 文件不存在时，hash 应为 None
  - `test_multiple_files_hash_calculation(self, mock_exists, mock_file, mock_stat)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L149) — 多个文件的 hash 计算
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`file_hashes`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.file_hashes), [`_file_hash_cache`](../../../tree_sitter_analyzer/core/analysis_session.md#_file_hash_cache._file_hash_cache)

### `TestGitIntegration`
- def: [`tests/unit/core/test_analysis_session.py:338`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L338)
- doc: 测试 Git commit 记录功能
- signature: `class TestGitIntegration:`
- members:
  - `setup_method(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L341) — 每个测试前清除 git commit 缓存，避免测试间干扰
  - `test_auto_detect_git_commit(self, mock_run)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L347) — 自动检测当前 git commit
  - `test_auto_detect_git_commit_not_in_repo(self, mock_run)` — [`L364`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L364) — 不在 git repo 中时，git_commit 应为 None
  - `test_manual_git_commit_overrides_auto_detect(self)` — [`L379`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L379) — 手动提供的 git_commit 优先于自动检测
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`git_commit`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.git_commit), [`_git_commit_cache`](../../../tree_sitter_analyzer/core/analysis_session.md#_git_commit_cache._git_commit_cache)

### `TestSessionMetadataFields`
- def: [`tests/unit/core/test_analysis_session.py:420`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L420)
- doc: 测试 Session metadata 字段的正确性
- signature: `class TestSessionMetadataFields:`
- members:
  - `test_multiple_input_files_preserved(self)` — [`L446`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L446) — 多个 input files 应该完整保存
  - `test_timestamp_format_iso8601(self)` — [`L423`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L423) — Timestamp 应为 ISO 8601 格式
  - `test_tools_used_preserves_order(self)` — [`L435`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L435) — tools_used 应保持调用顺序
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`file_hashes`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.file_hashes), [`timestamp`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.timestamp), [`tools_used`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.tools_used), [`input_files`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.input_files)

### `TestSessionPersistence`
- def: [`tests/unit/core/test_analysis_session.py:201`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L201)
- doc: 测试 Session 持久化到 \~/.tsa/sessions/
- signature: `class TestSessionPersistence:`
- members:
  - `test_save_creates_session_directory_if_not_exists(self, mock_file, mock_exists, mock_mkdir)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L207) — Session 目录不存在时自动创建（修复 P1 gap）
  - `test_save_skips_mkdir_if_directory_exists(self, mock_file, mock_exists, mock_mkdir)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L226) — Session 目录存在时不重复创建
  - `test_save_writes_json_to_correct_path(self, mock_exists, mock_file)` — [`L244`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L244) — 保存的 JSON 文件路径正确
  - `test_save_writes_valid_json_content(self, mock_exists, mock_file)` — [`L261`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L261) — 保存的 JSON 内容格式正确
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`save_to_audit_log`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.save_to_audit_log), [`session_id`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.session_id)

### `TestSessionRetention`
- def: [`tests/unit/core/test_analysis_session.py:399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L399)
- doc: 测试 Session 保留策略
- signature: `class TestSessionRetention:`
- members:
  - `test_custom_retention_from_env_var(self)` — [`L413`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L413) — 从环境变量读取自定义保留天数
  - `test_default_retention_90_days(self)` — [`L402`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L402) — 默认保留策略应为 90 天
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`DEFAULT_RETENTION_DAYS`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.DEFAULT_RETENTION_DAYS)

### `TestSessionSerialization`
- def: [`tests/unit/core/test_analysis_session.py:160`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L160)
- doc: 测试 Session 序列化到 JSON
- signature: `class TestSessionSerialization:`
- members:
  - `test_to_dict_includes_all_fields(self)` — [`L163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L163) — to_dict() 应包含所有字段
  - `test_to_dict_serializable_to_json(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L187) — to_dict() 返回的数据应该可以序列化为 JSON
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`to_dict`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.to_dict)

### `TestSessionValidation`
- def: [`tests/unit/core/test_analysis_session.py:285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L285)
- doc: 测试 Session 数据验证
- signature: `class TestSessionValidation:`
- members:
  - `test_empty_input_files_raises_error(self)` — [`L288`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L288) — input_files 为空应该抛出异常
  - `test_invalid_output_format_raises_error(self)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L296) — 无效的 output_format 应该抛出异常
  - `test_negative_token_count_raises_error(self)` — [`L315`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L315) — 负数 token count 应该抛出异常
  - `test_token_count_after_greater_than_before_warning(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L324) — token_count_after > before 应该警告（可能是统计错误）
  - `test_valid_output_formats(self)` — [`L304`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_analysis_session.py#L304) — 有效的 output_format 应该被接受
- uses (calls/refs, reference-scoped): [`AnalysisSession`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession), [`token_savings_pct`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.token_savings_pct), [`output_format`](../../../tree_sitter_analyzer/core/analysis_session.md#AnalysisSession.output_format)

