---
title: 'Module: gitgalaxy/core/prism.py'
type: catalog
provenance: extracted
module: gitgalaxy/core/prism.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.core.prism`/Prism
symbols:
  Prism._strip_segment_comments: '#_strip_segment_comments().'
  Prism.logger: '#logger.'
  Prism._strip_nested_comments: '#_strip_nested_comments().'
  Prism.split_streams: '#split_streams().'
  Prism._partition_embedded_languages: '#_partition_embedded_languages().'
  Prism.REGEX_MATRIX: '#REGEX_MATRIX.'
  Prism.PHP_MULTILINE_STRING: '#PHP_MULTILINE_STRING.'
  Prism._compile_regex_matrix: '#_compile_regex_matrix().'
  Prism._strip_php_string_mass: '#_strip_php_string_mass().'
  Prism.EMBEDDED_TRIGGERS: '#EMBEDDED_TRIGGERS.'
  Prism: '#'
  Prism._find_balanced_end: '#_find_balanced_end().'
  Prism.LITERAL_MASK_PATTERN: '#LITERAL_MASK_PATTERN.'
  Prism.NESTED_PEEL_LIMIT: '#NESTED_PEEL_LIMIT.'
  Prism.EMBEDDED_LOOKAHEAD_LIMIT: '#EMBEDDED_LOOKAHEAD_LIMIT.'
  Prism.POSITIONAL_ANCHORS: '#POSITIONAL_ANCHORS.'
  Prism.languages: '#languages.'
  Prism.PHP_HEREDOC_PATTERN: '#PHP_HEREDOC_PATTERN.'
  Prism._strip_python_docstrings: '#_strip_python_docstrings().'
  Prism.single_callback: '#single_callback().'
  Prism._strip_positional_comments: '#_strip_positional_comments().'
  Prism.unmask: '#unmask().'
  Prism.PYTHON_DOC_PATTERN: '#PYTHON_DOC_PATTERN.'
  Prism.lexical_families: '#lexical_families.'
  Prism.capture_lit: '#capture_lit().'
  PrismResult: Result#
  PrismError: Error#
  Prism.shield_callback: '#shield_callback().'
  Prism.strip_callback: '#strip_callback().'
  Prism.callback: '#callback().'
  Prism._shield_replacer: '#_shield_replacer().'
  Prism._guard_metadata_signal: '#_guard_metadata_signal().'
  Prism._strip_single_line_comments: '#_strip_single_line_comments().'
  PrismResult.code_stream: Result#code_stream.
  PrismResult.comment_stream: Result#comment_stream.
  PrismResult.coding_loc: Result#coding_loc.
  PrismResult.doc_loc: Result#doc_loc.
  Prism.__init__: '#__init__().'
---
# Module: [`gitgalaxy/core/prism.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py)

## Classes
### `Prism`
- def: [`gitgalaxy/core/prism.py:44`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L44)
- doc: GitGalaxy Phase 2: The Prism (Payload & Surface Splitter)
- signature: `class Prism:`
- members:
  - `__init__(self, comment_definitions: Dict[str, Any], language_definitions: Dict[str, Any], parent_logger: Optional[logging.Logger] = None)` — [`L65`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L65) — Initializes the Prism and pre-compiles the regex matrix.
  - `_compile_regex_matrix(self)` — [`L267`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L267) — Safely pre-compiles the standard regex matrix based on dynamic config lengths. — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_find_balanced_end(self, text: str, start_pos: int, opener: str, closer: str)` — [`L451`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L451) — Balanced scoping implementation for paired-bracket embedded segments. — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_guard_metadata_signal(self, content: str)` — [`L591`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L591) — Protects shebangs and preprocessor headers from the stripping engine. — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_partition_embedded_languages(self, content: str, primary_id: str)` — [`L379`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L379) — Splits content into language segments based on embedded language triggers. — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_strip_nested_comments(self, text: str)` — [`L492`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L492) — Iterative Peel loop for recursively nested block comments (e.g. Rust/Swift/Scala). — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_strip_php_string_mass(self, text: str)` — [`L361`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L361) — Surgically extracts PHP Heredoc and multi-line strings to prevent structural hallucinations. — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_strip_positional_comments(self, text: str)` — [`L565`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L565) — Column-anchored and Inline stripping for legacy languages (COBOL/Fortran). — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_strip_python_docstrings(self, text: str)` — [`L348`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L348) — Extracts triple-quoted strings as documentation. — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_strip_segment_comments(self, text: str, lang_id: str, family: str)` — [`L209`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L209) — Surgically strips documentation using an ordered, additive pipeline. — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `_strip_single_line_comments(self, text: str)` — [`L604`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L604) — Generic single-line comment stripper (for '#' or ';' or '--'). — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `callback(m: re.Match)` — [`L353`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L353)
  - `capture_lit(m: re.Match)` — [`L365`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L365)
  - `shield_callback(m: re.Match)` — [`L242`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L242) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `single_callback(m: re.Match)` — [`L532`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L532)
  - `split_streams(self, content: str, primary_lang: str)` — [`L117`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L117) — Decouples the file into mutually exclusive components (Executable Payload vs Documentation Surface). — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `strip_callback(m: re.Match)` — [`L255`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L255) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `unmask(chunk: str)` — [`L519`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L519)
  - `EMBEDDED_LOOKAHEAD_LIMIT` — [`L106`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L106) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `EMBEDDED_TRIGGERS` — [`L94`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L94) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `LITERAL_MASK_PATTERN` — [`L88`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L88) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `NESTED_PEEL_LIMIT` — [`L107`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L107) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `PHP_HEREDOC_PATTERN` — [`L112`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L112)
  - `PHP_MULTILINE_STRING` — [`L113`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L113)
  - `POSITIONAL_ANCHORS` — [`L108`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L108) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `PYTHON_DOC_PATTERN` — [`L111`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L111)
  - `REGEX_MATRIX` — [`L91`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L91) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
  - `languages` — [`L82`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L82)
  - `lexical_families` — [`L81`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L81)
  - `logger` — [`L75`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L75)
- protocol/private: `_shield_replacer`[`L509`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L509)
- uses (calls/refs, reference-scoped): [`LENS_CONFIG`](../standards/language_standards.md#LENS_CONFIG), [`PRISM_CONFIG`](../standards/language_standards.md#PRISM_CONFIG), [`PrismError`](prism.md#PrismError), [`PrismResult`](prism.md#PrismResult)
- used by: [`_init_worker`](../galaxyscope.md#_init_worker)  (2 test-only)

### `PrismError`  ·  implements/extends Exception
- def: [`gitgalaxy/core/prism.py:38`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L38) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
- doc: Exception raised for structural failures during the lexical scan.
- signature: `class PrismError(Exception):`
- used by: [`split_streams`](prism.md#Prism.split_streams)

### `PrismResult`  ·  implements/extends _TypedDict
- def: [`gitgalaxy/core/prism.py:21`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L21) — documented in [gitgalaxy-core-prism](../../../concepts/gitgalaxy-core-prism.md)
- doc: The dual-output of the Prism.
- signature: `class PrismResult(TypedDict):`
- members:
  - `code_stream` — [`L32`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L32)
  - `coding_loc` — [`L34`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L34)
  - `comment_stream` — [`L33`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L33)
  - `doc_loc` — [`L35`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/prism.py#L35)
- used by: [`split_streams`](prism.md#Prism.split_streams)

