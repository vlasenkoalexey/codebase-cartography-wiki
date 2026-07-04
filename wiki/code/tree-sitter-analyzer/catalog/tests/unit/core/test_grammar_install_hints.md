---
title: 'Module: tests/unit/core/test_grammar_install_hints.py'
type: catalog
provenance: extracted
module: tests/unit/core/test_grammar_install_hints.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.core.test_grammar_install_hints`/Test
symbols:
  TestParserErrorMessageCarriesHint.test_parse_code_error_message_contains_hint_for_grammar_missing: ParserErrorMessageCarriesHint#test_parse_code_error_message_contains_hint_for_grammar_missing().
  TestGrammarInstallHint.test_all_loader_languages_have_a_hint: GrammarInstallHint#test_all_loader_languages_have_a_hint().
  TestGrammarInstalledField.test_installed_false_for_missing_grammar: GrammarInstalledField#test_installed_false_for_missing_grammar().
  TestGrammarInstalledField.test_install_hint_field_present_for_missing_grammar: GrammarInstalledField#test_install_hint_field_present_for_missing_grammar().
  TestGrammarInstalledField.test_text_output_marks_not_installed: GrammarInstalledField#test_text_output_marks_not_installed().
  TestGrammarInstalledField.test_json_output_has_installed_field: GrammarInstalledField#test_json_output_has_installed_field().
  TestGrammarInstalledField.test_installed_true_for_available_grammar: GrammarInstalledField#test_installed_true_for_available_grammar().
  TestGrammarInstalledField.patched_find_spec: GrammarInstalledField#patched_find_spec().
  TestGrammarInstallHint.test_swift_hint_contains_extras_name: GrammarInstallHint#test_swift_hint_contains_extras_name().
  TestGrammarInstallHint.test_kotlin_hint_contains_extras_name: GrammarInstallHint#test_kotlin_hint_contains_extras_name().
  TestGrammarInstallHint.test_python_hint_contains_extras_name: GrammarInstallHint#test_python_hint_contains_extras_name().
  TestGrammarInstallHint.test_unknown_language_hint_is_none: GrammarInstallHint#test_unknown_language_hint_is_none().
  TestGrammarInstallHint.test_hint_format_uses_tree_sitter_analyzer_bracket: GrammarInstallHint#test_hint_format_uses_tree_sitter_analyzer_bracket().
  TestGrammarInstallHint.test_rust_hint_format: GrammarInstallHint#test_rust_hint_format().
  TestGrammarInstallHint.test_go_hint_format: GrammarInstallHint#test_go_hint_format().
  TestGrammarInstallHint.test_csharp_hint_format: GrammarInstallHint#test_csharp_hint_format().
  TestParserErrorMessageCarriesHint.test_parse_code_error_message_contains_hint_for_grammar_missing.FakeLoader: ParserErrorMessageCarriesHint#test_parse_code_error_message_contains_hint_for_grammar_missing().FakeLoader#
  TestGrammarInstallHint: GrammarInstallHint#
  TestGrammarInstalledField: GrammarInstalledField#
  TestParserErrorMessageCarriesHint: ParserErrorMessageCarriesHint#
  ? TestParserErrorMessageCarriesHint.test_parse_code_error_message_contains_hint_for_grammar_missing.FakeLoader.is_language_available
  : ParserErrorMessageCarriesHint#test_parse_code_error_message_contains_hint_for_grammar_missing().FakeLoader#is_language_available().
  ? TestParserErrorMessageCarriesHint.test_parse_code_error_message_contains_hint_for_grammar_missing.FakeLoader.create_parser_safely
  : ParserErrorMessageCarriesHint#test_parse_code_error_message_contains_hint_for_grammar_missing().FakeLoader#create_parser_safely().
  ? TestParserErrorMessageCarriesHint.test_parse_code_error_message_contains_hint_for_grammar_missing.FakeLoader.LANGUAGE_MODULES
  : ParserErrorMessageCarriesHint#test_parse_code_error_message_contains_hint_for_grammar_missing().FakeLoader#LANGUAGE_MODULES.
---
# Module: [`tests/unit/core/test_grammar_install_hints.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py)

## Classes
### `FakeLoader`
- def: [`tests/unit/core/test_grammar_install_hints.py:231`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L231)
- signature: `class FakeLoader:`
- members:
  - `create_parser_safely(self, lang)` — [`L235`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L235)
  - `is_language_available(self, lang)` — [`L232`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L232)
  - `LANGUAGE_MODULES` — [`L238`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L238)
- used by: (1 test-only callers)

### `TestGrammarInstallHint`
- def: [`tests/unit/core/test_grammar_install_hints.py:19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L19)
- doc: Leg 1: grammar_install_hint() returns the correct pip-install instruction.
- signature: `class TestGrammarInstallHint:`
- members:
  - `test_all_loader_languages_have_a_hint(self)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L64) — Every language in LANGUAGE_MODULES must have a hint (extras or package).
  - `test_csharp_hint_format(self)` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L59)
  - `test_go_hint_format(self)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L55)
  - `test_hint_format_uses_tree_sitter_analyzer_bracket(self)` — [`L46`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L46) — Hints must use the canonical 'pip install tree-sitter-analyzer[<extra>]' form.
  - `test_kotlin_hint_contains_extras_name(self)` — [`L30`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L30)
  - `test_python_hint_contains_extras_name(self)` — [`L36`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L36)
  - `test_rust_hint_format(self)` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L51)
  - `test_swift_hint_contains_extras_name(self)` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L22)
  - `test_unknown_language_hint_is_none(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L42) — A language not in LANGUAGE_MODULES has no hint.
- uses (calls/refs, reference-scoped): [`LanguageLoader`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader), [`LANGUAGE_MODULES`](../../../tree_sitter_analyzer/language_loader.md#LanguageLoader.LANGUAGE_MODULES), [`grammar_install_hint`](../../../tree_sitter_analyzer/language_loader.md#grammar_install_hint)

### `TestGrammarInstalledField`
- def: [`tests/unit/core/test_grammar_install_hints.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L75)
- doc: Leg 2: ShowLanguagesCommand adds installed: bool to each language entry.
- signature: `class TestGrammarInstalledField:`
- members:
  - `patched_find_spec(name, *args, **kwargs)` — [`L129`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L129)
  - `test_install_hint_field_present_for_missing_grammar(self)` — [`L151`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L151) — Entries with installed=False must also carry an 'install_hint' key.
  - `test_installed_false_for_missing_grammar(self)` — [`L118`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L118) — Languages whose grammar module is not importable must have installed=False.
  - `test_installed_true_for_available_grammar(self)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L98) — Languages whose grammar module is importable must have installed=True.
  - `test_json_output_has_installed_field(self)` — [`L78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L78) — Each language dict in the JSON envelope must have an 'installed' key.
  - `test_text_output_marks_not_installed(self)` — [`L185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L185) — Text output must visually flag languages whose grammar is missing.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowLanguagesCommand.execute), [`ShowLanguagesCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowLanguagesCommand)

### `TestParserErrorMessageCarriesHint`
- def: [`tests/unit/core/test_grammar_install_hints.py:220`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L220)
- doc: Leg 1: parser.parse_code returns an error message with pip install hint
- signature: `class TestParserErrorMessageCarriesHint:`
- members:
  - `test_parse_code_error_message_contains_hint_for_grammar_missing(self)` — [`L224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/core/test_grammar_install_hints.py#L224) — When grammar module is absent, error_message must contain install hint.
- uses (calls/refs, reference-scoped): [`Parser`](../../../tree_sitter_analyzer/core/parser.md#Parser), [`parse_code`](../../../tree_sitter_analyzer/core/parser.md#Parser.parse_code), [`success`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.success), [`error_message`](../../../tree_sitter_analyzer/core/parser.md#ParseResult.error_message), [`_loader`](../../../tree_sitter_analyzer/core/parser.md#Parser._loader), [`_encoding_manager`](../../../tree_sitter_analyzer/core/parser.md#Parser._encoding_manager)  (1 test-only)

