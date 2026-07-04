---
title: 'Module: tests/unit/test_code_similarity.py'
type: catalog
provenance: extracted
module: tests/unit/test_code_similarity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_code_similarity`/
symbols:
  TestAnalyzeCodeSimilarityWithCache.test_path_filter_limits_cached_scan: TestAnalyzeCodeSimilarityWithCache#test_path_filter_limits_cached_scan().
  TestAnalyzeCodeSimilarityWithCache.test_stale_cache_falls_back_to_live_scan: TestAnalyzeCodeSimilarityWithCache#test_stale_cache_falls_back_to_live_scan().
  TestDetectStructuralClonesCached.test_finds_structural_clones: TestDetectStructuralClonesCached#test_finds_structural_clones().
  TestAnalyzeCodeSimilarityWithCache.test_path_filter_limits_uncached_scan: TestAnalyzeCodeSimilarityWithCache#test_path_filter_limits_uncached_scan().
  TestDetectTextualClonesCached.test_no_clones_returns_empty: TestDetectTextualClonesCached#test_no_clones_returns_empty().
  cached_clone_project: cached_clone_project().
  TestDetectTextualClonesCached.test_finds_clones_via_cache: TestDetectTextualClonesCached#test_finds_clones_via_cache().
  TestDetectTextualClonesCached.test_fallback_when_cache_empty: TestDetectTextualClonesCached#test_fallback_when_cache_empty().
  TestDetectStructuralClonesCached.test_fallback_no_cache: TestDetectStructuralClonesCached#test_fallback_no_cache().
  TestAnalyzeCodeSimilarityWithCache.test_cache_used_by_default: TestAnalyzeCodeSimilarityWithCache#test_cache_used_by_default().
  TestAnalyzeCodeSimilarityWithCache.test_cache_disabled: TestAnalyzeCodeSimilarityWithCache#test_cache_disabled().
  TestAnalyzeCodeSimilarityWithCache.test_structural_only_cached: TestAnalyzeCodeSimilarityWithCache#test_structural_only_cached().
  TestAnalyzeCodeSimilarityWithCache.test_textual_only_cached: TestAnalyzeCodeSimilarityWithCache#test_textual_only_cached().
  TestAnalyzeCodeSimilarityWithCache.test_no_cache_falls_back_gracefully: TestAnalyzeCodeSimilarityWithCache#test_no_cache_falls_back_gracefully().
  TestConsistencyCachedVsUncached.test_textual_clones_match: TestConsistencyCachedVsUncached#test_textual_clones_match().
  TestConsistencyCachedVsUncached.test_structural_clones_match: TestConsistencyCachedVsUncached#test_structural_clones_match().
  TestTextFingerprint.test_identical_after_rename: TestTextFingerprint#test_identical_after_rename().
  TestTextFingerprint.test_different_logic: TestTextFingerprint#test_different_logic().
  TestTextFingerprint.test_whitespace_stripped: TestTextFingerprint#test_whitespace_stripped().
  TestBodySnippet.test_short_body: TestBodySnippet#test_short_body().
  TestBodySnippet.test_long_body_truncated: TestBodySnippet#test_long_body_truncated().
  TestPathFilter.test_matches_glob: TestPathFilter#test_matches_glob().
  TestPathFilter.test_matches_directory_prefix_without_glob: TestPathFilter#test_matches_directory_prefix_without_glob().
  TestPathFilter.test_rejects_other_directories: TestPathFilter#test_rejects_other_directories().
  TestPathFilter.test_accepts_comma_separated_globs: TestPathFilter#test_accepts_comma_separated_globs().
  TestExtractCachedFunctions.test_extracts_from_cache: TestExtractCachedFunctions#test_extracts_from_cache().
  TestExtractCachedFunctions.test_min_lines_filter: TestExtractCachedFunctions#test_min_lines_filter().
  TestExtractCachedFunctions.test_stale_cache_returns_empty_for_fallback: TestExtractCachedFunctions#test_stale_cache_returns_empty_for_fallback().
  clone_project: clone_project().
  path_filtered_clone_project: path_filtered_clone_project().
  TestTextFingerprint: TestTextFingerprint#
  TestBodySnippet: TestBodySnippet#
  TestPathFilter: TestPathFilter#
  TestDetectTextualClonesCached: TestDetectTextualClonesCached#
  TestDetectStructuralClonesCached: TestDetectStructuralClonesCached#
  TestExtractCachedFunctions: TestExtractCachedFunctions#
  TestAnalyzeCodeSimilarityWithCache: TestAnalyzeCodeSimilarityWithCache#
  TestConsistencyCachedVsUncached: TestConsistencyCachedVsUncached#
---
# Module: [`tests/unit/test_code_similarity.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py)

## Classes
### `TestAnalyzeCodeSimilarityWithCache`
- def: [`tests/unit/test_code_similarity.py:251`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L251)
- signature: `class TestAnalyzeCodeSimilarityWithCache:`
- members:
  - `test_cache_disabled(self, clone_project)` — [`L258`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L258)
  - `test_cache_used_by_default(self, cached_clone_project)` — [`L252`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L252)
  - `test_no_cache_falls_back_gracefully(self, tmp_path)` — [`L277`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L277)
  - `test_path_filter_limits_cached_scan(self, path_filtered_clone_project)` — [`L298`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L298)
  - `test_path_filter_limits_uncached_scan(self, path_filtered_clone_project)` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L285)
  - `test_stale_cache_falls_back_to_live_scan(self, path_filtered_clone_project)` — [`L316`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L316)
  - `test_structural_only_cached(self, cached_clone_project)` — [`L265`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L265)
  - `test_textual_only_cached(self, cached_clone_project)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L271)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`analyze_code_similarity`](../../tree_sitter_analyzer/code_similarity.md#analyze_code_similarity), [`functions`](../../tree_sitter_analyzer/code_similarity.md#SimilarityGroup.functions), [`groups`](../../tree_sitter_analyzer/code_similarity.md#SimilarityResult.groups), [`method`](../../tree_sitter_analyzer/code_similarity.md#SimilarityGroup.method), [`stats`](../../tree_sitter_analyzer/code_similarity.md#SimilarityResult.stats), [`file`](../../tree_sitter_analyzer/code_similarity.md#SimilarFunction.file), [`SimilarityResult`](../../tree_sitter_analyzer/code_similarity.md#SimilarityResult)

### `TestBodySnippet`
- def: [`tests/unit/test_code_similarity.py:137`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L137)
- signature: `class TestBodySnippet:`
- members:
  - `test_long_body_truncated(self)` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L141)
  - `test_short_body(self)` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L138)
- uses (calls/refs, reference-scoped): [`_body_snippet`](../../tree_sitter_analyzer/code_similarity.md#_body_snippet)

### `TestConsistencyCachedVsUncached`
- def: [`tests/unit/test_code_similarity.py:335`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L335)
- signature: `class TestConsistencyCachedVsUncached:`
- members:
  - `test_structural_clones_match(self, cached_clone_project)` — [`L342`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L342)
  - `test_textual_clones_match(self, cached_clone_project)` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L336)
- uses (calls/refs, reference-scoped): [`detect_structural_clones_cached`](../../tree_sitter_analyzer/code_similarity.md#detect_structural_clones_cached), [`detect_structural_clones`](../../tree_sitter_analyzer/code_similarity.md#detect_structural_clones), [`detect_textual_clones_cached`](../../tree_sitter_analyzer/code_similarity.md#detect_textual_clones_cached), [`detect_textual_clones`](../../tree_sitter_analyzer/code_similarity.md#detect_textual_clones)

### `TestDetectStructuralClonesCached`
- def: [`tests/unit/test_code_similarity.py:197`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L197)
- signature: `class TestDetectStructuralClonesCached:`
- members:
  - `test_fallback_no_cache(self, clone_project)` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L209)
  - `test_finds_structural_clones(self, cached_clone_project)` — [`L198`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L198)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`detect_structural_clones_cached`](../../tree_sitter_analyzer/code_similarity.md#detect_structural_clones_cached), [`functions`](../../tree_sitter_analyzer/code_similarity.md#SimilarityGroup.functions), [`method`](../../tree_sitter_analyzer/code_similarity.md#SimilarityGroup.method), [`name`](../../tree_sitter_analyzer/code_similarity.md#SimilarFunction.name), [`similarity`](../../tree_sitter_analyzer/code_similarity.md#SimilarityGroup.similarity)

### `TestDetectTextualClonesCached`
- def: [`tests/unit/test_code_similarity.py:162`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L162)
- signature: `class TestDetectTextualClonesCached:`
- members:
  - `test_fallback_when_cache_empty(self, clone_project)` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L186)
  - `test_finds_clones_via_cache(self, cached_clone_project)` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L163)
  - `test_no_clones_returns_empty(self, tmp_path)` — [`L172`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L172)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../tree_sitter_analyzer/ast_cache.md#ASTCache), [`close`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.close), [`index_project`](../../tree_sitter_analyzer/ast_cache.md#ASTCache.index_project), [`detect_textual_clones_cached`](../../tree_sitter_analyzer/code_similarity.md#detect_textual_clones_cached), [`functions`](../../tree_sitter_analyzer/code_similarity.md#SimilarityGroup.functions), [`method`](../../tree_sitter_analyzer/code_similarity.md#SimilarityGroup.method)

### `TestExtractCachedFunctions`
- def: [`tests/unit/test_code_similarity.py:220`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L220)
- signature: `class TestExtractCachedFunctions:`
- members:
  - `test_extracts_from_cache(self, cached_clone_project)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L221)
  - `test_min_lines_filter(self, cached_clone_project)` — [`L235`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L235)
  - `test_stale_cache_returns_empty_for_fallback(self, cached_clone_project)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L241)
- uses (calls/refs, reference-scoped): [`_extract_cached_functions`](../../tree_sitter_analyzer/code_similarity.md#_extract_cached_functions)

### `TestPathFilter`
- def: [`tests/unit/test_code_similarity.py:148`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L148)
- signature: `class TestPathFilter:`
- members:
  - `test_accepts_comma_separated_globs(self)` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L158)
  - `test_matches_directory_prefix_without_glob(self)` — [`L152`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L152)
  - `test_matches_glob(self)` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L149)
  - `test_rejects_other_directories(self)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L155)
- uses (calls/refs, reference-scoped): [`_matches_path_filter`](../../tree_sitter_analyzer/code_similarity.md#_matches_path_filter)

### `TestTextFingerprint`
- def: [`tests/unit/test_code_similarity.py:120`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L120)
- signature: `class TestTextFingerprint:`
- members:
  - `test_different_logic(self)` — [`L126`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L126)
  - `test_identical_after_rename(self)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L121)
  - `test_whitespace_stripped(self)` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L131)
- uses (calls/refs, reference-scoped): [`_text_fingerprint`](../../tree_sitter_analyzer/code_similarity.md#_text_fingerprint)

## Functions
- `cached_clone_project(clone_project)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L68)
- `clone_project(tmp_path)` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L29)
- `path_filtered_clone_project(tmp_path)` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_code_similarity.py#L78)

