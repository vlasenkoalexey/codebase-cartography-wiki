---
title: 'Module: tests/unit/cli/test_info_commands.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_info_commands.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_info_commands`/
symbols:
  TestListQueriesCommand.test_with_explicit_language: TestListQueriesCommand#test_with_explicit_language().
  TestListQueriesCommand.test_with_file_path_language_detection: TestListQueriesCommand#test_with_file_path_language_detection().
  TestListQueriesCommand.test_no_language_no_file_lists_all: TestListQueriesCommand#test_no_language_no_file_lists_all().
  TestDescribeQueryCommand.test_describe_with_explicit_language: TestDescribeQueryCommand#test_describe_with_explicit_language().
  TestDescribeQueryCommand.test_describe_no_language_no_file: TestDescribeQueryCommand#test_describe_no_language_no_file().
  TestDescribeQueryCommand.test_describe_query_not_found: TestDescribeQueryCommand#test_describe_query_not_found().
  TestDescribeQueryCommand.test_describe_query_value_error: TestDescribeQueryCommand#test_describe_query_value_error().
  TestShowLanguagesCommand.test_show_languages: TestShowLanguagesCommand#test_show_languages().
  TestShowExtensionsCommand.test_show_extensions: TestShowExtensionsCommand#test_show_extensions().
  TestR37adListQueriesJsonEnvelope.test_list_queries_json_for_specific_language: TestR37adListQueriesJsonEnvelope#test_list_queries_json_for_specific_language().
  TestR37adListQueriesJsonEnvelope.test_list_queries_json_for_all_languages: TestR37adListQueriesJsonEnvelope#test_list_queries_json_for_all_languages().
  TestR37adListQueriesJsonEnvelope.test_list_queries_text_path_preserved: TestR37adListQueriesJsonEnvelope#test_list_queries_text_path_preserved().
  TestR37aeRemainingInfoCommandsJsonEnvelope.test_describe_query_json_envelope: TestR37aeRemainingInfoCommandsJsonEnvelope#test_describe_query_json_envelope().
  TestR37aeRemainingInfoCommandsJsonEnvelope.test_describe_query_not_found_json_envelope: TestR37aeRemainingInfoCommandsJsonEnvelope#test_describe_query_not_found_json_envelope().
  TestR37aeRemainingInfoCommandsJsonEnvelope.test_show_supported_languages_json_envelope: TestR37aeRemainingInfoCommandsJsonEnvelope#test_show_supported_languages_json_envelope().
  TestR37aeRemainingInfoCommandsJsonEnvelope.test_show_supported_extensions_json_envelope: TestR37aeRemainingInfoCommandsJsonEnvelope#test_show_supported_extensions_json_envelope().
  TestR37aeRemainingInfoCommandsJsonEnvelope.test_show_languages_text_path_preserved: TestR37aeRemainingInfoCommandsJsonEnvelope#test_show_languages_text_path_preserved().
  TestInfoCommandAbstract.test_cannot_instantiate_abstract: TestInfoCommandAbstract#test_cannot_instantiate_abstract().
  TestQ3SupportedExtensionsParity.detector_instance: TestQ3SupportedExtensionsParity#detector_instance().
  args_with_language: args_with_language().
  args_no_language: args_no_language().
  args_with_file: args_with_file().
  TestInfoCommandAbstract: TestInfoCommandAbstract#
  TestListQueriesCommand: TestListQueriesCommand#
  TestDescribeQueryCommand: TestDescribeQueryCommand#
  TestShowLanguagesCommand: TestShowLanguagesCommand#
  TestShowExtensionsCommand: TestShowExtensionsCommand#
  TestQ3SupportedExtensionsParity: TestQ3SupportedExtensionsParity#
  TestQ3SupportedExtensionsParity.test_every_supported_extension_maps_to_supported_language: TestQ3SupportedExtensionsParity#test_every_supported_extension_maps_to_supported_language().
  TestQ3SupportedExtensionsParity.test_orphan_extensions_not_advertised: TestQ3SupportedExtensionsParity#test_orphan_extensions_not_advertised().
  TestQ3SupportedExtensionsParity.test_core_extensions_still_advertised: TestQ3SupportedExtensionsParity#test_core_extensions_still_advertised().
  TestQ3SupportedExtensionsParity.test_all_known_extensions_still_includes_orphans: TestQ3SupportedExtensionsParity#test_all_known_extensions_still_includes_orphans().
  TestQ3SupportedExtensionsParity.test_show_extensions_cli_advertises_scala: TestQ3SupportedExtensionsParity#test_show_extensions_cli_advertises_scala().
  TestQ3SupportedExtensionsParity.test_show_languages_cli_advertises_scala: TestQ3SupportedExtensionsParity#test_show_languages_cli_advertises_scala().
  TestR37adListQueriesJsonEnvelope: TestR37adListQueriesJsonEnvelope#
  TestR37aeRemainingInfoCommandsJsonEnvelope: TestR37aeRemainingInfoCommandsJsonEnvelope#
---
# Module: [`tests/unit/cli/test_info_commands.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py)

## Classes
### `TestDescribeQueryCommand`
- def: [`tests/unit/cli/test_info_commands.py:78`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L78)
- signature: `class TestDescribeQueryCommand:`
- members:
  - `test_describe_no_language_no_file(self, args_no_language)` — [`L91`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L91)
  - `test_describe_query_not_found(self, args_with_language)` — [`L98`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L98)
  - `test_describe_query_value_error(self, args_with_language)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L109)
  - `test_describe_with_explicit_language(self, args_with_language)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L79)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#DescribeQueryCommand.execute), [`DescribeQueryCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#DescribeQueryCommand)

### `TestInfoCommandAbstract`
- def: [`tests/unit/cli/test_info_commands.py:33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L33)
- signature: `class TestInfoCommandAbstract:`
- members:
  - `test_cannot_instantiate_abstract(self)` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L34)
- uses (calls/refs, reference-scoped): [`InfoCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#InfoCommand)

### `TestListQueriesCommand`
- def: [`tests/unit/cli/test_info_commands.py:39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L39)
- signature: `class TestListQueriesCommand:`
- members:
  - `test_no_language_no_file_lists_all(self, args_no_language)` — [`L64`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L64)
  - `test_with_explicit_language(self, args_with_language)` — [`L40`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L40)
  - `test_with_file_path_language_detection(self, args_with_file)` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L49)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#ListQueriesCommand.execute), [`ListQueriesCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#ListQueriesCommand)

### `TestQ3SupportedExtensionsParity`
- def: [`tests/unit/cli/test_info_commands.py:164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L164)
- doc: Q3 regression: --show-supported-extensions must only list extensions
- signature: `class TestQ3SupportedExtensionsParity:`
- members:
  - `detector_instance(self)` — [`L178`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L178)
  - `test_all_known_extensions_still_includes_orphans(self, detector_instance)` — [`L275`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L275) — The raw mapping (``get_all_known_extensions``) must still expose
  - `test_core_extensions_still_advertised(self, detector_instance)` — [`L240`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L240) — Make sure the trim didn't accidentally hide real, working
  - `test_every_supported_extension_maps_to_supported_language(self, detector_instance)` — [`L183`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L183) — Every extension reported as supported must resolve to a language
  - `test_orphan_extensions_not_advertised(self, detector_instance, extension)` — [`L229`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L229) — Orphan-plugin / no-parser extensions must NOT appear in the
  - `test_show_extensions_cli_advertises_scala(self)` — [`L285`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L285) — End-to-end check: ``--show-supported-extensions`` must mention
  - `test_show_languages_cli_advertises_scala(self)` — [`L312`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L312) — End-to-end check: ``--show-supported-languages`` must list
- uses (calls/refs, reference-scoped): [`LanguageDetector`](../../../tree_sitter_analyzer/language_detector.md#LanguageDetector)

### `TestR37adListQueriesJsonEnvelope`
- def: [`tests/unit/cli/test_info_commands.py:337`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L337)
- doc: r37ad (dogfood): `--list-queries` previously ignored
- signature: `class TestR37adListQueriesJsonEnvelope:`
- members:
  - `test_list_queries_json_for_all_languages(self)` — [`L373`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L373)
  - `test_list_queries_json_for_specific_language(self)` — [`L344`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L344)
  - `test_list_queries_text_path_preserved(self)` — [`L399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L399) — Text path (default) must still work — regression for backward compat.
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#ListQueriesCommand.execute), [`ListQueriesCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#ListQueriesCommand)

### `TestR37aeRemainingInfoCommandsJsonEnvelope`
- def: [`tests/unit/cli/test_info_commands.py:421`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L421)
- doc: r37ae (dogfood): batch follow-up to r37ad — extend JSON envelope
- signature: `class TestR37aeRemainingInfoCommandsJsonEnvelope:`
- members:
  - `test_describe_query_json_envelope(self)` — [`L428`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L428)
  - `test_describe_query_not_found_json_envelope(self)` — [`L456`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L456)
  - `test_show_languages_text_path_preserved(self)` — [`L524`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L524) — Text default must still go through output_list (backward compat).
  - `test_show_supported_extensions_json_envelope(self)` — [`L505`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L505)
  - `test_show_supported_languages_json_envelope(self)` — [`L481`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L481)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#DescribeQueryCommand.execute), [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowLanguagesCommand.execute), [`ShowLanguagesCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowLanguagesCommand), [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowExtensionsCommand.execute), [`DescribeQueryCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#DescribeQueryCommand), [`ShowExtensionsCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowExtensionsCommand)

### `TestShowExtensionsCommand`
- def: [`tests/unit/cli/test_info_commands.py:139`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L139)
- signature: `class TestShowExtensionsCommand:`
- members:
  - `test_show_extensions(self)` — [`L140`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L140)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowExtensionsCommand.execute), [`ShowExtensionsCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowExtensionsCommand)

### `TestShowLanguagesCommand`
- def: [`tests/unit/cli/test_info_commands.py:120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L120)
- signature: `class TestShowLanguagesCommand:`
- members:
  - `test_show_languages(self)` — [`L121`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L121)
- uses (calls/refs, reference-scoped): [`execute`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowLanguagesCommand.execute), [`ShowLanguagesCommand`](../../../tree_sitter_analyzer/cli/info_commands.md#ShowLanguagesCommand)

## Functions
- `args_no_language()` — [`L24`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L24)
- `args_with_file()` — [`L29`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L29)
- `args_with_language()` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_info_commands.py#L19)

