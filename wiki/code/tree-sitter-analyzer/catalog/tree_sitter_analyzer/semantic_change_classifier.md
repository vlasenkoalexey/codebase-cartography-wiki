---
title: 'Module: tree_sitter_analyzer/semantic_change_classifier.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/semantic_change_classifier.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.semantic_change_classifier`/
symbols:
  _classify_single_hunk: _classify_single_hunk().
  SemanticCategory: SemanticCategory#
  SemanticChangeClassifier.classify: SemanticChangeClassifier#classify().
  ClassifiedHunk.category: ClassifiedHunk#category.
  _CATEGORY_LABELS._CATEGORY_LABELS: _CATEGORY_LABELS._CATEGORY_LABELS.
  _RISK_LEVELS._RISK_LEVELS: _RISK_LEVELS._RISK_LEVELS.
  _PRIORITY_ORDER: _PRIORITY_ORDER.
  ClassifiedHunk.confidence: ClassifiedHunk#confidence.
  ClassifiedHunk: ClassifiedHunk#
  ClassifiedHunk.reason: ClassifiedHunk#reason.
  ClassifiedHunk.hunk: ClassifiedHunk#hunk.
  SemanticClassification.to_dict: SemanticClassification#to_dict().
  ClassifiedHunk.to_dict: ClassifiedHunk#to_dict().
  SemanticChangeClassifier: SemanticChangeClassifier#
  _compute_risk: _compute_risk().
  SemanticCategory.API_CHANGE: SemanticCategory#API_CHANGE.
  SemanticCategory.INTERNAL_CHANGE: SemanticCategory#INTERNAL_CHANGE.
  SemanticClassification.dominant_category: SemanticClassification#dominant_category.
  _hunk_name: _hunk_name().
  _pick_dominant: _pick_dominant().
  _is_test_path: _is_test_path().
  SemanticCategory.REFACTOR: SemanticCategory#REFACTOR.
  _build_summary: _build_summary().
  SemanticCategory.UNKNOWN: SemanticCategory#UNKNOWN.
  _hunk_preview: _hunk_preview().
  SemanticClassification.classifications: SemanticClassification#classifications.
  SemanticCategory.FEATURE_ADDITION: SemanticCategory#FEATURE_ADDITION.
  SemanticCategory.FEATURE_REMOVAL: SemanticCategory#FEATURE_REMOVAL.
  _is_doc_path: _is_doc_path().
  SemanticClassification.risk_level: SemanticClassification#risk_level.
  _is_public_name: _is_public_name().
  SemanticCategory.TEST_CHANGE: SemanticCategory#TEST_CHANGE.
  SemanticClassification.change_summary: SemanticClassification#change_summary.
  SemanticCategory.IMPORT_CHANGE: SemanticCategory#IMPORT_CHANGE.
  SemanticCategory.DOCUMENTATION: SemanticCategory#DOCUMENTATION.
  SemanticClassification: SemanticClassification#
  SemanticClassification.category_counts: SemanticClassification#category_counts.
  SemanticCategory.STYLE_CHANGE: SemanticCategory#STYLE_CHANGE.
  _has_public_indicator: _has_public_indicator().
  SemanticCategory.CONFIGURATION: SemanticCategory#CONFIGURATION.
  _PUBLIC_NAME_INDICATORS: _PUBLIC_NAME_INDICATORS.
  _TEST_PATH_INDICATORS: _TEST_PATH_INDICATORS.
  _DOC_EXTENSIONS: _DOC_EXTENSIONS.
  SemanticChangeClassifier._file_path: SemanticChangeClassifier#_file_path.
  SemanticChangeClassifier.__init__: SemanticChangeClassifier#__init__().
---
# Module: [`tree_sitter_analyzer/semantic_change_classifier.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py)

## Classes
### `ClassifiedHunk`
- def: [`tree_sitter_analyzer/semantic_change_classifier.py:105`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L105)
- signature: `class ClassifiedHunk:`
- members:
  - `to_dict(self, include_children: bool = False)` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L111)
  - `category` — [`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L107)
  - `confidence` — [`L108`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L108)
  - `hunk` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L106)
  - `reason` — [`L109`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L109)
- uses (calls/refs, reference-scoped): [`SemanticCategory`](semantic_change_classifier.md#SemanticCategory), [`_CATEGORY_LABELS`](semantic_change_classifier.md#_CATEGORY_LABELS._CATEGORY_LABELS), [`_RISK_LEVELS`](semantic_change_classifier.md#_RISK_LEVELS._RISK_LEVELS), [`ASTDiffHunk`](ast_diff.md#ASTDiffHunk), [`to_dict`](ast_diff.md#ASTDiffHunk.to_dict)
- used by: [`execute`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`_classify_single_hunk`](semantic_change_classifier.md#_classify_single_hunk), [`classify`](semantic_change_classifier.md#SemanticChangeClassifier.classify), [`to_dict`](semantic_change_classifier.md#SemanticClassification.to_dict), [`_compute_risk`](semantic_change_classifier.md#_compute_risk), [`classifications`](semantic_change_classifier.md#SemanticClassification.classifications)  (20 test-only)

### `SemanticCategory`  ·  implements/extends Enum, str
- def: [`tree_sitter_analyzer/semantic_change_classifier.py:26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L26)
- signature: `class SemanticCategory(str, Enum):`
- members:
  - `API_CHANGE` — [`L27`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L27)
  - `CONFIGURATION` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L33)
  - `DOCUMENTATION` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L36)
  - `FEATURE_ADDITION` — [`L29`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L29)
  - `FEATURE_REMOVAL` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L30)
  - `IMPORT_CHANGE` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L32)
  - `INTERNAL_CHANGE` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L31)
  - `REFACTOR` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L28)
  - `STYLE_CHANGE` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L34)
  - `TEST_CHANGE` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L35)
  - `UNKNOWN` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L37)
- used by: [`_classify_single_hunk`](semantic_change_classifier.md#_classify_single_hunk), [`classify`](semantic_change_classifier.md#SemanticChangeClassifier.classify), [`category`](semantic_change_classifier.md#ClassifiedHunk.category), [`_CATEGORY_LABELS`](semantic_change_classifier.md#_CATEGORY_LABELS._CATEGORY_LABELS), [`_RISK_LEVELS`](semantic_change_classifier.md#_RISK_LEVELS._RISK_LEVELS), [`_PRIORITY_ORDER`](semantic_change_classifier.md#_PRIORITY_ORDER), [`dominant_category`](semantic_change_classifier.md#SemanticClassification.dominant_category), [`_pick_dominant`](semantic_change_classifier.md#_pick_dominant), [`_build_summary`](semantic_change_classifier.md#_build_summary)  (32 test-only)

### `SemanticChangeClassifier`
- def: [`tree_sitter_analyzer/semantic_change_classifier.py:385`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L385)
- doc: Classify AST diff results into semantic categories.
- signature: `class SemanticChangeClassifier:`
- members:
  - `classify(self, diff_result: ASTDiffResult)` — [`L402`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L402)
- protocol/private: `__init__`[`L399`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L399), `_file_path`[`L400`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L400)
- uses (calls/refs, reference-scoped): [`_classify_single_hunk`](semantic_change_classifier.md#_classify_single_hunk), [`SemanticCategory`](semantic_change_classifier.md#SemanticCategory), [`category`](semantic_change_classifier.md#ClassifiedHunk.category), [`ClassifiedHunk`](semantic_change_classifier.md#ClassifiedHunk), [`_compute_risk`](semantic_change_classifier.md#_compute_risk), [`hunks`](ast_diff.md#ASTDiffResult.hunks), [`ASTDiffResult`](ast_diff.md#ASTDiffResult), [`dominant_category`](semantic_change_classifier.md#SemanticClassification.dominant_category), [`_pick_dominant`](semantic_change_classifier.md#_pick_dominant), [`_build_summary`](semantic_change_classifier.md#_build_summary), [`UNKNOWN`](semantic_change_classifier.md#SemanticCategory.UNKNOWN), [`classifications`](semantic_change_classifier.md#SemanticClassification.classifications), [`new_file`](ast_diff.md#ASTDiffResult.new_file), [`risk_level`](semantic_change_classifier.md#SemanticClassification.risk_level), [`change_summary`](semantic_change_classifier.md#SemanticClassification.change_summary), [`SemanticClassification`](semantic_change_classifier.md#SemanticClassification), [`category_counts`](semantic_change_classifier.md#SemanticClassification.category_counts)
- used by: [`execute`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`execute`](mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.execute), [`_classify_changed_files`](mcp/tools/utils/change_impact_analysis.md#_classify_changed_files)  (8 test-only)

### `SemanticClassification`
- def: [`tree_sitter_analyzer/semantic_change_classifier.py:123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L123)
- signature: `class SemanticClassification:`
- members:
  - `to_dict(self, include_children: bool = False)` — [`L130`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L130)
  - `category_counts` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L128)
  - `change_summary` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L127)
  - `classifications` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L124)
  - `dominant_category` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L125)
  - `risk_level` — [`L126`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L126)
- uses (calls/refs, reference-scoped): [`SemanticCategory`](semantic_change_classifier.md#SemanticCategory), [`_CATEGORY_LABELS`](semantic_change_classifier.md#_CATEGORY_LABELS._CATEGORY_LABELS), [`ClassifiedHunk`](semantic_change_classifier.md#ClassifiedHunk), [`to_dict`](semantic_change_classifier.md#ClassifiedHunk.to_dict), [`UNKNOWN`](semantic_change_classifier.md#SemanticCategory.UNKNOWN)
- used by: [`execute`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`classify`](semantic_change_classifier.md#SemanticChangeClassifier.classify), [`execute`](mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.execute), [`_classify_changed_files`](mcp/tools/utils/change_impact_analysis.md#_classify_changed_files)  (9 test-only)

## Functions
- `_build_summary(dominant: SemanticCategory, counts: dict[SemanticCategory, int], total: int)` — [`L368`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L368)
- `_classify_single_hunk(hunk: ASTDiffHunk, file_path: str | None = None)` — [`L172`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L172) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- `_compute_risk(classifications: list[ClassifiedHunk])` — [`L348`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L348)
- `_has_public_indicator(text: str | None)` — [`L166`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L166)
- `_hunk_name(hunk: ASTDiffHunk)` — [`L310`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L310)
- `_hunk_preview(hunk: ASTDiffHunk)` — [`L318`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L318)
- `_is_doc_path(file_path: str | None)` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L151)
- `_is_public_name(name: str | None)` — [`L158`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L158)
- `_is_test_path(file_path: str | None)` — [`L144`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L144)
- `_pick_dominant(counts: dict[SemanticCategory, int])` — [`L341`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L341)

## Module values
- `_CATEGORY_LABELS` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L40)
- `_DOC_EXTENSIONS` — [`L94`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L94)
- `_PRIORITY_ORDER` — [`L326`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L326)
- `_PUBLIC_NAME_INDICATORS` — [`L68`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L68)
- `_RISK_LEVELS` — [`L54`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L54)
- `_TEST_PATH_INDICATORS` — [`L78`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/semantic_change_classifier.py#L78)

