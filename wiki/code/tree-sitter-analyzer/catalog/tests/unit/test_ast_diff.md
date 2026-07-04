---
title: 'Module: tests/unit/test_ast_diff.py'
type: catalog
provenance: extracted
module: tests/unit/test_ast_diff.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_ast_diff`/
symbols:
  TestExtractSignature.test_basic: TestExtractSignature#test_basic().
  TestMatchNodes.test_match_by_name: TestMatchNodes#test_match_by_name().
  TestMatchNodes.test_no_match: TestMatchNodes#test_no_match().
  TestComputeStats.test_mixed: TestComputeStats#test_mixed().
  TestDiffStrings.test_added_function: TestDiffStrings#test_added_function().
  TestClassifyNode.test_function_types: TestClassifyNode#test_function_types().
  TestClassifyNode.test_class_types: TestClassifyNode#test_class_types().
  TestClassifyNode.test_import_types: TestClassifyNode#test_import_types().
  TestClassifyNode.test_other: TestClassifyNode#test_other().
  TestDiffStrings.test_changed_body: TestDiffStrings#test_changed_body().
  differ: differ().
  TestTextHash.test_deterministic: TestTextHash#test_deterministic().
  TestTextHash.test_different: TestTextHash#test_different().
  TestComputeStats.test_empty: TestComputeStats#test_empty().
  TestClassifyNode: TestClassifyNode#
  TestTextHash: TestTextHash#
  TestComputeStats: TestComputeStats#
  TestMatchNodes: TestMatchNodes#
  TestDiffStrings: TestDiffStrings#
  TestDiffStrings.test_identical_code: TestDiffStrings#test_identical_code().
  TestDiffStrings.test_removed_function: TestDiffStrings#test_removed_function().
  TestDiffStrings.test_changed_signature: TestDiffStrings#test_changed_signature().
  TestDiffStrings.test_added_class: TestDiffStrings#test_added_class().
  TestDiffStrings.test_javascript_diff: TestDiffStrings#test_javascript_diff().
  TestDiffStrings.test_import_added: TestDiffStrings#test_import_added().
  TestDiffStrings.test_both_parse_fail: TestDiffStrings#test_both_parse_fail().
  TestDiffStrings.test_to_dict_roundtrip: TestDiffStrings#test_to_dict_roundtrip().
  TestDiffFiles: TestDiffFiles#
  TestDiffFiles.test_diff_same_file: TestDiffFiles#test_diff_same_file().
  TestDiffFiles.test_diff_changed_file: TestDiffFiles#test_diff_changed_file().
  TestDiffFiles.test_diff_unsupported_language: TestDiffFiles#test_diff_unsupported_language().
  TestDiffFiles.test_diff_nonexistent_file: TestDiffFiles#test_diff_nonexistent_file().
  TestDiffStringPairs: TestDiffStringPairs#
  TestDiffStringPairs.test_batch_diff: TestDiffStringPairs#test_batch_diff().
  TestExtractSignature: TestExtractSignature#
---
# Module: [`tests/unit/test_ast_diff.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py)

## Classes
### `TestClassifyNode`
- def: [`tests/unit/test_ast_diff.py:23`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L23)
- signature: `class TestClassifyNode:`
- members:
  - `test_class_types(self)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L29)
  - `test_function_types(self)` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L24)
  - `test_import_types(self)` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L33)
  - `test_other(self)` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L37)
- uses (calls/refs, reference-scoped): [`ASTNodeKind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind), [`_classify_node`](../../tree_sitter_analyzer/ast_diff.md#_classify_node), [`FUNCTION`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.FUNCTION), [`CLASS`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.CLASS), [`IMPORT`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.IMPORT), [`OTHER`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.OTHER)

### `TestComputeStats`
- def: [`tests/unit/test_ast_diff.py:50`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L50)
- signature: `class TestComputeStats:`
- members:
  - `test_empty(self)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L51)
  - `test_mixed(self)` — [`L62`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L62)
- uses (calls/refs, reference-scoped): [`ASTNodeKind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind), [`DiffKind`](../../tree_sitter_analyzer/ast_diff.md#DiffKind), [`FUNCTION`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.FUNCTION), [`ASTDiffHunk`](../../tree_sitter_analyzer/ast_diff.md#ASTDiffHunk), [`NODE_ADDED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_ADDED), [`BODY_CHANGED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.BODY_CHANGED), [`_compute_stats`](../../tree_sitter_analyzer/ast_diff.md#_compute_stats), [`CLASS`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.CLASS), [`NODE_REMOVED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_REMOVED)

### `TestDiffFiles`
- def: [`tests/unit/test_ast_diff.py:216`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L216)
- signature: `class TestDiffFiles:`
- members:
  - `test_diff_changed_file(self, differ, tmp_path)` — [`L224`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L224)
  - `test_diff_nonexistent_file(self, differ, tmp_path)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L240)
  - `test_diff_same_file(self, differ, tmp_path)` — [`L217`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L217)
  - `test_diff_unsupported_language(self, differ, tmp_path)` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L232)

### `TestDiffStringPairs`
- def: [`tests/unit/test_ast_diff.py:247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L247)
- signature: `class TestDiffStringPairs:`
- members:
  - `test_batch_diff(self, differ)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L248)

### `TestDiffStrings`
- def: [`tests/unit/test_ast_diff.py:145`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L145)
- signature: `class TestDiffStrings:`
- members:
  - `test_added_class(self, differ)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L181)
  - `test_added_function(self, differ)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L151)
  - `test_both_parse_fail(self, differ)` — [`L199`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L199)
  - `test_changed_body(self, differ)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L167)
  - `test_changed_signature(self, differ)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L175)
  - `test_identical_code(self, differ)` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L146)
  - `test_import_added(self, differ)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L193)
  - `test_javascript_diff(self, differ)` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L187)
  - `test_removed_function(self, differ)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L161)
  - `test_to_dict_roundtrip(self, differ)` — [`L203`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L203)
- uses (calls/refs, reference-scoped): [`ASTNodeKind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind), [`DiffKind`](../../tree_sitter_analyzer/ast_diff.md#DiffKind), [`FUNCTION`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.FUNCTION), [`NODE_ADDED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.NODE_ADDED), [`BODY_CHANGED`](../../tree_sitter_analyzer/ast_diff.md#DiffKind.BODY_CHANGED)

### `TestExtractSignature`
- def: [`tests/unit/test_ast_diff.py:258`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L258)
- signature: `class TestExtractSignature:`
- members:
  - `test_basic(self)` — [`L259`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L259)
- uses (calls/refs, reference-scoped): [`ASTNodeKind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind), [`kind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.kind), [`name`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.name), [`ASTNodeInfo`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo), [`FUNCTION`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.FUNCTION), [`_extract_signature`](../../tree_sitter_analyzer/ast_diff.md#_extract_signature), [`children`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.children), [`text_hash`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.text_hash), [`text_preview`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.text_preview), [`node_type`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.node_type), [`end_line`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.end_line), [`start_line`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.start_line), [`end_col`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.end_col), [`start_col`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.start_col), [`PARAMETER`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.PARAMETER)

### `TestMatchNodes`
- def: [`tests/unit/test_ast_diff.py:75`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L75)
- signature: `class TestMatchNodes:`
- members:
  - `test_match_by_name(self)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L76)
  - `test_no_match(self)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L110)
- uses (calls/refs, reference-scoped): [`ASTNodeKind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind), [`kind`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.kind), [`name`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.name), [`ASTNodeInfo`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo), [`FUNCTION`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeKind.FUNCTION), [`_match_nodes`](../../tree_sitter_analyzer/ast_diff.md#_match_nodes), [`text_hash`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.text_hash), [`text_preview`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.text_preview), [`node_type`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.node_type), [`end_line`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.end_line), [`start_line`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.start_line), [`end_col`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.end_col), [`start_col`](../../tree_sitter_analyzer/ast_diff.md#ASTNodeInfo.start_col)

### `TestTextHash`
- def: [`tests/unit/test_ast_diff.py:42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L42)
- signature: `class TestTextHash:`
- members:
  - `test_deterministic(self)` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L43)
  - `test_different(self)` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L46)
- uses (calls/refs, reference-scoped): [`_text_hash`](../../tree_sitter_analyzer/ast_diff.md#_text_hash)

## Functions
- `differ()` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_ast_diff.py#L19)

