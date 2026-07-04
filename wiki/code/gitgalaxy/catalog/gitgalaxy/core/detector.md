---
title: 'Module: gitgalaxy/core/detector.py'
type: catalog
provenance: extracted
module: gitgalaxy/core/detector.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.core.detector`/
symbols:
  StructuralExtractor: StructuralExtractor#
  StructuralExtractor.splice: StructuralExtractor#splice().
  StructuralExtractor._function_slice: StructuralExtractor#_function_slice().
  StructuralExtractor._slice_by_keywords: StructuralExtractor#_slice_by_keywords().
  StructuralExtractor.raw_content_lines: StructuralExtractor#raw_content_lines.
  StructuralExtractor.languages: StructuralExtractor#languages.
  StructuralExtractor._calculate_block_metrics: StructuralExtractor#_calculate_block_metrics().
  StructuralExtractor.logger: StructuralExtractor#logger.
  StructuralExtractor._slice_by_terminator: StructuralExtractor#_slice_by_terminator().
  StructuralExtractor._slice_by_braces: StructuralExtractor#_slice_by_braces().
  StructuralExtractor.HANDSHAKE_LOOKAHEAD_LIMIT: StructuralExtractor#HANDSHAKE_LOOKAHEAD_LIMIT.
  StructuralExtractor.coding_analysis: StructuralExtractor#coding_analysis().
  HAS_TIKTOKEN: HAS_TIKTOKEN.
  StructuralExtractor._slice_by_labels: StructuralExtractor#_slice_by_labels().
  StructuralExtractor._slice_by_indentation: StructuralExtractor#_slice_by_indentation().
  StructuralExtractor.primary_rules: StructuralExtractor#primary_rules.
  get_token_mass: get_token_mass().
  StructuralExtractor.primary_lang_id: StructuralExtractor#primary_lang_id.
  StructuralExtractor._extract_name: StructuralExtractor#_extract_name().
  StructuralExtractor.comment_analysis: StructuralExtractor#comment_analysis().
  StructuralExtractor._extract_semantic_name: StructuralExtractor#_extract_semantic_name().
  FunctionNode: FunctionNode#
  StructuralExtractor._correlate_signals: StructuralExtractor#_correlate_signals().
  StructuralExtractor._apply_literal_shield: StructuralExtractor#_apply_literal_shield().
  StructuralExtractor._partition_segments: StructuralExtractor#_partition_segments().
  ScopeParsingRegistry.get_config: ScopeParsingRegistry#get_config().
  StructuralExtractor._find_balanced_end: StructuralExtractor#_find_balanced_end().
  StructuralExtractor.preserve_newlines: StructuralExtractor#preserve_newlines().
  ScopeParsingRegistry: ScopeParsingRegistry#
  StructuralExtractor._decode_comment_stream: StructuralExtractor#_decode_comment_stream().
  StructuralExtractor.MAX_SATELLITES: StructuralExtractor#MAX_SATELLITES.
  StructuralExtractor.MAX_DEPTH: StructuralExtractor#MAX_DEPTH.
  ScopeParsingRegistry._ALIASES: ScopeParsingRegistry#_ALIASES.
  StructuralExtractor.index_aligned_shield: StructuralExtractor#index_aligned_shield().
  ScopeParsingRegistry.get_mode: ScopeParsingRegistry#get_mode().
  StructuralExtractor.UNIVERSAL_METRICS_SCHEMA: StructuralExtractor#UNIVERSAL_METRICS_SCHEMA.
  StructuralExtractor._extract_documentation_tether: StructuralExtractor#_extract_documentation_tether().
  LogicData.functions: LogicData#functions.
  StructuralExtractor.assembly_returns: StructuralExtractor#assembly_returns.
  StructuralExtractor.CORE_MAPPING: StructuralExtractor#CORE_MAPPING.
  ENCODER: ENCODER.
  ScopeParsingRegistry.DEFINITIONS: ScopeParsingRegistry#DEFINITIONS.
  StructuralExtractor.HANDSHAKE_REGISTRY: StructuralExtractor#HANDSHAKE_REGISTRY.
  StructuralExtractor.primary_family: StructuralExtractor#primary_family.
  StructuralExtractor.fast_shield: StructuralExtractor#fast_shield().
  StructuralExtractor._classify_function: StructuralExtractor#_classify_function().
  FunctionNode.name: FunctionNode#name.
  FunctionNode.semantic_type: FunctionNode#semantic_type.
  FunctionNode.type_id: FunctionNode#type_id.
  FunctionNode.loc: FunctionNode#loc.
  FunctionNode.coding_loc: FunctionNode#coding_loc.
  FunctionNode.keyword_density: FunctionNode#keyword_density.
  FunctionNode.branch_count: FunctionNode#branch_count.
  FunctionNode.branch: FunctionNode#branch.
  FunctionNode.args: FunctionNode#args.
  FunctionNode.args_count: FunctionNode#args_count.
  FunctionNode.control_flow_angle: FunctionNode#control_flow_angle.
  FunctionNode.angle: FunctionNode#angle.
  FunctionNode.control_flow_ratio: FunctionNode#control_flow_ratio.
  FunctionNode.cf_ratio: FunctionNode#cf_ratio.
  FunctionNode.structural_weight: FunctionNode#structural_weight.
  FunctionNode.mag: FunctionNode#mag.
  FunctionNode.impact: FunctionNode#impact.
  FunctionNode.start_line: FunctionNode#start_line.
  FunctionNode.end_line: FunctionNode#end_line.
  FunctionNode.big_o_depth: FunctionNode#big_o_depth.
  FunctionNode.is_recursive: FunctionNode#is_recursive.
  FunctionNode.db_complexity: FunctionNode#db_complexity.
  FunctionNode.docstring: FunctionNode#docstring.
  FunctionNode.calls_out_to: FunctionNode#calls_out_to.
  FunctionNode.hit_vector: FunctionNode#hit_vector.
  FunctionNode.token_mass: FunctionNode#token_mass.
  LogicData: LogicData#
  LogicData.equations: LogicData#equations.
  LogicData.logic_density: LogicData#logic_density.
  LogicData.total_functional_impact: LogicData#total_functional_impact.
  LogicData.total_control_flow_ratio: LogicData#total_control_flow_ratio.
  LogicData.raw_imports: LogicData#raw_imports.
  LogicData.metadata: LogicData#metadata.
  LogicData.token_mass: LogicData#token_mass.
  LogicData.financial_read_cost: LogicData#financial_read_cost.
  StructuralExtractor.__init__: StructuralExtractor#__init__().
---
# Module: [`gitgalaxy/core/detector.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py)

## Classes
### `FunctionNode`  ·  implements/extends _TypedDict
- def: [`gitgalaxy/core/detector.py:44`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L44) — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
- doc: Metadata for a surgically extracted functional logic block.
- signature: `class FunctionNode(TypedDict, total=False):`
- members:
  - `angle` — [`L64`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L64)
  - `args` — [`L60`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L60)
  - `args_count` — [`L61`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L61)
  - `big_o_depth` — [`L76`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L76)
  - `branch` — [`L58`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L58)
  - `branch_count` — [`L57`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L57)
  - `calls_out_to` — [`L80`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L80)
  - `cf_ratio` — [`L67`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L67)
  - `coding_loc` — [`L54`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L54)
  - `control_flow_angle` — [`L63`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L63)
  - `control_flow_ratio` — [`L66`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L66)
  - `db_complexity` — [`L78`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L78)
  - `docstring` — [`L79`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L79)
  - `end_line` — [`L74`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L74)
  - `hit_vector` — [`L81`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L81)
  - `impact` — [`L71`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L71)
  - `is_recursive` — [`L77`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L77)
  - `keyword_density` — [`L55`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L55)
  - `loc` — [`L53`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L53)
  - `mag` — [`L70`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L70)
  - `name` — [`L47`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L47)
  - `semantic_type` — [`L50`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L50)
  - `start_line` — [`L73`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L73)
  - `structural_weight` — [`L69`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L69)
  - `token_mass` — [`L82`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L82)
  - `type_id` — [`L51`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L51)
- used by: [`_function_slice`](detector.md#StructuralExtractor._function_slice), [`_slice_by_keywords`](detector.md#StructuralExtractor._slice_by_keywords), [`_calculate_block_metrics`](detector.md#StructuralExtractor._calculate_block_metrics), [`_slice_by_terminator`](detector.md#StructuralExtractor._slice_by_terminator), [`_slice_by_braces`](detector.md#StructuralExtractor._slice_by_braces), [`_slice_by_indentation`](detector.md#StructuralExtractor._slice_by_indentation), [`_slice_by_labels`](detector.md#StructuralExtractor._slice_by_labels), [`functions`](detector.md#LogicData.functions)

### `LogicData`  ·  implements/extends _TypedDict
- def: [`gitgalaxy/core/detector.py:85`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L85)
- doc: The standardized output schema for Strategy v6.2.0+ compliance.
- signature: `class LogicData(TypedDict, total=False):`
- members:
  - `equations` — [`L88`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L88)
  - `financial_read_cost` — [`L96`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L96)
  - `functions` — [`L89`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L89)
  - `logic_density` — [`L90`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L90)
  - `metadata` — [`L94`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L94)
  - `raw_imports` — [`L93`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L93)
  - `token_mass` — [`L95`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L95)
  - `total_control_flow_ratio` — [`L92`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L92)
  - `total_functional_impact` — [`L91`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L91)
- uses (calls/refs, reference-scoped): [`FunctionNode`](detector.md#FunctionNode)

### `ScopeParsingRegistry`
- def: [`gitgalaxy/core/detector.py:104`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L104)
- doc: The Structural Signature Calibration Matrix for GalaxyScope's Primary Detector.
- signature: `class ScopeParsingRegistry:`
- members:
  - `get_config(cls, lang_id: str)` — [`L230`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L230) — Resolves aliases and returns the structural signature config for the language. — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `get_mode(cls, lang_id: str)` — [`L239`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L239) — Returns the specific integration mode required for the language.
  - `DEFINITIONS` — [`L132`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L132)
- protocol/private: `_ALIASES`[`L119`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L119)
- used by: [`_function_slice`](detector.md#StructuralExtractor._function_slice), [`_slice_by_keywords`](detector.md#StructuralExtractor._slice_by_keywords), [`_slice_by_terminator`](detector.md#StructuralExtractor._slice_by_terminator), [`_extract_semantic_name`](detector.md#StructuralExtractor._extract_semantic_name)

### `StructuralExtractor`
- def: [`gitgalaxy/core/detector.py:250`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L250) — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
- doc: GitGalaxy Structural Extractor (Primary Heuristic Logic & Function Mapper).
- signature: `class StructuralExtractor:`
- members:
  - `_apply_literal_shield(self, text: str, lang_id: str = None)` — [`L1060`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1060) — The Smarter Atomic Literal Shield: Handles C++ Raw Strings, Python Triple Quotes, — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_calculate_block_metrics(self, name: str, block: str, loc: int, start_line: int, end_line: int, rules: Dict[str, Any], start_idx: int = 0, end_idx: int = 0, spatial_map: Dict[str, List[int]] = None)` — [`L1859`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1859) — Calculates the structural weight, algorithmic complexity, and hit vector — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_correlate_signals(self, targets: List[int], dampeners: List[int], max_distance: int = 500)` — [`L809`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L809) — Sweeps two sorted lists of indices to find how many targets are within
  - `_extract_documentation_tether(self, start_line: int, lang_id: str)` — [`L678`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L678) — Surgically extracts the human intent (docstring/comments) using exact spatial coordinates.
  - `_extract_name(self, raw_match: str)` — [`L2115`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L2115) — Heuristic Token Normalizer. — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_extract_semantic_name(self, line: str, lang_id: str)` — [`L1145`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1145) — Safely extracts function/block names for Mode D logic. — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_find_balanced_end(self, safe_text: str, start_pos: int, opener: str, closer: str)` — [`L772`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L772) — C-Optimized jump-tracking algorithm.
  - `_function_slice(self, segments: List[Tuple[str, str, int]], segment_spatial_maps: List[Dict[str, List[int]]], regex_telemetry: dict = None)` — [`L1180`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1180) — The Master Routing Dispatcher: Directs the structural signal into the correct integration mode. — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_partition_segments(self, content: str, primary_id: str)` — [`L723`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L723) — Splits content into language segments based on handshake triggers.
  - `_slice_by_braces(self, code: str, lang_id: str, rules: Dict[str, Any], offset: int, spatial_map: Dict[str, List[int]], family: str = "c_style_comment")` — [`L1324`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1324) — [INTEGRATION MODE B] - Global Recursive Scope Analysis (C-Family & Lisp). — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_slice_by_indentation(self, code: str, rules: Dict[str, Any], offset: int, spatial_map: Dict[str, List[int]])` — [`L1457`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1457) — [INTEGRATION MODE C] - Density Stratification (Python, YAML). — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_slice_by_keywords(self, code: str, lang_id: str, rules: Dict[str, Any], offset: int, spatial_map: Dict[str, List[int]])` — [`L1578`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1578) — [INTEGRATION MODE D] - Semantic Handshake Stack (Shell, Ruby, Lua). — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_slice_by_labels(self, code: str, rules: Dict[str, Any], offset: int, spatial_map: Dict[str, List[int]])` — [`L1250`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1250) — [INTEGRATION MODE A] - Greedy Label-Based Scan (Assembly, COBOL). — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `_slice_by_terminator(self, code: str, lang_id: str, rules: Dict[str, Any], offset: int, spatial_map: Dict[str, List[int]])` — [`L1736`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1736) — [INTEGRATION MODE E] - Terminator Cleaving (SQL, Erlang, Prolog). — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `coding_analysis(self, segments: List[Tuple[str, str, int]], regex_telemetry: dict = None)` — [`L838`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L838)
  - `comment_analysis(self, comment_stream: str, lang_id: str, counts: Dict[str, int])` — [`L1017`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1017) — Analyzes the comment stream for developer intent, technical debt, and traceability.
  - `fast_shield(m)` — [`L1353`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1353)
  - `index_aligned_shield(m)` — [`L1474`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1474)
  - `preserve_newlines(m)` — [`L1070`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L1070)
  - `splice(self, code_stream: str, comment_stream: str, confidence: float = 1, profile_regex: bool = False, raw_content: str = "")` — [`L347`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L347) — Executes the structural regex pass over refracted code streams. — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `CORE_MAPPING` — [`L320`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L320)
  - `HANDSHAKE_LOOKAHEAD_LIMIT` — [`L331`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L331) — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `HANDSHAKE_REGISTRY` — [`L274`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L274)
  - `MAX_DEPTH` — [`L330`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L330)
  - `MAX_SATELLITES` — [`L329`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L329)
  - `UNIVERSAL_METRICS_SCHEMA` — [`L272`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L272) — documented in [gitgalaxy-standards-analysis_lens](../../../concepts/gitgalaxy-standards-analysis_lens.md)
  - `assembly_returns` — [`L315`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L315)
  - `languages` — [`L309`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L309) — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `logger` — [`L302`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L302)
  - `primary_family` — [`L313`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L313)
  - `primary_lang_id` — [`L308`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L308) — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
  - `primary_rules` — [`L312`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L312)
  - `raw_content_lines` — [`L356`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L356) — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)
- protocol/private: `__init__`[`L295`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L295), `_classify_function`[`L2181`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L2181), `_decode_comment_stream`[`L572`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L572)
- uses (calls/refs, reference-scoped): [`LANGUAGE_DEFINITIONS`](../standards/language_standards.md#LANGUAGE_DEFINITIONS), [`get_token_mass`](detector.md#get_token_mass), [`RECORDING_SCHEMAS`](../standards/analysis_lens.md#RECORDING_SCHEMAS), [`FunctionNode`](detector.md#FunctionNode), [`get_config`](detector.md#ScopeParsingRegistry.get_config), [`ScopeParsingRegistry`](detector.md#ScopeParsingRegistry), [`_ALIASES`](detector.md#ScopeParsingRegistry._ALIASES), [`get_mode`](detector.md#ScopeParsingRegistry.get_mode)
- used by: [`_init_worker`](../galaxyscope.md#_init_worker)  (46 test-only)

## Functions
- `get_token_mass(text: str, deep_scan: bool = False)` — [`L29`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L29) — Calculates context window footprint. Returns None if tiktoken is missing to prevent dataset poisoning. — documented in [gitgalaxy-core-detector](../../../concepts/gitgalaxy-core-detector.md)

## Module values
- `ENCODER` — [`L24`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L24)
- `HAS_TIKTOKEN` — [`L18`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/detector.py#L18) — documented in [gitgalaxy-galaxyscope](../../../concepts/gitgalaxy-galaxyscope.md)

