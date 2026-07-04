---
title: 'Module: tests/unit/test_semantic_change_classifier.py'
type: catalog
provenance: extracted
module: tests/unit/test_semantic_change_classifier.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_semantic_change_classifier`/
symbols:
  _hunk: _hunk().
  TestSemanticChangeClassifier.test_mixed_changes: TestSemanticChangeClassifier#test_mixed_changes().
  TestSemanticChangeClassifier.test_single_addition: TestSemanticChangeClassifier#test_single_addition().
  TestSemanticChangeClassifier.test_file_path_override: TestSemanticChangeClassifier#test_file_path_override().
  TestSemanticChangeClassifier.test_to_dict_roundtrip: TestSemanticChangeClassifier#test_to_dict_roundtrip().
  TestSemanticChangeClassifier.test_classified_hunk_to_dict: TestSemanticChangeClassifier#test_classified_hunk_to_dict().
  _node: _node().
  TestSemanticChangeClassifier.test_empty_diff: TestSemanticChangeClassifier#test_empty_diff().
  TestClassifySingleHunk.test_public_signature_change: TestClassifySingleHunk#test_public_signature_change().
  TestClassifySingleHunk.test_function_added: TestClassifySingleHunk#test_function_added().
  TestClassifySingleHunk.test_public_function_removed: TestClassifySingleHunk#test_public_function_removed().
  TestClassifySingleHunk.test_private_function_removed: TestClassifySingleHunk#test_private_function_removed().
  TestClassifySingleHunk.test_import_change: TestClassifySingleHunk#test_import_change().
  TestClassifySingleHunk.test_private_signature_change: TestClassifySingleHunk#test_private_signature_change().
  TestClassifySingleHunk.test_public_rename: TestClassifySingleHunk#test_public_rename().
  TestClassifySingleHunk.test_private_rename: TestClassifySingleHunk#test_private_rename().
  TestClassifySingleHunk.test_class_added: TestClassifySingleHunk#test_class_added().
  TestClassifySingleHunk.test_non_func_added: TestClassifySingleHunk#test_non_func_added().
  TestClassifySingleHunk.test_body_changed: TestClassifySingleHunk#test_body_changed().
  TestClassifySingleHunk.test_generic_changed: TestClassifySingleHunk#test_generic_changed().
  TestComputeRisk.test_high_risk: TestComputeRisk#test_high_risk().
  TestComputeRisk.test_medium_risk: TestComputeRisk#test_medium_risk().
  TestComputeRisk.test_low_risk: TestComputeRisk#test_low_risk().
  TestComputeRisk.test_low_confidence_high_ignored: TestComputeRisk#test_low_confidence_high_ignored().
  TestClassifySingleHunk.test_test_file: TestClassifySingleHunk#test_test_file().
  TestClassifySingleHunk.test_doc_file: TestClassifySingleHunk#test_doc_file().
  TestSemanticChangeClassifier.test_semantic_classification_to_dict: TestSemanticChangeClassifier#test_semantic_classification_to_dict().
  TestSemanticCategory.test_values: TestSemanticCategory#test_values().
  TestPickDominant.test_api_wins: TestPickDominant#test_api_wins().
  TestPickDominant.test_feature_removal_second: TestPickDominant#test_feature_removal_second().
  TestPickDominant.test_refactor_over_internal: TestPickDominant#test_refactor_over_internal().
  TestBuildSummary.test_with_changes: TestBuildSummary#test_with_changes().
  TestPickDominant.test_empty: TestPickDominant#test_empty().
  TestBuildSummary.test_empty: TestBuildSummary#test_empty().
  TestSemanticCategory.test_str_enum: TestSemanticCategory#test_str_enum().
  TestHelpers.test_is_test_path_positive: TestHelpers#test_is_test_path_positive().
  TestHelpers.test_is_test_path_negative: TestHelpers#test_is_test_path_negative().
  TestHelpers.test_is_doc_path_positive: TestHelpers#test_is_doc_path_positive().
  TestHelpers.test_is_doc_path_negative: TestHelpers#test_is_doc_path_negative().
  TestHelpers.test_is_public_name: TestHelpers#test_is_public_name().
  TestComputeRisk.test_empty: TestComputeRisk#test_empty().
  TestSemanticCategory: TestSemanticCategory#
  TestHelpers: TestHelpers#
  TestClassifySingleHunk: TestClassifySingleHunk#
  TestPickDominant: TestPickDominant#
  TestComputeRisk: TestComputeRisk#
  TestBuildSummary: TestBuildSummary#
  TestSemanticChangeClassifier: TestSemanticChangeClassifier#
---
# Module: [`tests/unit/test_semantic_change_classifier.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py)

## Classes
### `TestBuildSummary`
- def: [`tests/unit/test_semantic_change_classifier.py:239`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L239)
- signature: `class TestBuildSummary:`
- members:
  - `test_empty(self)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L240)
  - `test_with_changes(self)` — [`L243`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L243)
- uses (calls/refs, reference-scoped): [`SemanticCategory`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory), [`API_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.API_CHANGE), [`INTERNAL_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.INTERNAL_CHANGE), [`_build_summary`](../../tree_sitter_analyzer/semantic_change_classifier.md#_build_summary), [`UNKNOWN`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.UNKNOWN)

### `TestClassifySingleHunk`
- def: [`tests/unit/test_semantic_change_classifier.py:93`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L93)
- signature: `class TestClassifySingleHunk:`
- members:
  - `test_body_changed(self)` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L159)
  - `test_class_added(self)` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L137)
  - `test_doc_file(self)` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L100)
  - `test_function_added(self)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L131)
  - `test_generic_changed(self)` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L164)
  - `test_import_change(self)` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L105)
  - `test_non_func_added(self)` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L142)
  - `test_private_function_removed(self)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L153)
  - `test_private_rename(self)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L126)
  - `test_private_signature_change(self)` — [`L116`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L116)
  - `test_public_function_removed(self)` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L147)
  - `test_public_rename(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L121)
  - `test_public_signature_change(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L110)
  - `test_test_file(self)` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L94)
- uses (calls/refs, reference-scoped): [`_classify_single_hunk`](../../tree_sitter_analyzer/semantic_change_classifier.md#_classify_single_hunk), [`SemanticCategory`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory), [`ASTNodeKind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind), [`DiffKind`](../../tree_sitter_analyzer/ast_diff.md#DiffKind), [`category`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.category), [`FUNCTION`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.FUNCTION), [`confidence`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.confidence), [`reason`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.reason), [`API_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.API_CHANGE), [`INTERNAL_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.INTERNAL_CHANGE), [`NODE_ADDED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_ADDED), [`REFACTOR`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.REFACTOR), [`BODY_CHANGED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.BODY_CHANGED), [`FEATURE_ADDITION`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.FEATURE_ADDITION), [`FEATURE_REMOVAL`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.FEATURE_REMOVAL), [`CLASS`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.CLASS), [`NODE_CHANGED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_CHANGED), [`NODE_REMOVED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_REMOVED), [`SIGNATURE_CHANGED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.SIGNATURE_CHANGED), [`TEST_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.TEST_CHANGE), [`DOCUMENTATION`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.DOCUMENTATION), [`IMPORT`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.IMPORT), [`IMPORT_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.IMPORT_CHANGE), [`NODE_RENAMED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_RENAMED), [`VARIABLE`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.VARIABLE)  (1 test-only)

### `TestComputeRisk`
- def: [`tests/unit/test_semantic_change_classifier.py:190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L190)
- signature: `class TestComputeRisk:`
- members:
  - `test_empty(self)` — [`L191`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L191)
  - `test_high_risk(self)` — [`L194`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L194)
  - `test_low_confidence_high_ignored(self)` — [`L227`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L227)
  - `test_low_risk(self)` — [`L216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L216)
  - `test_medium_risk(self)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L205)
- uses (calls/refs, reference-scoped): [`SemanticCategory`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory), [`category`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.category), [`confidence`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.confidence), [`ClassifiedHunk`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk), [`reason`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.reason), [`hunk`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.hunk), [`_compute_risk`](../../tree_sitter_analyzer/semantic_change_classifier.md#_compute_risk), [`API_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.API_CHANGE), [`REFACTOR`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.REFACTOR), [`STYLE_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.STYLE_CHANGE)  (1 test-only)

### `TestHelpers`
- def: [`tests/unit/test_semantic_change_classifier.py:65`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L65)
- signature: `class TestHelpers:`
- members:
  - `test_is_doc_path_negative(self)` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L82)
  - `test_is_doc_path_positive(self)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L78)
  - `test_is_public_name(self)` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L86)
  - `test_is_test_path_negative(self)` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L73)
  - `test_is_test_path_positive(self)` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L66)
- uses (calls/refs, reference-scoped): [`_is_test_path`](../../tree_sitter_analyzer/semantic_change_classifier.md#_is_test_path), [`_is_doc_path`](../../tree_sitter_analyzer/semantic_change_classifier.md#_is_doc_path), [`_is_public_name`](../../tree_sitter_analyzer/semantic_change_classifier.md#_is_public_name)

### `TestPickDominant`
- def: [`tests/unit/test_semantic_change_classifier.py:170`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L170)
- signature: `class TestPickDominant:`
- members:
  - `test_api_wins(self)` — [`L174`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L174)
  - `test_empty(self)` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L171)
  - `test_feature_removal_second(self)` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L178)
  - `test_refactor_over_internal(self)` — [`L185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L185)
- uses (calls/refs, reference-scoped): [`SemanticCategory`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory), [`API_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.API_CHANGE), [`INTERNAL_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.INTERNAL_CHANGE), [`_pick_dominant`](../../tree_sitter_analyzer/semantic_change_classifier.md#_pick_dominant), [`REFACTOR`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.REFACTOR), [`UNKNOWN`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.UNKNOWN), [`FEATURE_REMOVAL`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.FEATURE_REMOVAL)

### `TestSemanticCategory`
- def: [`tests/unit/test_semantic_change_classifier.py:54`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L54)
- signature: `class TestSemanticCategory:`
- members:
  - `test_str_enum(self)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L61)
  - `test_values(self)` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L55)
- uses (calls/refs, reference-scoped): [`SemanticCategory`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory), [`API_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.API_CHANGE), [`REFACTOR`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.REFACTOR), [`UNKNOWN`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.UNKNOWN), [`FEATURE_ADDITION`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.FEATURE_ADDITION)

### `TestSemanticChangeClassifier`
- def: [`tests/unit/test_semantic_change_classifier.py:250`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L250)
- signature: `class TestSemanticChangeClassifier:`
- members:
  - `test_classified_hunk_to_dict(self)` — [`L335`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L335)
  - `test_empty_diff(self)` — [`L251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L251)
  - `test_file_path_override(self)` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L297)
  - `test_mixed_changes(self)` — [`L278`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L278)
  - `test_semantic_classification_to_dict(self)` — [`L350`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L350)
  - `test_single_addition(self)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L264)
  - `test_to_dict_roundtrip(self)` — [`L311`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L311)
- uses (calls/refs, reference-scoped): [`SemanticCategory`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory), [`ASTNodeKind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind), [`classify`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticChangeClassifier.classify), [`DiffKind`](../../tree_sitter_analyzer/ast_diff.md#DiffKind), [`category`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.category), [`FUNCTION`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.FUNCTION), [`confidence`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.confidence), [`ClassifiedHunk`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk), [`reason`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.reason), [`hunk`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.hunk), [`to_dict`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.to_dict), [`to_dict`](../../tree_sitter_analyzer/semantic_change_classifier.md#ClassifiedHunk.to_dict), [`SemanticChangeClassifier`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticChangeClassifier), [`API_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.API_CHANGE), [`hunks`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffResult.hunks), [`ASTDiffResult`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffResult), [`dominant_category`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.dominant_category), [`NODE_ADDED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_ADDED), [`REFACTOR`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.REFACTOR), [`UNKNOWN`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.UNKNOWN), [`classifications`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.classifications), [`new_file`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffResult.new_file), [`BODY_CHANGED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.BODY_CHANGED), [`FEATURE_ADDITION`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.FEATURE_ADDITION), [`language`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffResult.language), [`old_file`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffResult.old_file), [`risk_level`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.risk_level), [`SIGNATURE_CHANGED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.SIGNATURE_CHANGED), [`TEST_CHANGE`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticCategory.TEST_CHANGE), [`change_summary`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.change_summary), [`SemanticClassification`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification), [`category_counts`](../../tree_sitter_analyzer/semantic_change_classifier.md#SemanticClassification.category_counts)  (1 test-only)

## Functions
- `_hunk(diff_kind: DiffKind = DiffKind.NODE_ADDED, node_kind: ASTNodeKind = ASTNodeKind.FUNCTION, name: str = "func")` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L39)
- `_node(name: str = "func", kind: ASTNodeKind = ASTNodeKind.FUNCTION)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_semantic_change_classifier.py#L25)

