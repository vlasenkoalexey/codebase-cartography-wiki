---
title: 'Module: tests/unit/test_pr_url.py'
type: catalog
provenance: extracted
module: tests/unit/test_pr_url.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_pr_url`/Test
symbols:
  TestParsedPRUrl.test_slug: ParsedPRUrl#test_slug().
  TestParsedPRUrl.test_url: ParsedPRUrl#test_url().
  TestParsePRUrl.test_standard_https_url: ParsePRUrl#test_standard_https_url().
  TestParsePRUrl.test_http_url: ParsePRUrl#test_http_url().
  TestParsePRUrl.test_api_url: ParsePRUrl#test_api_url().
  TestParsedPRUrl.test_frozen: ParsedPRUrl#test_frozen().
  TestParsePRUrl.test_url_with_trailing_files: ParsePRUrl#test_url_with_trailing_files().
  TestParsePRUrl.test_url_with_trailing_slash: ParsePRUrl#test_url_with_trailing_slash().
  TestParsePRUrl.test_url_with_whitespace: ParsePRUrl#test_url_with_whitespace().
  TestFetchPRChangedFiles.test_success: FetchPRChangedFiles#test_success().
  TestFetchPRChangedFiles.test_failure_returns_empty: FetchPRChangedFiles#test_failure_returns_empty().
  TestFetchPRChangedFiles.test_empty_output: FetchPRChangedFiles#test_empty_output().
  TestFetchPRDiffStat.test_success: FetchPRDiffStat#test_success().
  TestFetchPRDiffStat.test_failure_returns_empty: FetchPRDiffStat#test_failure_returns_empty().
  TestFetchPRDiff.test_success: FetchPRDiff#test_success().
  TestFetchPRDiff.test_failure_returns_empty: FetchPRDiff#test_failure_returns_empty().
  TestChangeImpactToolPRUrlValidation.test_validate_accepts_pr_mode: ChangeImpactToolPRUrlValidation#test_validate_accepts_pr_mode().
  TestChangeImpactToolPRUrlValidation.test_validate_rejects_bad_mode: ChangeImpactToolPRUrlValidation#test_validate_rejects_bad_mode().
  TestChangeImpactToolPRUrlExecute.test_pr_url_analysis_returns_pr_metadata: ChangeImpactToolPRUrlExecute#test_pr_url_analysis_returns_pr_metadata().
  TestChangeImpactToolPRUrlExecute.test_pr_url_with_scope_filters_files: ChangeImpactToolPRUrlExecute#test_pr_url_with_scope_filters_files().
  TestChangeImpactToolPRUrlExecute.test_pr_url_invalid_url: ChangeImpactToolPRUrlExecute#test_pr_url_invalid_url().
  TestChangeImpactToolPRUrlExecute.test_pr_url_gh_not_available: ChangeImpactToolPRUrlExecute#test_pr_url_gh_not_available().
  TestChangeImpactToolPRUrlExecute.test_pr_url_no_changes: ChangeImpactToolPRUrlExecute#test_pr_url_no_changes().
  TestChangeImpactToolPRUrlExecute.test_pr_url_agent_summary_only: ChangeImpactToolPRUrlExecute#test_pr_url_agent_summary_only().
  TestParsePRUrl.test_invalid_url_returns_none: ParsePRUrl#test_invalid_url_returns_none().
  TestParsePRUrl.test_issue_url_not_matched: ParsePRUrl#test_issue_url_not_matched().
  TestCheckGhAvailable.test_available: CheckGhAvailable#test_available().
  TestCheckGhAvailable.test_not_available: CheckGhAvailable#test_not_available().
  TestToolSchemaIncludesPRUrl.test_schema_has_pr_url: ToolSchemaIncludesPRUrl#test_schema_has_pr_url().
  TestToolSchemaIncludesPRUrl.test_schema_mode_includes_pr: ToolSchemaIncludesPRUrl#test_schema_mode_includes_pr().
  TestChangeImpactToolPRUrlExecute.test_pr_url_auto_mode_override: ChangeImpactToolPRUrlExecute#test_pr_url_auto_mode_override().
  TestParsePRUrl: ParsePRUrl#
  TestParsedPRUrl: ParsedPRUrl#
  TestFetchPRChangedFiles: FetchPRChangedFiles#
  TestFetchPRDiffStat: FetchPRDiffStat#
  TestFetchPRDiff: FetchPRDiff#
  TestCheckGhAvailable: CheckGhAvailable#
  TestToolSchemaIncludesPRUrl: ToolSchemaIncludesPRUrl#
  TestChangeImpactToolPRUrlValidation: ChangeImpactToolPRUrlValidation#
  TestChangeImpactToolPRUrlExecute: ChangeImpactToolPRUrlExecute#
---
# Module: [`tests/unit/test_pr_url.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py)

## Classes
### `TestChangeImpactToolPRUrlExecute`
- def: [`tests/unit/test_pr_url.py:178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L178)
- signature: `class TestChangeImpactToolPRUrlExecute:`
- members:
  - `test_pr_url_agent_summary_only(self, mock_files, mock_stat, mock_gh, tmp_path)` — [`L287`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L287)
  - `test_pr_url_analysis_returns_pr_metadata(self, mock_files, mock_stat, mock_gh, tmp_path)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L185)
  - `test_pr_url_auto_mode_override(self)` — [`L304`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L304)
  - `test_pr_url_gh_not_available(self, mock_gh, tmp_path)` — [`L244`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L244)
  - `test_pr_url_invalid_url(self, tmp_path)` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L227)
  - `test_pr_url_no_changes(self, mock_files, mock_gh, tmp_path)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L265)
  - `test_pr_url_with_scope_filters_files(self, mock_files, mock_stat, mock_gh, tmp_path)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L210)
- uses (calls/refs, reference-scoped): [`execute`](../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool.execute), [`ChangeImpactTool`](../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool), [`parse_pr_url`](../../tree_sitter_analyzer/pr_url.md#parse_pr_url)

### `TestChangeImpactToolPRUrlValidation`
- def: [`tests/unit/test_pr_url.py:157`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L157)
- signature: `class TestChangeImpactToolPRUrlValidation:`
- members:
  - `test_validate_accepts_pr_mode(self, tmp_path)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L158)
  - `test_validate_rejects_bad_mode(self, tmp_path)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L167)
- uses (calls/refs, reference-scoped): [`ChangeImpactTool`](../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#ChangeImpactTool.validate_arguments)

### `TestCheckGhAvailable`
- def: [`tests/unit/test_pr_url.py:137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L137)
- signature: `class TestCheckGhAvailable:`
- members:
  - `test_available(self, mock_gh)` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L139)
  - `test_not_available(self, mock_gh)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L144)
- uses (calls/refs, reference-scoped): [`check_gh_available`](../../tree_sitter_analyzer/pr_url.md#check_gh_available)

### `TestFetchPRChangedFiles`
- def: [`tests/unit/test_pr_url.py:87`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L87)
- signature: `class TestFetchPRChangedFiles:`
- members:
  - `test_empty_output(self, mock_gh)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L105)
  - `test_failure_returns_empty(self, mock_gh)` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L99)
  - `test_success(self, mock_gh)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L89)
- uses (calls/refs, reference-scoped): [`ParsedPRUrl`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl), [`fetch_pr_changed_files`](../../tree_sitter_analyzer/pr_url.md#fetch_pr_changed_files)

### `TestFetchPRDiff`
- def: [`tests/unit/test_pr_url.py:124`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L124)
- signature: `class TestFetchPRDiff:`
- members:
  - `test_failure_returns_empty(self, mock_gh)` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L132)
  - `test_success(self, mock_gh)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L126)
- uses (calls/refs, reference-scoped): [`ParsedPRUrl`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl), [`fetch_pr_diff`](../../tree_sitter_analyzer/pr_url.md#fetch_pr_diff)

### `TestFetchPRDiffStat`
- def: [`tests/unit/test_pr_url.py:111`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L111)
- signature: `class TestFetchPRDiffStat:`
- members:
  - `test_failure_returns_empty(self, mock_gh)` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L119)
  - `test_success(self, mock_gh)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L113)
- uses (calls/refs, reference-scoped): [`ParsedPRUrl`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl), [`fetch_pr_diff_stat`](../../tree_sitter_analyzer/pr_url.md#fetch_pr_diff_stat)

### `TestParsePRUrl`
- def: [`tests/unit/test_pr_url.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L24)
- signature: `class TestParsePRUrl:`
- members:
  - `test_api_url(self)` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L49)
  - `test_http_url(self)` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L32)
  - `test_invalid_url_returns_none(self)` — [`L63`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L63)
  - `test_issue_url_not_matched(self)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L68)
  - `test_standard_https_url(self)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L25)
  - `test_url_with_trailing_files(self)` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L39)
  - `test_url_with_trailing_slash(self)` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L44)
  - `test_url_with_whitespace(self)` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L58)
- uses (calls/refs, reference-scoped): [`parse_pr_url`](../../tree_sitter_analyzer/pr_url.md#parse_pr_url), [`pr_number`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.pr_number), [`owner`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.owner), [`repo`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.repo)

### `TestParsedPRUrl`
- def: [`tests/unit/test_pr_url.py:72`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L72)
- signature: `class TestParsedPRUrl:`
- members:
  - `test_frozen(self)` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L81)
  - `test_slug(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L73)
  - `test_url(self)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L77)
- uses (calls/refs, reference-scoped): [`ParsedPRUrl`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl), [`pr_number`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.pr_number), [`owner`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.owner), [`repo`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.repo), [`slug`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.slug), [`url`](../../tree_sitter_analyzer/pr_url.md#ParsedPRUrl.url)

### `TestToolSchemaIncludesPRUrl`
- def: [`tests/unit/test_pr_url.py:149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L149)
- signature: `class TestToolSchemaIncludesPRUrl:`
- members:
  - `test_schema_has_pr_url(self)` — [`L150`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L150)
  - `test_schema_mode_includes_pr(self)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_pr_url.py#L153)
- uses (calls/refs, reference-scoped): [`TOOL_SCHEMA`](../../tree_sitter_analyzer/mcp/tools/change_impact_tool.md#TOOL_SCHEMA.TOOL_SCHEMA)

