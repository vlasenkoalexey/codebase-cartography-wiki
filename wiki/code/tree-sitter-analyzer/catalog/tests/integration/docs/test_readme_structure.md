---
title: 'Module: tests/integration/docs/test_readme_structure.py'
type: catalog
provenance: extracted
module: tests/integration/docs/test_readme_structure.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.integration.docs.test_readme_structure`/
symbols:
  README_PATH: README_PATH.
  TestNoStaleFacadeToolNames.test_no_stale_codegraph_tool_names: TestNoStaleFacadeToolNames#test_no_stale_codegraph_tool_names().
  TestOnboardingPrerequisites.test_python_version_prerequisite_in_get_started: TestOnboardingPrerequisites#test_python_version_prerequisite_in_get_started().
  TestOnboardingPrerequisites.test_full_index_prereq_for_callers_callees: TestOnboardingPrerequisites#test_full_index_prereq_for_callers_callees().
  get_readme_content: get_readme_content().
  TestReadmeLineCount.test_readme_under_500_lines: TestReadmeLineCount#test_readme_under_500_lines().
  TestHeroSection.test_hero_section_within_first_20_lines: TestHeroSection#test_hero_section_within_first_20_lines().
  TestSectionHeaders.test_section_headers_have_emoji: TestSectionHeaders#test_section_headers_have_emoji().
  TestWhatsNewSection.test_whats_new_section_brevity: TestWhatsNewSection#test_whats_new_section_brevity().
  TestRequiredSections.test_required_sections_exist: TestRequiredSections#test_required_sections_exist().
  README_JA_PATH: README_JA_PATH.
  README_ZH_PATH: README_ZH_PATH.
  TestAIIntegrationPosition.test_ai_integration_in_first_half: TestAIIntegrationPosition#test_ai_integration_in_first_half().
  TestCLICommandsSection.test_cli_commands_has_five_examples: TestCLICommandsSection#test_cli_commands_has_five_examples().
  get_readme_lines: get_readme_lines().
  PROJECT_ROOT: PROJECT_ROOT.
  MAX_README_LINES: MAX_README_LINES.
  MAX_WHATS_NEW_LINES: MAX_WHATS_NEW_LINES.
  HERO_SECTION_MAX_LINE: HERO_SECTION_MAX_LINE.
  get_section_headers: get_section_headers().
  TestRequiredSections.REQUIRED_SECTIONS: TestRequiredSections#REQUIRED_SECTIONS.
  _STALE_TOOL_NAME: _STALE_TOOL_NAME.
  TestReadmeLineCount: TestReadmeLineCount#
  TestHeroSection: TestHeroSection#
  TestSectionHeaders: TestSectionHeaders#
  TestWhatsNewSection: TestWhatsNewSection#
  TestAIIntegrationPosition: TestAIIntegrationPosition#
  TestCLICommandsSection: TestCLICommandsSection#
  TestRequiredSections: TestRequiredSections#
  TestOnboardingPrerequisites: TestOnboardingPrerequisites#
  TestNoStaleFacadeToolNames: TestNoStaleFacadeToolNames#
---
# Module: [`tests/integration/docs/test_readme_structure.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py)

## Classes
### `TestAIIntegrationPosition`
- def: [`tests/integration/docs/test_readme_structure.py:154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L154)
- doc: Tests for AI Integration section position.
- signature: `class TestAIIntegrationPosition:`
- members:
  - `test_ai_integration_in_first_half(self)` — [`L164`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L164) — AI Integration section should appear within first 50% of the document.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestCLICommandsSection`
- def: [`tests/integration/docs/test_readme_structure.py:185`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L185)
- doc: Tests for CLI Commands section completeness.
- signature: `class TestCLICommandsSection:`
- members:
  - `test_cli_commands_has_five_examples(self)` — [`L191`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L191) — Common CLI Commands section should contain at least 5 distinct command examples.
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestHeroSection`
- def: [`tests/integration/docs/test_readme_structure.py:56`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L56)
- doc: Tests for Hero section position and content.
- signature: `class TestHeroSection:`
- members:
  - `test_hero_section_within_first_20_lines(self)` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L62) — Hero section (project name, badges, value proposition) should be within first 20 lines.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestNoStaleFacadeToolNames`
- def: [`tests/integration/docs/test_readme_structure.py:306`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L306)
- doc: The feature table + quick-start must reference real facade tools.
- signature: `class TestNoStaleFacadeToolNames:`
- members:
  - `test_no_stale_codegraph_tool_names(self, readme_path: Path)` — [`L320`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L320)
- uses (calls/refs, reference-scoped): (5 test-only callers)

### `TestOnboardingPrerequisites`
- def: [`tests/integration/docs/test_readme_structure.py:266`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L266)
- doc: #545/#548: README onboarding prerequisites must be present in all 3 locales.
- signature: `class TestOnboardingPrerequisites:`
- members:
  - `test_full_index_prereq_for_callers_callees(self, readme_path: Path)` — [`L296`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L296) — #548: CLI section must note that --callers/--callees require --full-index.
  - `test_python_version_prerequisite_in_get_started(self, readme_path: Path)` — [`L278`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L278) — #545: Get Started section must state the Python minimum version.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestReadmeLineCount`
- def: [`tests/integration/docs/test_readme_structure.py:42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L42)
- doc: Tests for README line count constraints.
- signature: `class TestReadmeLineCount:`
- members:
  - `test_readme_under_500_lines(self)` — [`L48`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L48) — README.md should be under 500 lines.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestRequiredSections`
- def: [`tests/integration/docs/test_readme_structure.py:224`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L224)
- doc: Tests for required sections existence.
- signature: `class TestRequiredSections:`
- members:
  - `test_required_sections_exist(self)` — [`L245`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L245) — All required sections should exist in README.
  - `REQUIRED_SECTIONS` — [`L227`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L227)
- uses (calls/refs, reference-scoped): (2 test-only callers)

### `TestSectionHeaders`
- def: [`tests/integration/docs/test_readme_structure.py:83`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L83)
- doc: Tests for section header formatting.
- signature: `class TestSectionHeaders:`
- members:
  - `test_section_headers_have_emoji(self)` — [`L94`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L94) — All major section headers should contain emoji for visual navigation.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestWhatsNewSection`
- def: [`tests/integration/docs/test_readme_structure.py:120`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L120)
- doc: Tests for What's New section brevity.
- signature: `class TestWhatsNewSection:`
- members:
  - `test_whats_new_section_brevity(self)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L126) — What's New section should be limited to 15 lines or fewer.
- uses (calls/refs, reference-scoped): (3 test-only callers)

## Functions
- `get_readme_content(readme_path: Path)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L23) — Read README content.
- `get_readme_lines(readme_path: Path)` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L28) — Get README lines as list.
- `get_section_headers(content: str)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L33) — Extract section headers with their line numbers.

## Module values
- `HERO_SECTION_MAX_LINE` — [`L20`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L20)
- `MAX_README_LINES` — [`L18`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L18)
- `MAX_WHATS_NEW_LINES` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L19)
- `PROJECT_ROOT` — [`L13`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L13)
- `README_JA_PATH` — [`L15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L15)
- `README_PATH` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L14)
- `README_ZH_PATH` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L16)
- `_STALE_TOOL_NAME` — [`L263`](../../../../../../../raw/code/tree-sitter-analyzer/tests/integration/docs/test_readme_structure.py#L263)

