---
title: 'Module: tree_sitter_analyzer/core/analysis_session.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/core/analysis_session.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.core.analysis_session`/
symbols:
  AnalysisSession: AnalysisSession#
  AnalysisSession.to_dict: AnalysisSession#to_dict().
  AnalysisSession.token_savings_pct: AnalysisSession#token_savings_pct().
  AnalysisSession.save_to_audit_log: AnalysisSession#save_to_audit_log().
  AnalysisSession.git_commit: AnalysisSession#git_commit.
  AnalysisSession.file_hashes: AnalysisSession#file_hashes.
  AnalysisSession.token_count_before: AnalysisSession#token_count_before.
  AnalysisSession.session_id: AnalysisSession#session_id.
  AnalysisSession._detect_git_commit: AnalysisSession#_detect_git_commit().
  AnalysisSession.timestamp: AnalysisSession#timestamp.
  AnalysisSession.token_count_after: AnalysisSession#token_count_after.
  _git_commit_cache._git_commit_cache: _git_commit_cache._git_commit_cache.
  AnalysisSession.tools_used: AnalysisSession#tools_used.
  AnalysisSession._resolve_git_commit: AnalysisSession#_resolve_git_commit().
  AnalysisSession._calculate_file_hashes: AnalysisSession#_calculate_file_hashes().
  AnalysisSession._hash_one_file: AnalysisSession#_hash_one_file().
  AnalysisSession.input_files: AnalysisSession#input_files.
  AnalysisSession.output_format: AnalysisSession#output_format.
  _file_hash_cache._file_hash_cache: _file_hash_cache._file_hash_cache.
  AnalysisSession.__init__: AnalysisSession#__init__().
  _GIT_CACHE_TTL: _GIT_CACHE_TTL.
  AnalysisSession.DEFAULT_RETENTION_DAYS: AnalysisSession#DEFAULT_RETENTION_DAYS.
  AnalysisSession._validate_session_inputs: AnalysisSession#_validate_session_inputs().
  AnalysisSession._make_session_id: AnalysisSession#_make_session_id().
---
# Module: [`tree_sitter_analyzer/core/analysis_session.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py)

## Classes
### `AnalysisSession`
- def: [`tree_sitter_analyzer/core/analysis_session.py:34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L34)
- doc: 记录和管理 TSA 分析会话
- signature: `class AnalysisSession:`
- members:
  - `__init__(self, input_files: list[str], output_format: str, git_commit: str | None = None, tools_used: list[str] | None = None, token_count_before: int | None = None, token_count_after: int | None = None, auto_detect_git_commit: bool = False)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L49) — 初始化 Analysis Session
  - `_calculate_file_hashes(self, file_paths: list[str])` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L166) — 计算文件的 SHA256 hash（带 mtime 缓存）
  - `_detect_git_commit(self)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L216) — 自动检测当前 git commit（带5秒缓存，避免同一工作流重复 subprocess 调用）
  - `_hash_one_file(file_path: str)` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L188) — Return SHA256 digest of ``file_path``, using the mtime cache.
  - `_make_session_id()` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L121) — Return ``(session_id, iso_timestamp)`` — UTC-stamped with UUID4 suffix.
  - `_resolve_git_commit(self, git_commit: str | None, auto_detect: bool)` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L134) — Pick the git commit string: explicit arg > auto-detect > None.
  - `_validate_session_inputs(input_files: list[str], output_format: str, token_count_before: int | None, token_count_after: int | None)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L98) — Reject empty input list / unknown format / negative token counts.
  - `save_to_audit_log(self)` — [`L272`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L272) — 保存 session 到审计日志
  - `to_dict(self)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L252) — 转换为字典格式（用于 JSON 序列化）
  - `token_savings_pct(self)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L145) — 计算 token 节省百分比
  - `DEFAULT_RETENTION_DAYS` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L47)
  - `file_hashes` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L92)
  - `git_commit` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L93)
  - `input_files` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L86)
  - `output_format` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L87)
  - `session_id` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L83)
  - `timestamp` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L83)
  - `token_count_after` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L90)
  - `token_count_before` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L89)
  - `tools_used` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L88)
- uses (calls/refs, reference-scoped): [`_git_commit_cache`](analysis_session.md#_git_commit_cache._git_commit_cache), [`_file_hash_cache`](analysis_session.md#_file_hash_cache._file_hash_cache), [`_GIT_CACHE_TTL`](analysis_session.md#_GIT_CACHE_TTL)
- used by: (28 test-only callers)

## Module values
- `_GIT_CACHE_TTL` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L27)
- `_file_hash_cache` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L31)
- `_git_commit_cache` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/core/analysis_session.py#L26)

