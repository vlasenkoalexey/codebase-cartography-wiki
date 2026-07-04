---
title: 'Module: tests/unit/test_call_path.py'
type: catalog
provenance: extracted
module: tests/unit/test_call_path.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_call_path`/
symbols:
  _make_cache_with_edges: _make_cache_with_edges().
  TestCallPathResult.test_with_paths: TestCallPathResult#test_with_paths().
  TestCallPathFinderForward.test_linear_forward: TestCallPathFinderForward#test_linear_forward().
  TestFallbackBackwardGate.test_bidirectional_fallback_backward_duplicate_deduped: TestFallbackBackwardGate#test_bidirectional_fallback_backward_duplicate_deduped().
  TestFallbackBackwardGate.test_bidirectional_fallback_backward_adds_distinct_chain: TestFallbackBackwardGate#test_bidirectional_fallback_backward_adds_distinct_chain().
  TestBidirectionalDistinctByFile.test_two_chains_differing_only_by_intermediate_file_preserved: TestBidirectionalDistinctByFile#test_two_chains_differing_only_by_intermediate_file_preserved().
  TestBidirectionalMeetingOrder.test_three_plus_hop_path_in_executable_order: TestBidirectionalMeetingOrder#test_three_plus_hop_path_in_executable_order().
  TestCallPathFinderBidirectional.test_same_function: TestCallPathFinderBidirectional#test_same_function().
  TestCallPathFinderCrossFile.test_two_hop_cross_file_with_unresolved_intermediate: TestCallPathFinderCrossFile#test_two_hop_cross_file_with_unresolved_intermediate().
  TestCallPathFinderCrossFile.test_two_hop_cross_file_with_resolved_intermediate: TestCallPathFinderCrossFile#test_two_hop_cross_file_with_resolved_intermediate().
  TestCallChain.test_chain_with_hops: TestCallChain#test_chain_with_hops().
  TestCallPathFinderForward.test_no_path_forward: TestCallPathFinderForward#test_no_path_forward().
  TestCallPathFinderForward.test_diamond_forward: TestCallPathFinderForward#test_diamond_forward().
  TestCallPathFinderForward.test_max_depth_respected: TestCallPathFinderForward#test_max_depth_respected().
  TestCallPathFinderForward.test_max_paths_respected: TestCallPathFinderForward#test_max_paths_respected().
  TestCallPathFinderBackward.test_linear_backward: TestCallPathFinderBackward#test_linear_backward().
  TestCallPathFinderBackward.test_no_path_backward: TestCallPathFinderBackward#test_no_path_backward().
  TestCallPathFinderBidirectional.test_linear_bidirectional: TestCallPathFinderBidirectional#test_linear_bidirectional().
  TestCallPathFinderBidirectional.test_diamond_bidirectional: TestCallPathFinderBidirectional#test_diamond_bidirectional().
  TestCallPathFinderBidirectional.test_direct_call_bidirectional_no_target_file: TestCallPathFinderBidirectional#test_direct_call_bidirectional_no_target_file().
  TestCallPathFinderBidirectional.test_direct_call_forward_finds_path: TestCallPathFinderBidirectional#test_direct_call_forward_finds_path().
  TestCallPathHopCalleFile.test_hop_callee_file_is_definition_file_not_caller_file: TestCallPathHopCalleFile#test_hop_callee_file_is_definition_file_not_caller_file().
  TestCallPathHopCalleFile.test_hop_callee_file_empty_when_resolution_unknown: TestCallPathHopCalleFile#test_hop_callee_file_empty_when_resolution_unknown().
  TestCallPathHopCalleFile.test_bidirectional_hop_callee_file_is_definition_file: TestCallPathHopCalleFile#test_bidirectional_hop_callee_file_is_definition_file().
  TestBidirectionalMeetingOrder.test_no_duplicate_paths_from_both_frontiers: TestBidirectionalMeetingOrder#test_no_duplicate_paths_from_both_frontiers().
  TestFallbackBackwardGate.fake_forward: TestFallbackBackwardGate#fake_forward().
  TestFallbackBackwardGate.fake_backward: TestFallbackBackwardGate#fake_backward().
  TestCallPathResult.test_no_paths: TestCallPathResult#test_no_paths().
  _LINEAR_EDGES: _LINEAR_EDGES.
  TestCallPathFinderFallback.test_no_cache_falls_back: TestCallPathFinderFallback#test_no_cache_falls_back().
  TestCallPathFinderCLI.test_cli_tool_instantiation: TestCallPathFinderCLI#test_cli_tool_instantiation().
  TestCallChain.test_empty_chain: TestCallChain#test_empty_chain().
  TestCallPathFinderCLI.test_validate_missing_source: TestCallPathFinderCLI#test_validate_missing_source().
  TestCallPathFinderCLI.test_validate_missing_target: TestCallPathFinderCLI#test_validate_missing_target().
  _DIAMOND_EDGES: _DIAMOND_EDGES.
  TestFilesInChain.test_empty: TestFilesInChain#test_empty().
  TestFilesInChain.test_single_file: TestFilesInChain#test_single_file().
  TestFilesInChain.test_cross_file: TestFilesInChain#test_cross_file().
  TestPathSignatureFileAware.test_same_names_different_file_have_distinct_signatures: TestPathSignatureFileAware#test_same_names_different_file_have_distinct_signatures().
  TestPathSignatureFileAware.test_identical_chains_share_signature: TestPathSignatureFileAware#test_identical_chains_share_signature().
  _FOUR_HOP_EDGES: _FOUR_HOP_EDGES.
  _DISTINCT_BY_FILE_EDGES: _DISTINCT_BY_FILE_EDGES.
  TestCallChain: TestCallChain#
  TestCallPathResult: TestCallPathResult#
  TestFilesInChain: TestFilesInChain#
  TestCallPathFinderForward: TestCallPathFinderForward#
  TestCallPathFinderBackward: TestCallPathFinderBackward#
  TestCallPathFinderBidirectional: TestCallPathFinderBidirectional#
  TestCallPathFinderCrossFile: TestCallPathFinderCrossFile#
  TestCallPathFinderFallback: TestCallPathFinderFallback#
  TestCallPathFinderCLI: TestCallPathFinderCLI#
  TestCallPathHopCalleFile: TestCallPathHopCalleFile#
  TestPathSignatureFileAware: TestPathSignatureFileAware#
  TestBidirectionalDistinctByFile: TestBidirectionalDistinctByFile#
  TestBidirectionalMeetingOrder: TestBidirectionalMeetingOrder#
  TestFallbackBackwardGate: TestFallbackBackwardGate#
---
# Module: [`tests/unit/test_call_path.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py)

## Classes
### `TestBidirectionalDistinctByFile`
- def: [`tests/unit/test_call_path.py:590`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L590)
- doc: #968: distinct-by-file chains must both survive the bidirectional BFS.
- signature: `class TestBidirectionalDistinctByFile:`
- members:
  - `test_two_chains_differing_only_by_intermediate_file_preserved(self, tmp_path)` — [`L593`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L593)
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`data_source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.data_source), [`hops`](../../tree_sitter_analyzer/call_path.md#CallChain.hops)  (2 test-only)

### `TestBidirectionalMeetingOrder`
- def: [`tests/unit/test_call_path.py:604`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L604)
- doc: #951: forward-side meetings must reconstruct in caller-&gt;callee order.
- signature: `class TestBidirectionalMeetingOrder:`
- members:
  - `test_no_duplicate_paths_from_both_frontiers(self, tmp_path)` — [`L622`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L622) — A meeting node found by both passes is recorded exactly once.
  - `test_three_plus_hop_path_in_executable_order(self, tmp_path)` — [`L607`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L607)
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`data_source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.data_source), [`hops`](../../tree_sitter_analyzer/call_path.md#CallChain.hops)  (3 test-only)

### `TestCallChain`
- def: [`tests/unit/test_call_path.py:143`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L143)
- signature: `class TestCallChain:`
- members:
  - `test_chain_with_hops(self)` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L151)
  - `test_empty_chain(self)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L144)
- uses (calls/refs, reference-scoped): [`CallChain`](../../tree_sitter_analyzer/call_path.md#CallChain), [`hops`](../../tree_sitter_analyzer/call_path.md#CallChain.hops), [`to_dict`](../../tree_sitter_analyzer/call_path.md#CallChain.to_dict), [`total_hops`](../../tree_sitter_analyzer/call_path.md#CallChain.total_hops), [`files_crossed`](../../tree_sitter_analyzer/call_path.md#CallChain.files_crossed)

### `TestCallPathFinderBackward`
- def: [`tests/unit/test_call_path.py:233`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L233)
- signature: `class TestCallPathFinderBackward:`
- members:
  - `test_linear_backward(self, tmp_path)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L234)
  - `test_no_path_backward(self, tmp_path)` — [`L240`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L240)
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder)  (2 test-only)

### `TestCallPathFinderBidirectional`
- def: [`tests/unit/test_call_path.py:247`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L247)
- signature: `class TestCallPathFinderBidirectional:`
- members:
  - `test_diamond_bidirectional(self, tmp_path)` — [`L254`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L254)
  - `test_direct_call_bidirectional_no_target_file(self, tmp_path)` — [`L267`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L267) — #797: bidirectional with no target_file must find a direct 1-hop call.
  - `test_direct_call_forward_finds_path(self, tmp_path)` — [`L290`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L290) — Baseline: forward BFS always finds the direct 1-hop call.
  - `test_linear_bidirectional(self, tmp_path)` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L248)
  - `test_same_function(self, tmp_path)` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L260)
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`data_source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.data_source)  (3 test-only)

### `TestCallPathFinderCLI`
- def: [`tests/unit/test_call_path.py:381`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L381)
- signature: `class TestCallPathFinderCLI:`
- members:
  - `test_cli_tool_instantiation(self, tmp_path)` — [`L382`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L382)
  - `test_validate_missing_source(self, tmp_path)` — [`L393`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L393)
  - `test_validate_missing_target(self, tmp_path)` — [`L403`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L403)
- uses (calls/refs, reference-scoped): [`CodeGraphCallPathTool`](../../tree_sitter_analyzer/mcp/tools/call_path_tool.md#CodeGraphCallPathTool), [`get_tool_definition`](../../tree_sitter_analyzer/mcp/tools/call_path_tool.md#CodeGraphCallPathTool.get_tool_definition), [`validate_arguments`](../../tree_sitter_analyzer/mcp/tools/call_path_tool.md#CodeGraphCallPathTool.validate_arguments), [`get_tool_schema`](../../tree_sitter_analyzer/mcp/tools/call_path_tool.md#CodeGraphCallPathTool.get_tool_schema)

### `TestCallPathFinderCrossFile`
- def: [`tests/unit/test_call_path.py:307`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L307)
- doc: #734: 2-hop cross-file chains must not dead-end when the intermediate
- signature: `class TestCallPathFinderCrossFile:`
- members:
  - `test_two_hop_cross_file_with_resolved_intermediate(self, tmp_path)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L345) — Baseline: same chain with callee_resolved_file set must also work.
  - `test_two_hop_cross_file_with_unresolved_intermediate(self, tmp_path)` — [`L321`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L321) — main(a.py) → foo(b.py, unresolved) → bar(c.py) must yield 1 path.
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`data_source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.data_source), [`total_hops`](../../tree_sitter_analyzer/call_path.md#CallChain.total_hops)  (1 test-only)

### `TestCallPathFinderFallback`
- def: [`tests/unit/test_call_path.py:369`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L369)
- signature: `class TestCallPathFinderFallback:`
- members:
  - `test_no_cache_falls_back(self, tmp_path)` — [`L370`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L370)
- uses (calls/refs, reference-scoped): [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`data_source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.data_source)

### `TestCallPathFinderForward`
- def: [`tests/unit/test_call_path.py:196`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L196)
- signature: `class TestCallPathFinderForward:`
- members:
  - `test_diamond_forward(self, tmp_path)` — [`L214`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L214)
  - `test_linear_forward(self, tmp_path)` — [`L197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L197)
  - `test_max_depth_respected(self, tmp_path)` — [`L220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L220)
  - `test_max_paths_respected(self, tmp_path)` — [`L226`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L226)
  - `test_no_path_forward(self, tmp_path)` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L208)
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`data_source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.data_source), [`total_hops`](../../tree_sitter_analyzer/call_path.md#CallChain.total_hops), [`source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.source), [`target`](../../tree_sitter_analyzer/call_path.md#CallPathResult.target)  (3 test-only)

### `TestCallPathHopCalleFile`
- def: [`tests/unit/test_call_path.py:414`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L414)
- doc: #735: hop callee_file must be the DEFINITION file, not the call-site file.
- signature: `class TestCallPathHopCalleFile:`
- members:
  - `test_bidirectional_hop_callee_file_is_definition_file(self, tmp_path)` — [`L465`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L465) — Same fix must apply in the bidirectional BFS path.
  - `test_hop_callee_file_empty_when_resolution_unknown(self, tmp_path)` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L441) — When callee_resolved_file is empty, callee_file must be '' not the caller's file.
  - `test_hop_callee_file_is_definition_file_not_caller_file(self, tmp_path)` — [`L417`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L417) — When callee_resolved_file is set, callee_file in the hop must use it.
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`find_path`](../../tree_sitter_analyzer/call_path.md#CallPathFinder.find_path), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`hops`](../../tree_sitter_analyzer/call_path.md#CallChain.hops)  (1 test-only)

### `TestCallPathResult`
- def: [`tests/unit/test_call_path.py:166`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L166)
- signature: `class TestCallPathResult:`
- members:
  - `test_no_paths(self)` — [`L167`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L167)
  - `test_with_paths(self)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L173)
- uses (calls/refs, reference-scoped): [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`to_dict`](../../tree_sitter_analyzer/call_path.md#CallPathResult.to_dict), [`CallChain`](../../tree_sitter_analyzer/call_path.md#CallChain), [`data_source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.data_source), [`hops`](../../tree_sitter_analyzer/call_path.md#CallChain.hops), [`CallPathResult`](../../tree_sitter_analyzer/call_path.md#CallPathResult), [`total_hops`](../../tree_sitter_analyzer/call_path.md#CallChain.total_hops), [`source`](../../tree_sitter_analyzer/call_path.md#CallPathResult.source), [`target`](../../tree_sitter_analyzer/call_path.md#CallPathResult.target), [`files_crossed`](../../tree_sitter_analyzer/call_path.md#CallChain.files_crossed)

### `TestFallbackBackwardGate`
- def: [`tests/unit/test_call_path.py:630`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L630)
- doc: #968: parse-fallback backward pass runs and is merged with signature dedup.
- signature: `class TestFallbackBackwardGate:`
- members:
  - `fake_backward(g, *a)` — [`L655`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L655)
  - `fake_forward(g, *a)` — [`L651`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L651)
  - `test_bidirectional_fallback_backward_adds_distinct_chain(self, tmp_path)` — [`L673`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L673)
  - `test_bidirectional_fallback_backward_duplicate_deduped(self, tmp_path)` — [`L640`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L640)
- uses (calls/refs, reference-scoped): [`CallGraph`](../../tree_sitter_analyzer/call_graph.md#CallGraph), [`build`](../../tree_sitter_analyzer/call_graph.md#CallGraph.build), [`paths`](../../tree_sitter_analyzer/call_path.md#CallPathResult.paths), [`_fallback_graph`](../../tree_sitter_analyzer/call_path.md#CallPathFinder._fallback_graph), [`CallPathFinder`](../../tree_sitter_analyzer/call_path.md#CallPathFinder), [`CallChain`](../../tree_sitter_analyzer/call_path.md#CallChain), [`hops`](../../tree_sitter_analyzer/call_path.md#CallChain.hops), [`_bfs_graph_backward`](../../tree_sitter_analyzer/call_path.md#CallPathFinder._bfs_graph_backward), [`_bfs_graph_forward`](../../tree_sitter_analyzer/call_path.md#CallPathFinder._bfs_graph_forward), [`total_hops`](../../tree_sitter_analyzer/call_path.md#CallChain.total_hops), [`files_crossed`](../../tree_sitter_analyzer/call_path.md#CallChain.files_crossed)

### `TestFilesInChain`
- def: [`tests/unit/test_call_path.py:185`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L185)
- signature: `class TestFilesInChain:`
- members:
  - `test_cross_file(self)` — [`L192`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L192)
  - `test_empty(self)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L186)
  - `test_single_file(self)` — [`L189`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L189)
- uses (calls/refs, reference-scoped): [`_files_in_chain`](../../tree_sitter_analyzer/call_path.md#_files_in_chain)

### `TestPathSignatureFileAware`
- def: [`tests/unit/test_call_path.py:544`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L544)
- doc: #968: dedup signature must distinguish chains by node file identity.
- signature: `class TestPathSignatureFileAware:`
- members:
  - `test_identical_chains_share_signature(self)` — [`L578`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L578)
  - `test_same_names_different_file_have_distinct_signatures(self)` — [`L547`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L547)
- uses (calls/refs, reference-scoped): [`_path_signature`](../../tree_sitter_analyzer/call_path.md#_path_signature)

## Functions
- `_make_cache_with_edges(tmp_path: Path, edges: list[dict])` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L18) — Build a cache whose DB holds the call edges in the unified ``edges`` table.

## Module values
- `_DIAMOND_EDGES` — [`L115`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L115)
- `_DISTINCT_BY_FILE_EDGES` — [`L516`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L516)
- `_FOUR_HOP_EDGES` — [`L490`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L490)
- `_LINEAR_EDGES` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_call_path.py#L97)

