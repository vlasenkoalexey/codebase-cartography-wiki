---
title: 'Module: tests/unit/formatters/test_toon_roundtrip.py'
type: catalog
provenance: extracted
module: tests/unit/formatters/test_toon_roundtrip.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.formatters.test_toon_roundtrip`/Test
symbols:
  TestToonRoundTrip._rt: ToonRoundTrip#_rt().
  TestAmbiguousStringQuoting.enc: AmbiguousStringQuoting#enc.
  TestAmbiguousStringQuoting.test_string_true_is_quoted: AmbiguousStringQuoting#test_string_true_is_quoted().
  TestAmbiguousStringQuoting.test_string_false_is_quoted: AmbiguousStringQuoting#test_string_false_is_quoted().
  TestAmbiguousStringQuoting.test_string_null_is_quoted: AmbiguousStringQuoting#test_string_null_is_quoted().
  TestAmbiguousStringQuoting.test_string_integer_positive_is_quoted: AmbiguousStringQuoting#test_string_integer_positive_is_quoted().
  TestAmbiguousStringQuoting.test_string_integer_zero_is_quoted: AmbiguousStringQuoting#test_string_integer_zero_is_quoted().
  TestAmbiguousStringQuoting.test_string_integer_negative_is_quoted: AmbiguousStringQuoting#test_string_integer_negative_is_quoted().
  TestAmbiguousStringQuoting.test_string_float_is_quoted: AmbiguousStringQuoting#test_string_float_is_quoted().
  TestAmbiguousStringQuoting.test_string_float_no_leading_digit_is_quoted: AmbiguousStringQuoting#test_string_float_no_leading_digit_is_quoted().
  TestAmbiguousStringQuoting.test_string_negative_float_is_quoted: AmbiguousStringQuoting#test_string_negative_float_is_quoted().
  TestAmbiguousStringQuoting.test_string_scientific_upper_is_quoted: AmbiguousStringQuoting#test_string_scientific_upper_is_quoted().
  TestAmbiguousStringQuoting.test_string_scientific_lower_is_quoted: AmbiguousStringQuoting#test_string_scientific_lower_is_quoted().
  TestAmbiguousStringQuoting.test_string_scientific_negative_exp_is_quoted: AmbiguousStringQuoting#test_string_scientific_negative_exp_is_quoted().
  TestAmbiguousStringQuoting.test_bool_true_stays_bare: AmbiguousStringQuoting#test_bool_true_stays_bare().
  TestAmbiguousStringQuoting.test_bool_false_stays_bare: AmbiguousStringQuoting#test_bool_false_stays_bare().
  TestAmbiguousStringQuoting.test_none_stays_bare: AmbiguousStringQuoting#test_none_stays_bare().
  TestAmbiguousStringQuoting.test_int_stays_bare: AmbiguousStringQuoting#test_int_stays_bare().
  TestAmbiguousStringQuoting.test_float_stays_bare: AmbiguousStringQuoting#test_float_stays_bare().
  TestAmbiguousStringQuoting.test_ordinary_word_stays_bare: AmbiguousStringQuoting#test_ordinary_word_stays_bare().
  TestAmbiguousStringQuoting.test_mixed_alphanum_stays_bare: AmbiguousStringQuoting#test_mixed_alphanum_stays_bare().
  TestAmbiguousStringQuoting.test_dict_with_scalar_ambiguous_string_values: AmbiguousStringQuoting#test_dict_with_scalar_ambiguous_string_values().
  TestAmbiguousStringQuoting.setup_method: AmbiguousStringQuoting#setup_method().
  TestToonDecoder.test_decode_null: ToonDecoder#test_decode_null().
  TestToonDecoder.test_decode_true: ToonDecoder#test_decode_true().
  TestToonDecoder.test_decode_false: ToonDecoder#test_decode_false().
  TestToonDecoder.test_decode_integer: ToonDecoder#test_decode_integer().
  TestToonDecoder.test_decode_negative_integer: ToonDecoder#test_decode_negative_integer().
  TestToonDecoder.test_decode_float: ToonDecoder#test_decode_float().
  TestToonDecoder.test_decode_quoted_true_gives_str: ToonDecoder#test_decode_quoted_true_gives_str().
  TestToonDecoder.test_decode_quoted_false_gives_str: ToonDecoder#test_decode_quoted_false_gives_str().
  TestToonDecoder.test_decode_quoted_null_gives_str: ToonDecoder#test_decode_quoted_null_gives_str().
  TestToonDecoder.test_decode_quoted_number_gives_str: ToonDecoder#test_decode_quoted_number_gives_str().
  TestToonDecoder.test_decode_quoted_string: ToonDecoder#test_decode_quoted_string().
  TestToonDecoder.test_decode_quoted_string_with_escape_sequences: ToonDecoder#test_decode_quoted_string_with_escape_sequences().
  TestToonDecoder.test_decode_quoted_string_with_tab: ToonDecoder#test_decode_quoted_string_with_tab().
  TestToonDecoder.test_decode_quoted_string_with_escaped_quote: ToonDecoder#test_decode_quoted_string_with_escaped_quote().
  TestToonDecoder.test_decode_bare_word_gives_str: ToonDecoder#test_decode_bare_word_gives_str().
  TestToonRoundTrip.test_none_roundtrip: ToonRoundTrip#test_none_roundtrip().
  TestToonRoundTrip.test_true_roundtrip: ToonRoundTrip#test_true_roundtrip().
  TestToonRoundTrip.test_false_roundtrip: ToonRoundTrip#test_false_roundtrip().
  TestToonRoundTrip.test_zero_roundtrip: ToonRoundTrip#test_zero_roundtrip().
  TestToonRoundTrip.test_positive_int_roundtrip: ToonRoundTrip#test_positive_int_roundtrip().
  TestToonRoundTrip.test_negative_int_roundtrip: ToonRoundTrip#test_negative_int_roundtrip().
  TestToonRoundTrip.test_float_roundtrip: ToonRoundTrip#test_float_roundtrip().
  TestToonRoundTrip.test_negative_float_roundtrip: ToonRoundTrip#test_negative_float_roundtrip().
  TestToonRoundTrip.test_str_true_roundtrip: ToonRoundTrip#test_str_true_roundtrip().
  TestToonRoundTrip.test_str_false_roundtrip: ToonRoundTrip#test_str_false_roundtrip().
  TestToonRoundTrip.test_str_null_roundtrip: ToonRoundTrip#test_str_null_roundtrip().
  TestToonRoundTrip.test_str_integer_roundtrip: ToonRoundTrip#test_str_integer_roundtrip().
  TestToonRoundTrip.test_str_float_roundtrip: ToonRoundTrip#test_str_float_roundtrip().
  TestToonRoundTrip.test_str_negative_int_roundtrip: ToonRoundTrip#test_str_negative_int_roundtrip().
  TestToonRoundTrip.test_str_scientific_roundtrip: ToonRoundTrip#test_str_scientific_roundtrip().
  TestToonRoundTrip.test_ordinary_str_roundtrip: ToonRoundTrip#test_ordinary_str_roundtrip().
  TestToonRoundTrip.test_str_with_spaces_roundtrip: ToonRoundTrip#test_str_with_spaces_roundtrip().
  TestToonRoundTrip.test_str_with_special_chars_roundtrip: ToonRoundTrip#test_str_with_special_chars_roundtrip().
  TestToonRoundTrip.test_str_with_newline_roundtrip: ToonRoundTrip#test_str_with_newline_roundtrip().
  TestToonRoundTrip.test_str_with_colon_roundtrip: ToonRoundTrip#test_str_with_colon_roundtrip().
  TestAmbiguousStringQuoting: AmbiguousStringQuoting#
  TestToonDecoder: ToonDecoder#
  TestToonRoundTrip: ToonRoundTrip#
---
# Module: [`tests/unit/formatters/test_toon_roundtrip.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py)

## Classes
### `TestAmbiguousStringQuoting`
- def: [`tests/unit/formatters/test_toon_roundtrip.py:34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L34)
- doc: Strings that look like TOON/JSON scalars MUST be quoted.
- signature: `class TestAmbiguousStringQuoting:`
- members:
  - `setup_method(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L42)
  - `test_bool_false_stays_bare(self)` — [`L111`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L111)
  - `test_bool_true_stays_bare(self)` — [`L106`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L106) — Python True -> bare ``true``; it is a genuine bool scalar.
  - `test_dict_with_scalar_ambiguous_string_values(self)` — [`L139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L139) — All scalar-looking string VALUES in a dict must be quoted.
  - `test_float_stays_bare(self)` — [`L123`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L123)
  - `test_int_stays_bare(self)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L119)
  - `test_mixed_alphanum_stays_bare(self)` — [`L133`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L133)
  - `test_none_stays_bare(self)` — [`L115`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L115)
  - `test_ordinary_word_stays_bare(self)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L129)
  - `test_string_false_is_quoted(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L51)
  - `test_string_float_is_quoted(self)` — [`L77`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L77) — The exact case from #1058: "100.0" decoded as float, not str.
  - `test_string_float_no_leading_digit_is_quoted(self)` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L82)
  - `test_string_integer_negative_is_quoted(self)` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L71)
  - `test_string_integer_positive_is_quoted(self)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L63)
  - `test_string_integer_zero_is_quoted(self)` — [`L67`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L67)
  - `test_string_negative_float_is_quoted(self)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L86)
  - `test_string_null_is_quoted(self)` — [`L57`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L57)
  - `test_string_scientific_lower_is_quoted(self)` — [`L96`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L96)
  - `test_string_scientific_negative_exp_is_quoted(self)` — [`L100`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L100)
  - `test_string_scientific_upper_is_quoted(self)` — [`L92`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L92)
  - `test_string_true_is_quoted(self)` — [`L47`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L47)
  - `enc` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L43)
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode)

### `TestToonDecoder`
- def: [`tests/unit/formatters/test_toon_roundtrip.py:163`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L163)
- doc: Unit tests for the `decode_toon` function.
- signature: `class TestToonDecoder:`
- members:
  - `test_decode_bare_word_gives_str(self)` — [`L228`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L228)
  - `test_decode_false(self)` — [`L174`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L174)
  - `test_decode_float(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L187)
  - `test_decode_integer(self)` — [`L177`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L177)
  - `test_decode_negative_integer(self)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L182)
  - `test_decode_null(self)` — [`L168`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L168)
  - `test_decode_quoted_false_gives_str(self)` — [`L199`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L199)
  - `test_decode_quoted_null_gives_str(self)` — [`L204`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L204)
  - `test_decode_quoted_number_gives_str(self)` — [`L209`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L209)
  - `test_decode_quoted_string(self)` — [`L214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L214)
  - `test_decode_quoted_string_with_escape_sequences(self)` — [`L217`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L217)
  - `test_decode_quoted_string_with_escaped_quote(self)` — [`L223`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L223)
  - `test_decode_quoted_string_with_tab(self)` — [`L220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L220)
  - `test_decode_quoted_true_gives_str(self)` — [`L194`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L194)
  - `test_decode_true(self)` — [`L171`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L171)
- uses (calls/refs, reference-scoped): [`decode_toon`](../../../tree_sitter_analyzer/formatters/toon_decoder.md#decode_toon)

### `TestToonRoundTrip`
- def: [`tests/unit/formatters/test_toon_roundtrip.py:239`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L239)
- doc: Property oracle: encode then decode must recover the original Python value.
- signature: `class TestToonRoundTrip:`
- members:
  - `_rt(self, value)` — [`L248`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L248) — Encode with ToonEncoder then decode; return reconstructed value.
  - `test_false_roundtrip(self)` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L263)
  - `test_float_roundtrip(self)` — [`L286`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L286)
  - `test_negative_float_roundtrip(self)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L291)
  - `test_negative_int_roundtrip(self)` — [`L279`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L279)
  - `test_none_roundtrip(self)` — [`L256`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L256)
  - `test_ordinary_str_roundtrip(self)` — [`L336`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L336)
  - `test_positive_int_roundtrip(self)` — [`L274`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L274)
  - `test_str_false_roundtrip(self)` — [`L303`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L303)
  - `test_str_float_roundtrip(self)` — [`L318`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L318) — The exact #1058 case: "100.0" must round-trip as str, not float.
  - `test_str_integer_roundtrip(self)` — [`L313`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L313)
  - `test_str_negative_int_roundtrip(self)` — [`L324`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L324)
  - `test_str_null_roundtrip(self)` — [`L308`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L308)
  - `test_str_scientific_roundtrip(self)` — [`L329`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L329)
  - `test_str_true_roundtrip(self)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L298)
  - `test_str_with_colon_roundtrip(self)` — [`L357`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L357)
  - `test_str_with_newline_roundtrip(self)` — [`L352`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L352)
  - `test_str_with_spaces_roundtrip(self)` — [`L341`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L341) — Strings with spaces pass through bare if no structural chars.
  - `test_str_with_special_chars_roundtrip(self)` — [`L347`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L347)
  - `test_true_roundtrip(self)` — [`L259`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L259)
  - `test_zero_roundtrip(self)` — [`L269`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/formatters/test_toon_roundtrip.py#L269)
- uses (calls/refs, reference-scoped): [`ToonEncoder`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder), [`encode_value`](../../../tree_sitter_analyzer/formatters/toon_encoder.md#ToonEncoder.encode_value), [`decode_toon`](../../../tree_sitter_analyzer/formatters/toon_decoder.md#decode_toon)

