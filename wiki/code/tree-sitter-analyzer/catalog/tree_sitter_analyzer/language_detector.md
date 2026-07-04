---
title: 'Module: tree_sitter_analyzer/language_detector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/language_detector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.language_detector`/
symbols:
  detect_language_from_file: detect_language_from_file().
  LanguageDetector.detect_from_extension: LanguageDetector#detect_from_extension().
  detector: detector.
  LanguageDetector.detect_language: LanguageDetector#detect_language().
  LanguageDetector: LanguageDetector#
  is_language_supported: is_language_supported().
  LanguageDetector.is_supported: LanguageDetector#is_supported().
  LanguageDetector._resolve_ambiguity: LanguageDetector#_resolve_ambiguity().
  LanguageDetector.content_patterns: LanguageDetector#content_patterns.
  LanguageDetector.get_language_info: LanguageDetector#get_language_info().
  LanguageDetector._detect_mapped_extension: LanguageDetector#_detect_mapped_extension().
  LanguageDetector.EXTENSION_MAPPING: LanguageDetector#EXTENSION_MAPPING.
  LanguageDetector.get_supported_extensions: LanguageDetector#get_supported_extensions().
  LanguageDetector.get_supported_languages: LanguageDetector#get_supported_languages().
  LanguageDetector.CONTENT_PATTERNS: LanguageDetector#CONTENT_PATTERNS.
  LanguageDetector.SUPPORTED_LANGUAGES: LanguageDetector#SUPPORTED_LANGUAGES.
  LanguageDetector.extension_map: LanguageDetector#extension_map.
  LanguageDetector._detect_c_family: LanguageDetector#_detect_c_family().
  LanguageDetector.add_extension_mapping: LanguageDetector#add_extension_mapping().
  LanguageDetector._detect_objc_vs_matlab: LanguageDetector#_detect_objc_vs_matlab().
  LanguageDetector.AMBIGUOUS_EXTENSIONS: LanguageDetector#AMBIGUOUS_EXTENSIONS.
  LanguageDetector._log_debug: LanguageDetector#_log_debug.
  LanguageDetector._log_warning: LanguageDetector#_log_warning.
  LanguageDetector.get_all_known_extensions: LanguageDetector#get_all_known_extensions().
  LanguageDetector.__init__: LanguageDetector#__init__().
---
# Module: [`tree_sitter_analyzer/language_detector.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py)

## Classes
### `LanguageDetector`
- def: [`tree_sitter_analyzer/language_detector.py:22`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L22)
- doc: Automatic programming language detector
- signature: `class LanguageDetector:`
- members:
  - `__init__(self)` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L152) — Initialize detector
  - `_detect_c_family(self, content: str, candidates: list[str])` — [`L333`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L333) — Detect among C-family languages
  - `_detect_objc_vs_matlab(self, content: str, candidates: list[str])` — [`L367`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L367) — Detect between Objective-C and MATLAB
  - `_resolve_ambiguity(self, extension: str, content: str)` — [`L306`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L306) — Resolve ambiguous extension using content
  - `add_extension_mapping(self, extension: str, language: str)` — [`L389`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L389) — Add custom extension mapping
  - `detect_from_extension(self, file_path: str)` — [`L214`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L214) — Quick detection using extension only
  - `detect_language(self, file_path: str, content: str | None = None)` — [`L162`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L162) — ファイルパスとコンテンツから言語を判定
  - `get_all_known_extensions(self)` — [`L282`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L282) — Get every extension recognised by the detector, even if its language
  - `get_language_info(self, language: str)` — [`L399`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L399) — Get language information
  - `get_supported_extensions(self)` — [`L262`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L262) — Get list of supported file extensions.
  - `get_supported_languages(self)` — [`L297`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L297) — Get list of supported languages
  - `is_supported(self, language: str)` — [`L236`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L236) — Check if language is supported by Tree-sitter
  - `AMBIGUOUS_EXTENSIONS` — [`L107`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L107)
  - `CONTENT_PATTERNS` — [`L116`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L116)
  - `EXTENSION_MAPPING` — [`L26`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L26)
  - `SUPPORTED_LANGUAGES` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L128)
  - `_log_debug` — [`L159`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L159) — ---
  - `_log_warning` — [`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L160) — ---
  - `content_patterns` — [`L155`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L155)
  - `extension_map` — [`L154`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L154)
- protocol/private: `_detect_mapped_extension`[`L189`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L189)
- uses (calls/refs, reference-scoped): [`log_debug`](utils/logging.md#log_debug), [`log_warning`](utils/logging.md#log_warning), [`PluginManager`](plugins/manager.md#PluginManager), [`load_plugins`](plugins/manager.md#PluginManager.load_plugins), [`get_supported_languages`](plugins/manager.md#PluginManager.get_supported_languages), [`build_content_pattern_weights`](_language_detector_helpers.md#build_content_pattern_weights), [`build_extension_confidence_map`](_language_detector_helpers.md#build_extension_confidence_map)
- used by: [`detect_language_from_file`](language_detector.md#detect_language_from_file), [`detector`](language_detector.md#detector), [`_ensure_initialized`](core/analysis_engine.md#UnifiedAnalysisEngine._ensure_initialized), [`is_language_supported`](language_detector.md#is_language_supported), [`execute`](cli/info_commands.md#ShowLanguagesCommand.execute), [`_parse`](ast_path.md#ASTPathNavigator._parse), [`execute`](cli/info_commands.md#ShowExtensionsCommand.execute), [`language_from_path`](_language_family.md#language_from_path), [`_get_extensions_for_language`](mcp/tools/trace_impact_tool.md#TraceImpactTool._get_extensions_for_language), [`_build_language_entry`](cli/info_commands.md#ShowLanguagesCommand._build_language_entry), [`language_detector`](mcp/tools/trace_impact_tool.md#TraceImpactTool.language_detector), [`_detector`](ast_path.md#ASTPathNavigator._detector)  (99 test-only)

## Functions
- `detect_language_from_file(file_path: str, *, project_root: str | None = None)` — [`L425`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L425) — Detect language from path (simple API) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
- `is_language_supported(language: str)` — [`L467`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L467) — Check if language is supported (simple API) — documented in [tree_sitter_analyzer-plugins-manager](../../concepts/tree_sitter_analyzer-plugins-manager.md)

## Module values
- `detector` — [`L422`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/language_detector.py#L422)

