---
title: 'Module: tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.mcp.tools.symbol_lineage_tool`/
symbols:
  SymbolLineageTool.execute: SymbolLineageTool#execute().
  SymbolLineageTool._hierarchy_for: SymbolLineageTool#_hierarchy_for().
  SymbolLineageTool._get_dep_graph: SymbolLineageTool#_get_dep_graph().
  SymbolLineageTool._finalize_and_cache_response: SymbolLineageTool#_finalize_and_cache_response().
  SymbolLineageTool._on_project_root_changed: SymbolLineageTool#_on_project_root_changed().
  SymbolLineageTool: SymbolLineageTool#
  SymbolLineageTool._collect_definitions_and_refs: SymbolLineageTool#_collect_definitions_and_refs().
  SymbolLineageTool._assemble_lineage_response: SymbolLineageTool#_assemble_lineage_response().
  _enrich_references_with_callers: _enrich_references_with_callers().
  SymbolLineageTool._invalidate_symbol_cache_on_stale_ast_index: SymbolLineageTool#_invalidate_symbol_cache_on_stale_ast_index().
  _find_definitions_via_grep: _find_definitions_via_grep().
  SymbolLineageTool._dep_graph: SymbolLineageTool#_dep_graph.
  SymbolLineageTool._explain_fingerprint_delta: SymbolLineageTool#_explain_fingerprint_delta().
  SymbolLineageTool._compute_blast_radius: SymbolLineageTool#_compute_blast_radius().
  SymbolLineageTool._invalidate_symbol_cache_on_index_change: SymbolLineageTool#_invalidate_symbol_cache_on_index_change().
  SymbolLineageTool._dep_graph_fingerprint: SymbolLineageTool#_dep_graph_fingerprint.
  SymbolLineageTool._dep_graph_built_at: SymbolLineageTool#_dep_graph_built_at.
  SymbolLineageTool._cache_invalidated_reason: SymbolLineageTool#_cache_invalidated_reason.
  _build_truncations_and_summary_line: _build_truncations_and_summary_line().
  _normalize_scope_file_paths: _normalize_scope_file_paths().
  SymbolLineageTool._symbol_cache: SymbolLineageTool#_symbol_cache.
  SymbolLineageTool._try_cached_lineage: SymbolLineageTool#_try_cached_lineage().
  _reclassify_definition_like: _reclassify_definition_like().
  _assess_risk: _assess_risk().
  _iter_grep_candidate_files: _iter_grep_candidate_files().
  SymbolLineageTool._ast_index_mtime_ns: SymbolLineageTool#_ast_index_mtime_ns.
  SymbolLineageTool.get_tool_schema: SymbolLineageTool#get_tool_schema().
  SymbolLineageTool._index_signature: SymbolLineageTool#_index_signature().
  logger: logger.
  _REF_LIMIT: _REF_LIMIT.
  _DOWNSTREAM_LIMIT: _DOWNSTREAM_LIMIT.
  _filter_references_to_scope: _filter_references_to_scope().
  _apply_grep_fallback_defs: _apply_grep_fallback_defs().
  _verdict_and_next_step: _verdict_and_next_step().
  SymbolLineageTool._validate_project_root: SymbolLineageTool#_validate_project_root().
  _is_definition_like: _is_definition_like().
  _line_looks_like_definition: _line_looks_like_definition().
  SymbolLineageTool.get_tool_definition: SymbolLineageTool#get_tool_definition().
  _HIER_LIMIT: _HIER_LIMIT.
  _DEF_LIMIT: _DEF_LIMIT.
  _UPSTREAM_LIMIT: _UPSTREAM_LIMIT.
  _TEST_LIMIT: _TEST_LIMIT.
  _build_agent_summary_block: _build_agent_summary_block().
  SymbolLineageTool.validate_arguments: SymbolLineageTool#validate_arguments().
  SymbolLineageTool._collect_symbol_files: SymbolLineageTool#_collect_symbol_files().
  _normalize_bare_symbol: _normalize_bare_symbol().
  _build_grep_definition_regexes: _build_grep_definition_regexes().
  _scan_file_for_definitions: _scan_file_for_definitions().
  TOOL_SCHEMA.TOOL_SCHEMA: TOOL_SCHEMA.TOOL_SCHEMA.
  _RISK_TO_VERDICT._RISK_TO_VERDICT: _RISK_TO_VERDICT._RISK_TO_VERDICT.
  _DEFINITION_LIKE_TYPES._DEFINITION_LIKE_TYPES: _DEFINITION_LIKE_TYPES._DEFINITION_LIKE_TYPES.
  _DEFINITION_LINE_PREFIXES._DEFINITION_LINE_PREFIXES: _DEFINITION_LINE_PREFIXES._DEFINITION_LINE_PREFIXES.
  _K3_FALLBACK_EXTS._K3_FALLBACK_EXTS: _K3_FALLBACK_EXTS._K3_FALLBACK_EXTS.
  _K3_FALLBACK_EXCLUDE._K3_FALLBACK_EXCLUDE: _K3_FALLBACK_EXCLUDE._K3_FALLBACK_EXCLUDE.
  SymbolLineageTool.__init__: SymbolLineageTool#__init__().
---
# Module: [`tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py)

## Classes
### `SymbolLineageTool`  ·  implements/extends BaseMCPTool
- def: [`tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py:205`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L205)
- doc: Trace symbol lineage: definitions, references, file-level downstream impact.
- signature: `class SymbolLineageTool(BaseMCPTool):`
- members:
  - `_assemble_lineage_response(*, symbol: str, definitions: list[dict[str, Any]], references: list[dict[str, Any]], all_symbol_files: set[str], downstream_files: set[str], upstream_files: set[str], test_files: list[str], risk: dict[str, Any], summary_line: str, verdict: str, agent_summary: dict[str, Any], hierarchy: dict[str, Any] | None = None)` — [`L610`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L610) — Assemble the canonical lineage envelope with G6 truncation + r37u verdict.
  - `_collect_definitions_and_refs(self, symbol: str)` — [`L433`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L433) — Find references, reclassify (H12), K3 grep fallback, and #757 caller enrichment.
  - `_collect_symbol_files(definitions: list[dict[str, Any]], references: list[dict[str, Any]])` — [`L471`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L471) — Union of ``file`` keys across definitions + references.
  - `_compute_blast_radius(graph: Any, all_symbol_files: set[str])` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L481) — Forward + reverse blast radius from the dep graph (empty when graph absent).
  - `_finalize_and_cache_response(self, response: dict[str, Any], cache_key: tuple[str, int, tuple[str, ...]], started: float, output_format: str)` — [`L671`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L671) — Cache a deep copy, stamp elapsed/from_cache, apply TOON formatting.
  - `_get_dep_graph(self)` — [`L237`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L237) — Return cached dependency graph, building it on first use.
  - `_hierarchy_for(self, symbol: str)` — [`L546`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L546) — #568: the advertised inheritance/override lineage.
  - `_index_signature(self)` — [`L502`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L502) — Max ``mtime_ns`` across the AST index DB and its WAL/SHM sidecars.
  - `_invalidate_symbol_cache_on_index_change(self)` — [`L523`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L523) — Clear the per-symbol cache when the AST index changed (#568).
  - `_invalidate_symbol_cache_on_stale_ast_index(self)` — [`L538`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L538) — Clear cached lineage responses when source has outpaced ast_index.
  - `_try_cached_lineage(self, cache_key: tuple[str, int, tuple[str, ...]], started: float)` — [`L411`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L411) — Return a deep-copied cached response if one exists, else ``None``.
  - `_validate_project_root(self)` — [`L403`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L403) — Reject when project_root is unset or not a directory.
  - `execute(self, arguments: dict[str, Any])` — [`L321`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L321) — Symbol lineage analysis with cache + grep fallback + blast radius. — documented in [tree_sitter_analyzer-mcp-tools-facade_tool](../../../../concepts/tree_sitter_analyzer-mcp-tools-facade_tool.md)
  - `get_tool_definition(self)` — [`L293`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L293)
  - `get_tool_schema(self)` — [`L290`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L290)
  - `validate_arguments(self, arguments: dict[str, Any])` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L312)
- protocol/private: `__init__`[`L208`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L208), `_ast_index_mtime_ns`[`L225`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L225), `_cache_invalidated_reason`[`L219`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L219), `_dep_graph`[`L211`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L211), `_dep_graph_built_at`[`L218`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L218), `_dep_graph_fingerprint`[`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L217), `_explain_fingerprint_delta`[`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L276), `_on_project_root_changed`[`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L228), `_symbol_cache`[`L212`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L212)
- uses (calls/refs, reference-scoped): [`ASTCache`](../../ast_cache.md#ASTCache), [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`project_root`](base_tool.md#BaseMCPTool.project_root), [`apply_toon_format_to_response`](../utils/format_helper.md#apply_toon_format_to_response), [`close`](../../ast_cache.md#ASTCache.close), [`DependencyGraph`](../../project_graph.md#DependencyGraph), [`__init__`](base_tool.md#BaseMCPTool.__init__), [`ClassHierarchy`](../../class_hierarchy.md#ClassHierarchy), [`compute_graph_fingerprint`](../../_graph_cache_fingerprint.md#compute_graph_fingerprint), [`subclasses_of`](../../class_hierarchy.md#ClassHierarchy.subclasses_of), [`build`](../../class_hierarchy.md#ClassHierarchy.build), [`file_count`](../../_graph_cache_fingerprint.md#GraphFingerprint.file_count), [`superclasses_of`](../../class_hierarchy.md#ClassHierarchy.superclasses_of), [`execute_find_references`](query_symbol_search.md#execute_find_references), [`GraphFingerprint`](../../_graph_cache_fingerprint.md#GraphFingerprint), [`is_ast_index_stale`](../../_graph_cache_fingerprint.md#is_ast_index_stale), [`has_class`](../../class_hierarchy.md#ClassHierarchy.has_class), [`_enrich_references_with_callers`](symbol_lineage_tool.md#_enrich_references_with_callers), [`BlastRadius`](../../project_graph.md#BlastRadius), [`forward`](../../project_graph.md#BlastRadius.forward), [`reverse`](../../project_graph.md#BlastRadius.reverse), [`max_mtime_ns`](../../_graph_cache_fingerprint.md#GraphFingerprint.max_mtime_ns), [`_assess_risk`](symbol_lineage_tool.md#_assess_risk), [`_build_truncations_and_summary_line`](symbol_lineage_tool.md#_build_truncations_and_summary_line), [`_normalize_scope_file_paths`](symbol_lineage_tool.md#_normalize_scope_file_paths), [`_reclassify_definition_like`](symbol_lineage_tool.md#_reclassify_definition_like), [`logger`](symbol_lineage_tool.md#logger), [`_DOWNSTREAM_LIMIT`](symbol_lineage_tool.md#_DOWNSTREAM_LIMIT), [`_REF_LIMIT`](symbol_lineage_tool.md#_REF_LIMIT), [`_filter_references_to_scope`](symbol_lineage_tool.md#_filter_references_to_scope), [`_apply_grep_fallback_defs`](symbol_lineage_tool.md#_apply_grep_fallback_defs), [`_verdict_and_next_step`](symbol_lineage_tool.md#_verdict_and_next_step), [`_HIER_LIMIT`](symbol_lineage_tool.md#_HIER_LIMIT), [`TOOL_SCHEMA`](symbol_lineage_tool.md#TOOL_SCHEMA.TOOL_SCHEMA), [`_DEF_LIMIT`](symbol_lineage_tool.md#_DEF_LIMIT), [`_TEST_LIMIT`](symbol_lineage_tool.md#_TEST_LIMIT), [`_UPSTREAM_LIMIT`](symbol_lineage_tool.md#_UPSTREAM_LIMIT), [`_build_agent_summary_block`](symbol_lineage_tool.md#_build_agent_summary_block)  (1 test-only)
- used by: [`BaseMCPTool`](base_tool.md#BaseMCPTool), [`execute`](base_tool.md#BaseMCPTool.execute), [`get_tool_definition`](base_tool.md#BaseMCPTool.get_tool_definition), [`get_tool_schema`](base_tool.md#BaseMCPTool.get_tool_schema), [`validate_arguments`](base_tool.md#BaseMCPTool.validate_arguments), [`build_nav_facade`](nav_facade.md#build_nav_facade), [`_on_project_root_changed`](base_tool.md#BaseMCPTool._on_project_root_changed)  (18 test-only)

## Functions
- `_apply_grep_fallback_defs(definitions: list[dict[str, Any]], references: list[dict[str, Any]], project_root: str, symbol: str)` — [`L87`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L87) — K3 fix: text-grep the project for definitions when the AST scan missed them.
- `_assess_risk(def_count: int, ref_count: int, downstream_count: int)` — [`L897`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L897)
- `_build_agent_summary_block(summary_line: str, next_step: str, verdict: str, truncations: list[str])` — [`L188`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L188) — Canonical agent_summary block with optional ``truncations`` echo.
- `_build_grep_definition_regexes(bare_name: str)` — [`L1090`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L1090) — Return (whole-word file-pre-check, full-line definition match) regexes.
- `_build_truncations_and_summary_line(symbol: str, definitions: list[dict[str, Any]], references: list[dict[str, Any]], downstream_files: set[str], risk: dict[str, Any])` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L123) — G6: compose the truncation list + the headline summary_line.
- `_enrich_references_with_callers(references: list[dict[str, Any]], project_root: str, symbol: str)` — [`L940`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L940) — #757: augment AST-element references with real call-site callers.
- `_filter_references_to_scope(references: list[dict[str, Any]], scope_files: set[str])` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L175)
- `_find_definitions_via_grep(project_root: str, symbol: str)` — [`L1056`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L1056) — Project-wide text scan for definition sites of ``symbol``.
- `_is_definition_like(element_type: str)` — [`L762`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L762) — Return ``True`` when ``element_type`` denotes a definition site.
- `_iter_grep_candidate_files(root: Path)` — [`L1111`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L1111) — Yield source files under ``root`` (manual scandir walk, excludes pruned).
- `_line_looks_like_definition(project_root: str, file_rel: str, line_no: int, symbol: str)` — [`L779`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L779) — Return ``True`` when the source line at ``line_no`` is a def site.
- `_normalize_bare_symbol(symbol: str)` — [`L1083`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L1083) — Return the trailing component of ``a.b.c`` style symbols.
- `_normalize_scope_file_paths(project_root: str, file_paths: list[Any])` — [`L159`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L159)
- `_reclassify_definition_like(definitions: list[dict[str, Any]], references: list[dict[str, Any]], project_root: str | None = None, symbol: str | None = None)` — [`L818`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L818) — H12 fix: promote definition-like references into ``definitions``.
- `_scan_file_for_definitions(file_path: Path, root: Path, bare_name: str, word_re: re.Pattern[str], line_re: re.Pattern[str], hits: list[dict[str, Any]], seen_keys: set[tuple[str, int]])` — [`L1140`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L1140) — Read ``file_path`` and append every matching definition line to ``hits``.
- `_verdict_and_next_step(risk_level: str)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L145) — Map a risk level to (verdict, next_step) per the lineage contract.

## Module values
- `TOOL_SCHEMA` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L33)
- `_DEFINITION_LIKE_TYPES` — [`L706`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L706)
- `_DEFINITION_LINE_PREFIXES` — [`L739`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L739)
- `_DEF_LIMIT` — [`L66`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L66)
- `_DOWNSTREAM_LIMIT` — [`L68`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L68)
- `_HIER_LIMIT` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L71)
- `_K3_FALLBACK_EXCLUDE` — [`L1033`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L1033)
- `_K3_FALLBACK_EXTS` — [`L1012`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L1012)
- `_REF_LIMIT` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L67)
- `_RISK_TO_VERDICT` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L79)
- `_TEST_LIMIT` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L70)
- `_UPSTREAM_LIMIT` — [`L69`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L69)
- `logger` — [`L31`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/mcp/tools/symbol_lineage_tool.py#L31)

