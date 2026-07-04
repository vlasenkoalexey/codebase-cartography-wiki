---
title: 'Module: tree_sitter_analyzer/ast_diff.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/ast_diff.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.ast_diff`/
symbols:
  ASTNodeKind: ASTNodeKind#
  ASTDiffer.diff_strings: ASTDiffer#diff_strings().
  _diff_matched_nodes: _diff_matched_nodes().
  _classify_node: _classify_node().
  DiffKind: DiffKind#
  ASTDiffer.diff_files: ASTDiffer#diff_files().
  _extract_node_info: _extract_node_info().
  _diff_children: _diff_children().
  ASTDiffer._diff_node_lists: ASTDiffer#_diff_node_lists().
  ASTNodeInfo.kind: ASTNodeInfo#kind.
  ASTNodeInfo.name: ASTNodeInfo#name.
  ASTNodeInfo: ASTNodeInfo#
  ASTNodeKind.FUNCTION: ASTNodeKind#FUNCTION.
  ASTDiffHunk: ASTDiffHunk#
  ASTDiffHunk.node_kind: ASTDiffHunk#node_kind.
  _extract_signature: _extract_signature().
  ASTNodeInfo.to_dict: ASTNodeInfo#to_dict().
  _match_nodes: _match_nodes().
  ASTDiffHunk.diff_kind: ASTDiffHunk#diff_kind.
  ASTDiffHunk.old_node: ASTDiffHunk#old_node.
  ASTDiffHunk.new_node: ASTDiffHunk#new_node.
  ASTDiffer: ASTDiffer#
  ASTDiffHunk.to_dict: ASTDiffHunk#to_dict().
  ASTNodeInfo.children: ASTNodeInfo#children.
  ASTDiffResult.to_dict: ASTDiffResult#to_dict().
  _get_body_hash: _get_body_hash().
  ASTNodeInfo.text_hash: ASTNodeInfo#text_hash.
  ASTDiffResult.hunks: ASTDiffResult#hunks.
  ASTNodeInfo.text_preview: ASTNodeInfo#text_preview.
  ASTDiffResult: ASTDiffResult#
  DiffKind.NODE_ADDED: DiffKind#NODE_ADDED.
  ASTNodeInfo.node_type: ASTNodeInfo#node_type.
  ASTDiffHunk.summary: ASTDiffHunk#summary.
  ASTDiffResult.new_file: ASTDiffResult#new_file.
  DiffKind.BODY_CHANGED: DiffKind#BODY_CHANGED.
  ASTNodeInfo.start_line: ASTNodeInfo#start_line.
  ASTNodeInfo.end_line: ASTNodeInfo#end_line.
  ASTDiffResult.old_file: ASTDiffResult#old_file.
  ASTDiffResult.language: ASTDiffResult#language.
  _compute_stats: _compute_stats().
  _child_name_overlap: _child_name_overlap().
  _body_hash_changed: _body_hash_changed().
  ASTNodeKind.CLASS: ASTNodeKind#CLASS.
  ASTNodeInfo.start_col: ASTNodeInfo#start_col.
  ASTNodeInfo.end_col: ASTNodeInfo#end_col.
  _extract_top_level_nodes: _extract_top_level_nodes().
  DiffKind.NODE_REMOVED: DiffKind#NODE_REMOVED.
  DiffKind.NODE_CHANGED: DiffKind#NODE_CHANGED.
  DiffKind.SIGNATURE_CHANGED: DiffKind#SIGNATURE_CHANGED.
  _text_hash: _text_hash().
  ASTNodeKind.IMPORT: ASTNodeKind#IMPORT.
  ASTNodeKind.OTHER: ASTNodeKind#OTHER.
  ASTDiffer.diff_string_pairs: ASTDiffer#diff_string_pairs().
  DiffKind.NODE_RENAMED: DiffKind#NODE_RENAMED.
  ASTDiffHunk.details: ASTDiffHunk#details.
  ASTNodeKind.METHOD: ASTNodeKind#METHOD.
  ASTNodeKind.VARIABLE: ASTNodeKind#VARIABLE.
  ASTNodeKind.PARAMETER: ASTNodeKind#PARAMETER.
  ASTDiffer.__init__: ASTDiffer#__init__().
  ASTNodeKind.DECORATOR: ASTNodeKind#DECORATOR.
  ASTNodeKind.BLOCK: ASTNodeKind#BLOCK.
  ASTDiffResult.summary_stats: ASTDiffResult#summary_stats.
  _sig_diff: _sig_diff().
  ASTDiffer._parser: ASTDiffer#_parser.
  _FUNCTION_NODES: _FUNCTION_NODES.
  _CLASS_NODES: _CLASS_NODES.
  _IMPORT_NODES: _IMPORT_NODES.
  _VARIABLE_NODES: _VARIABLE_NODES.
  _DECORATOR_NODES: _DECORATOR_NODES.
  _PARAM_NODES: _PARAM_NODES.
  _BLOCK_NODES: _BLOCK_NODES.
  _node_name: _node_name().
  _preview: _preview().
  logger: logger.
  DiffKind.NODE_MOVED: DiffKind#NODE_MOVED.
  DiffKind.UNCHANGED: DiffKind#UNCHANGED.
  ASTNodeKind.RETURN: ASTNodeKind#RETURN.
  ASTNodeKind.EXPRESSION: ASTNodeKind#EXPRESSION.
---
# Module: [`tree_sitter_analyzer/ast_diff.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py)

## Classes
### `ASTDiffHunk`
- def: [`tree_sitter_analyzer/ast_diff.py:183`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L183) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- signature: `class ASTDiffHunk:`
- members:
  - `to_dict(self, include_children: bool = False, with_child_count: bool = False)` — [`L191`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L191)
  - `details` — [`L189`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L189)
  - `diff_kind` — [`L184`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L184) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `new_node` — [`L187`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L187) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `node_kind` — [`L185`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L185) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `old_node` — [`L186`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L186) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `summary` — [`L188`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L188)
- uses (calls/refs, reference-scoped): [`ASTNodeKind`](ast_diff.md#ASTNodeKind), [`DiffKind`](ast_diff.md#DiffKind), [`ASTNodeInfo`](ast_diff.md#ASTNodeInfo), [`to_dict`](ast_diff.md#ASTNodeInfo.to_dict)
- used by: [`_classify_single_hunk`](semantic_change_classifier.md#_classify_single_hunk), [`diff_strings`](ast_diff.md#ASTDiffer.diff_strings), [`_diff_matched_nodes`](ast_diff.md#_diff_matched_nodes), [`diff_files`](ast_diff.md#ASTDiffer.diff_files), [`_diff_children`](ast_diff.md#_diff_children), [`_diff_node_lists`](ast_diff.md#ASTDiffer._diff_node_lists), [`hunk`](semantic_change_classifier.md#ClassifiedHunk.hunk), [`to_dict`](semantic_change_classifier.md#ClassifiedHunk.to_dict), [`to_dict`](ast_diff.md#ASTDiffResult.to_dict), [`hunks`](ast_diff.md#ASTDiffResult.hunks), [`_hunk_name`](semantic_change_classifier.md#_hunk_name), [`_hunk_preview`](semantic_change_classifier.md#_hunk_preview), [`_compute_stats`](ast_diff.md#_compute_stats)  (2 test-only)

### `ASTDiffResult`
- def: [`tree_sitter_analyzer/ast_diff.py:213`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L213)
- signature: `class ASTDiffResult:`
- members:
  - `to_dict(self, include_children: bool = False, with_child_count: bool = False)` — [`L220`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L220)
  - `hunks` — [`L217`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L217)
  - `language` — [`L216`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L216)
  - `new_file` — [`L215`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L215)
  - `old_file` — [`L214`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L214)
  - `summary_stats` — [`L218`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L218)
- uses (calls/refs, reference-scoped): [`ASTDiffHunk`](ast_diff.md#ASTDiffHunk), [`to_dict`](ast_diff.md#ASTDiffHunk.to_dict)
- used by: [`execute`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`diff_strings`](ast_diff.md#ASTDiffer.diff_strings), [`classify`](semantic_change_classifier.md#SemanticChangeClassifier.classify), [`diff_files`](ast_diff.md#ASTDiffer.diff_files), [`execute`](mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.execute), [`execute`](mcp/tools/ast_diff_tool.md#ASTDiffTool.execute), [`diff_string_pairs`](ast_diff.md#ASTDiffer.diff_string_pairs)  (5 test-only)

### `ASTDiffer`
- def: [`tree_sitter_analyzer/ast_diff.py:550`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L550)
- doc: Structural AST diff engine.
- signature: `class ASTDiffer:`
- members:
  - `diff_files(self, old_path: str, new_path: str, language: str | None = None)` — [`L611`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L611) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `diff_string_pairs(self, pairs: list[tuple[str, str, str]], language: str)` — [`L657`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L657)
  - `diff_strings(self, old_source: str, new_source: str, language: str, old_file: str | None = None, new_file: str | None = None)` — [`L562`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L562) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- protocol/private: `__init__`[`L559`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L559), `_diff_node_lists`[`L670`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L670), `_parser`[`L560`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L560)
- uses (calls/refs, reference-scoped): [`Parser`](core/parser.md#Parser), [`tree`](core/parser.md#ParseResult.tree), [`parse_code`](core/parser.md#Parser.parse_code), [`ASTNodeKind`](ast_diff.md#ASTNodeKind), [`success`](core/parser.md#ParseResult.success), [`_language_from_ext`](project_graph.md#_language_from_ext), [`_diff_matched_nodes`](ast_diff.md#_diff_matched_nodes), [`DiffKind`](ast_diff.md#DiffKind), [`kind`](ast_diff.md#ASTNodeInfo.kind), [`name`](ast_diff.md#ASTNodeInfo.name), [`ASTNodeInfo`](ast_diff.md#ASTNodeInfo), [`ASTDiffHunk`](ast_diff.md#ASTDiffHunk), [`node_kind`](ast_diff.md#ASTDiffHunk.node_kind), [`_match_nodes`](ast_diff.md#_match_nodes), [`diff_kind`](ast_diff.md#ASTDiffHunk.diff_kind), [`new_node`](ast_diff.md#ASTDiffHunk.new_node), [`old_node`](ast_diff.md#ASTDiffHunk.old_node), [`hunks`](ast_diff.md#ASTDiffResult.hunks), [`ASTDiffResult`](ast_diff.md#ASTDiffResult), [`NODE_ADDED`](ast_diff.md#DiffKind.NODE_ADDED), [`node_type`](ast_diff.md#ASTNodeInfo.node_type), [`summary`](ast_diff.md#ASTDiffHunk.summary), [`new_file`](ast_diff.md#ASTDiffResult.new_file), [`_compute_stats`](ast_diff.md#_compute_stats), [`language`](ast_diff.md#ASTDiffResult.language), [`old_file`](ast_diff.md#ASTDiffResult.old_file), [`_extract_top_level_nodes`](ast_diff.md#_extract_top_level_nodes), [`NODE_CHANGED`](ast_diff.md#DiffKind.NODE_CHANGED), [`NODE_REMOVED`](ast_diff.md#DiffKind.NODE_REMOVED), [`OTHER`](ast_diff.md#ASTNodeKind.OTHER), [`summary_stats`](ast_diff.md#ASTDiffResult.summary_stats)
- used by: [`execute`](mcp/tools/codegraph_pr_review_tool.md#CodeGraphPRReviewTool.execute), [`execute`](mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.execute), [`_classify_changed_files`](mcp/tools/utils/change_impact_analysis.md#_classify_changed_files), [`execute`](mcp/tools/ast_diff_tool.md#ASTDiffTool.execute), [`_diff_git`](mcp/tools/ast_diff_tool.md#ASTDiffTool._diff_git), [`_diff_git`](mcp/tools/semantic_classify_tool.md#SemanticClassifyTool._diff_git), [`_get_differ`](mcp/tools/ast_diff_tool.md#ASTDiffTool._get_differ), [`_get_differ`](mcp/tools/semantic_classify_tool.md#SemanticClassifyTool._get_differ), [`__init__`](mcp/tools/ast_diff_tool.md#ASTDiffTool.__init__), [`__init__`](mcp/tools/semantic_classify_tool.md#SemanticClassifyTool.__init__)  (4 test-only)

### `ASTNodeInfo`
- def: [`tree_sitter_analyzer/ast_diff.py:142`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L142) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- signature: `class ASTNodeInfo:`
- members:
  - `to_dict(self, include_children: bool = False, with_child_count: bool = False)` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L154)
  - `children` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L152)
  - `end_col` — [`L149`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L149)
  - `end_line` — [`L148`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L148)
  - `kind` — [`L144`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L144) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `name` — [`L145`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L145) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `node_type` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L143)
  - `start_col` — [`L147`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L147)
  - `start_line` — [`L146`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L146)
  - `text_hash` — [`L150`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L150)
  - `text_preview` — [`L151`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L151)
- uses (calls/refs, reference-scoped): [`ASTNodeKind`](ast_diff.md#ASTNodeKind)
- used by: [`_diff_matched_nodes`](ast_diff.md#_diff_matched_nodes), [`_extract_node_info`](ast_diff.md#_extract_node_info), [`_diff_children`](ast_diff.md#_diff_children), [`_diff_node_lists`](ast_diff.md#ASTDiffer._diff_node_lists), [`_extract_signature`](ast_diff.md#_extract_signature), [`_match_nodes`](ast_diff.md#_match_nodes), [`new_node`](ast_diff.md#ASTDiffHunk.new_node), [`old_node`](ast_diff.md#ASTDiffHunk.old_node), [`to_dict`](ast_diff.md#ASTDiffHunk.to_dict), [`_get_body_hash`](ast_diff.md#_get_body_hash), [`_hunk_name`](semantic_change_classifier.md#_hunk_name), [`_hunk_preview`](semantic_change_classifier.md#_hunk_preview), [`_body_hash_changed`](ast_diff.md#_body_hash_changed), [`_child_name_overlap`](ast_diff.md#_child_name_overlap), [`_extract_top_level_nodes`](ast_diff.md#_extract_top_level_nodes)  (4 test-only)

### `ASTNodeKind`  ·  implements/extends Enum, str
- def: [`tree_sitter_analyzer/ast_diff.py:42`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L42) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- signature: `class ASTNodeKind(str, Enum):`
- members:
  - `BLOCK` — [`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L52)
  - `CLASS` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L44)
  - `DECORATOR` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L49)
  - `EXPRESSION` — [`L51`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L51)
  - `FUNCTION` — [`L43`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L43) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
  - `IMPORT` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L47)
  - `METHOD` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L45)
  - `OTHER` — [`L53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L53)
  - `PARAMETER` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L48)
  - `RETURN` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L50)
  - `VARIABLE` — [`L46`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L46)
- used by: [`_classify_single_hunk`](semantic_change_classifier.md#_classify_single_hunk), [`diff_strings`](ast_diff.md#ASTDiffer.diff_strings), [`_classify_node`](ast_diff.md#_classify_node), [`diff_files`](ast_diff.md#ASTDiffer.diff_files), [`kind`](ast_diff.md#ASTNodeInfo.kind), [`node_kind`](ast_diff.md#ASTDiffHunk.node_kind), [`_extract_signature`](ast_diff.md#_extract_signature), [`_match_nodes`](ast_diff.md#_match_nodes), [`_get_body_hash`](ast_diff.md#_get_body_hash)  (28 test-only)

### `DiffKind`  ·  implements/extends Enum, str
- def: [`tree_sitter_analyzer/ast_diff.py:31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L31) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- signature: `class DiffKind(str, Enum):`
- members:
  - `BODY_CHANGED` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L38)
  - `NODE_ADDED` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L32)
  - `NODE_CHANGED` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L34)
  - `NODE_MOVED` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L35)
  - `NODE_REMOVED` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L33)
  - `NODE_RENAMED` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L36)
  - `SIGNATURE_CHANGED` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L37)
  - `UNCHANGED` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L39)
- used by: [`_classify_single_hunk`](semantic_change_classifier.md#_classify_single_hunk), [`diff_strings`](ast_diff.md#ASTDiffer.diff_strings), [`_diff_matched_nodes`](ast_diff.md#_diff_matched_nodes), [`diff_files`](ast_diff.md#ASTDiffer.diff_files), [`_diff_children`](ast_diff.md#_diff_children), [`_diff_node_lists`](ast_diff.md#ASTDiffer._diff_node_lists), [`diff_kind`](ast_diff.md#ASTDiffHunk.diff_kind)  (23 test-only)

## Functions
- `_body_hash_changed(old_n: ASTNodeInfo, new_n: ASTNodeInfo)` — [`L466`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L466)
- `_child_name_overlap(a: ASTNodeInfo, b: ASTNodeInfo)` — [`L375`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L375)
- `_classify_node(node_type: str)` — [`L237`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L237) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- `_compute_stats(hunks: list[ASTDiffHunk])` — [`L531`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L531)
- `_diff_children(old_n: ASTNodeInfo, new_n: ASTNodeInfo)` — [`L496`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L496) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- `_diff_matched_nodes(old_n: ASTNodeInfo, new_n: ASTNodeInfo)` — [`L381`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L381) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- `_extract_node_info(node: Any, source: str, depth: int = 0)` — [`L276`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L276) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- `_extract_signature(node: ASTNodeInfo)` — [`L454`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L454) — documented in [tree_sitter_analyzer-ast_diff](../../concepts/tree_sitter_analyzer-ast_diff.md)
- `_extract_top_level_nodes(tree: Any, source: str)` — [`L306`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L306)
- `_get_body_hash(node: ASTNodeInfo)` — [`L474`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L474)
- `_match_nodes(old_nodes: list[ASTNodeInfo], new_nodes: list[ASTNodeInfo])` — [`L318`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L318)
- `_node_name(node: Any, source: str)` — [`L255`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L255)
- `_preview(text: str, max_len: int = 80)` — [`L269`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L269)
- `_sig_diff(old_sig: dict[str, Any], new_sig: dict[str, Any])` — [`L481`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L481)
- `_text_hash(text: str)` — [`L265`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L265)

## Module values
- `_BLOCK_NODES` — [`L130`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L130)
- `_CLASS_NODES` — [`L72`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L72)
- `_DECORATOR_NODES` — [`L112`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L112)
- `_FUNCTION_NODES` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L56)
- `_IMPORT_NODES` — [`L88`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L88)
- `_PARAM_NODES` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L122)
- `_VARIABLE_NODES` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L101)
- `logger` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_diff.py#L28)

