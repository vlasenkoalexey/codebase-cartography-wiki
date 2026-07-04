---
title: 'Module: tests/unit/cli/test_install_skills.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_install_skills.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_install_skills`/Test
symbols:
  TestInstallSkillsHandlerDispatch.test_handle_install_skills_with_explicit_target: InstallSkillsHandlerDispatch#test_handle_install_skills_with_explicit_target().
  TestInstallSkillsHandlerDispatch.test_handle_install_skills_with_dot_target: InstallSkillsHandlerDispatch#test_handle_install_skills_with_dot_target().
  TestInstallSkillsHandlerDispatch.test_handle_install_skills_global_flag: InstallSkillsHandlerDispatch#test_handle_install_skills_global_flag().
  TestInstallSkillsHandlerDispatch.test_handle_install_skills_no_flag_returns_none: InstallSkillsHandlerDispatch#test_handle_install_skills_no_flag_returns_none().
  TestSkillContentSync.test_no_legacy_tool_names_in_skills: SkillContentSync#test_no_legacy_tool_names_in_skills().
  TestInstallSkillsPathValidation.test_self_copy_is_rejected: InstallSkillsPathValidation#test_self_copy_is_rejected().
  TestSkillContentSync.test_bundled_content_matches_claude_source_for_all_13_skills: SkillContentSync#test_bundled_content_matches_claude_source_for_all_13_skills().
  TestInstallSkillsHandlerDispatch.capture_json: InstallSkillsHandlerDispatch#capture_json().
  TestInstallSkillsHelper.test_install_copies_skills_to_target: InstallSkillsHelper#test_install_copies_skills_to_target().
  TestInstallSkillsHelper.test_install_global_uses_home_dot_claude: InstallSkillsHelper#test_install_global_uses_home_dot_claude().
  TestInstallSkillsHelper.test_no_overwrite_existing_skill: InstallSkillsHelper#test_no_overwrite_existing_skill().
  TestInstallSkillsHelper.test_idempotent_second_run: InstallSkillsHelper#test_idempotent_second_run().
  TestInstallSkillsCLIFlag.test_install_skills_flag_exists_in_parser: InstallSkillsCLIFlag#test_install_skills_flag_exists_in_parser().
  TestInstallSkillsCLIFlag.test_install_skills_global_flag_exists_in_parser: InstallSkillsCLIFlag#test_install_skills_global_flag_exists_in_parser().
  TestBundledSkillsWheelPath.test_skills_dir_constant_matches_file_parent: BundledSkillsWheelPath#test_skills_dir_constant_matches_file_parent().
  TestBundledSkillsWheelPath.test_exactly_13_tsa_dirs_via_skills_dir: BundledSkillsWheelPath#test_exactly_13_tsa_dirs_via_skills_dir().
  TestBundledSkillsWheelPath.test_each_skill_has_skill_md_via_skills_dir: BundledSkillsWheelPath#test_each_skill_has_skill_md_via_skills_dir().
  TestInstallSkillsErrorHandling.test_permission_error_on_mkdir_raised: InstallSkillsErrorHandling#test_permission_error_on_mkdir_raised().
  TestInstallSkillsErrorHandling.test_permission_error_on_copytree_raised: InstallSkillsErrorHandling#test_permission_error_on_copytree_raised().
  TestInstallSkillsErrorHandling.test_skip_existing_prints_to_stderr: InstallSkillsErrorHandling#test_skip_existing_prints_to_stderr().
  TestInstallSkillsErrorHandling.test_installed_skill_prints_to_stderr: InstallSkillsErrorHandling#test_installed_skill_prints_to_stderr().
  TestInstallSkillsErrorHandling.test_destination_echoed_to_stderr_before_install: InstallSkillsErrorHandling#test_destination_echoed_to_stderr_before_install().
  TestSkillContentSync.SKILL_NAMES: SkillContentSync#SKILL_NAMES.
  TestSkillContentSync._repo_root: SkillContentSync#_repo_root().
  TestBundledSkillsPackage: BundledSkillsPackage#
  TestBundledSkillsPackage.test_skills_dir_exists_in_package: BundledSkillsPackage#test_skills_dir_exists_in_package().
  TestBundledSkillsPackage.test_exactly_13_tsa_skill_dirs: BundledSkillsPackage#test_exactly_13_tsa_skill_dirs().
  TestBundledSkillsPackage.test_each_skill_dir_has_skill_md: BundledSkillsPackage#test_each_skill_dir_has_skill_md().
  TestBundledSkillsPackage.test_known_skill_names_present: BundledSkillsPackage#test_known_skill_names_present().
  TestInstallSkillsHelper: InstallSkillsHelper#
  TestInstallSkillsCLIFlag: InstallSkillsCLIFlag#
  TestBundledSkillsWheelPath: BundledSkillsWheelPath#
  TestInstallSkillsPathValidation: InstallSkillsPathValidation#
  TestInstallSkillsHandlerDispatch: InstallSkillsHandlerDispatch#
  TestInstallSkillsErrorHandling: InstallSkillsErrorHandling#
  TestSkillContentSync: SkillContentSync#
---
# Module: [`tests/unit/cli/test_install_skills.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py)

## Classes
### `TestBundledSkillsPackage`
- def: [`tests/unit/cli/test_install_skills.py:15`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L15)
- signature: `class TestBundledSkillsPackage:`
- members:
  - `test_each_skill_dir_has_skill_md(self)` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L33) — Every bundled tsa-* dir must contain SKILL.md.
  - `test_exactly_13_tsa_skill_dirs(self)` — [`L23`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L23) — Bundled skills dir must contain exactly 13 tsa-* subdirectories.
  - `test_known_skill_names_present(self)` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L42) — Spot-check: the 13 expected skill names are all present.
  - `test_skills_dir_exists_in_package(self)` — [`L16`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L16) — tree_sitter_analyzer/skills/ must exist as a package-level directory.

### `TestBundledSkillsWheelPath`
- def: [`tests/unit/cli/test_install_skills.py:170`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L170)
- doc: Verify bundled skills are reachable via the SKILLS_DIR constant that
- signature: `class TestBundledSkillsWheelPath:`
- members:
  - `test_each_skill_has_skill_md_via_skills_dir(self)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L197) — Every tsa-* dir reachable via SKILLS_DIR must contain SKILL.md.
  - `test_exactly_13_tsa_dirs_via_skills_dir(self)` — [`L187`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L187) — SKILLS_DIR must contain exactly 13 tsa-* subdirectories.
  - `test_skills_dir_constant_matches_file_parent(self)` — [`L179`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L179) — SKILLS_DIR in __init__.py must agree with __file__.parent.
- uses (calls/refs, reference-scoped): [`SKILLS_DIR`](../../../tree_sitter_analyzer/skills/__init__.md#SKILLS_DIR)

### `TestInstallSkillsCLIFlag`
- def: [`tests/unit/cli/test_install_skills.py:143`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L143)
- signature: `class TestInstallSkillsCLIFlag:`
- members:
  - `test_install_skills_flag_exists_in_parser(self)` — [`L144`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L144) — --install-skills must be registered in the argument parser.
  - `test_install_skills_global_flag_exists_in_parser(self)` — [`L154`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L154) — --install-skills-global must be registered alongside --install-skills.
- uses (calls/refs, reference-scoped): [`create_argument_parser`](../../../tree_sitter_analyzer/cli_main.md#create_argument_parser)

### `TestInstallSkillsErrorHandling`
- def: [`tests/unit/cli/test_install_skills.py:399`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L399)
- signature: `class TestInstallSkillsErrorHandling:`
- members:
  - `test_destination_echoed_to_stderr_before_install(self, tmp_path, capsys)` — [`L467`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L467) — #549: the resolved destination dir is echoed to stderr first, so the
  - `test_installed_skill_prints_to_stderr(self, tmp_path, capsys)` — [`L452`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L452) — When a skill is installed, message goes to stderr.
  - `test_permission_error_on_copytree_raised(self, tmp_path)` — [`L418`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L418) — install_skills propagates errors during copytree.
  - `test_permission_error_on_mkdir_raised(self, tmp_path)` — [`L400`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L400) — install_skills raises PermissionError when mkdir fails.
  - `test_skip_existing_prints_to_stderr(self, tmp_path, capsys)` — [`L436`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L436) — When a skill already exists, skip message goes to stderr.
- uses (calls/refs, reference-scoped): [`install_skills`](../../../tree_sitter_analyzer/cli/install_skills.md#install_skills)

### `TestInstallSkillsHandlerDispatch`
- def: [`tests/unit/cli/test_install_skills.py:249`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L249)
- signature: `class TestInstallSkillsHandlerDispatch:`
- members:
  - `capture_json(d)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L291)
  - `test_handle_install_skills_global_flag(self, tmp_path, monkeypatch)` — [`L356`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L356) — Test --install-skills-global installs to ~/.claude/skills/.
  - `test_handle_install_skills_no_flag_returns_none(self, tmp_path)` — [`L250`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L250) — Test _handle_install_skills returns None when no flags are set.
  - `test_handle_install_skills_with_dot_target(self, tmp_path, monkeypatch)` — [`L317`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L317) — Test --install-skills . installs to $CWD/.claude/skills/.
  - `test_handle_install_skills_with_explicit_target(self, tmp_path)` — [`L276`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L276) — Test --install-skills <dir> installs to <dir>/.claude/skills/.
- uses (calls/refs, reference-scoped): [`SpecialCommandContext`](../../../tree_sitter_analyzer/cli/special_commands.md#SpecialCommandContext), [`output_error`](../../../tree_sitter_analyzer/cli/special_commands.md#SpecialCommandContext.output_error), [`output_json`](../../../tree_sitter_analyzer/cli/special_commands.md#SpecialCommandContext.output_json), [`output_list`](../../../tree_sitter_analyzer/cli/special_commands.md#SpecialCommandContext.output_list), [`output_info`](../../../tree_sitter_analyzer/cli/special_commands.md#SpecialCommandContext.output_info), [`query_loader`](../../../tree_sitter_analyzer/cli/special_commands.md#SpecialCommandContext.query_loader), [`asyncio_run`](../../../tree_sitter_analyzer/cli/special_commands.md#SpecialCommandContext.asyncio_run), [`_handle_install_skills`](../../../tree_sitter_analyzer/cli/special_commands.md#_handle_install_skills)

### `TestInstallSkillsHelper`
- def: [`tests/unit/cli/test_install_skills.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L75)
- signature: `class TestInstallSkillsHelper:`
- members:
  - `test_idempotent_second_run(self, tmp_path)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L126) — Running install_skills twice must skip all dirs on the second run.
  - `test_install_copies_skills_to_target(self, tmp_path)` — [`L76`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L76) — install_skills should copy all 13 dirs into target/.claude/skills/.
  - `test_install_global_uses_home_dot_claude(self, tmp_path, monkeypatch)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L93) — With global=True, target must be ~/.claude/skills/.
  - `test_no_overwrite_existing_skill(self, tmp_path)` — [`L109`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L109) — If a skill dir already exists, it must be skipped (not overwritten).
- uses (calls/refs, reference-scoped): [`install_skills`](../../../tree_sitter_analyzer/cli/install_skills.md#install_skills)

### `TestInstallSkillsPathValidation`
- def: [`tests/unit/cli/test_install_skills.py:214`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L214)
- signature: `class TestInstallSkillsPathValidation:`
- members:
  - `test_self_copy_is_rejected(self)` — [`L215`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L215) — install_skills must raise ValueError if destination resolves into
- uses (calls/refs, reference-scoped): [`install_skills`](../../../tree_sitter_analyzer/cli/install_skills.md#install_skills), [`_bundled_skills_dir`](../../../tree_sitter_analyzer/cli/install_skills.md#_bundled_skills_dir)

### `TestSkillContentSync`
- def: [`tests/unit/cli/test_install_skills.py:488`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L488)
- doc: The bundled package copy (tree_sitter_analyzer/skills/) MUST be
- signature: `class TestSkillContentSync:`
- members:
  - `_repo_root(self)` — [`L512`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L512) — Locate the repository root relative to this test file.
  - `test_bundled_content_matches_claude_source_for_all_13_skills(self)` — [`L517`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L517) — Bundled SKILL.md bytes must equal .claude/skills SKILL.md bytes.
  - `test_no_legacy_tool_names_in_skills(self)` — [`L547`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L547) — Installed SKILL.md files must not contain legacy v1.x tool-call syntax.
  - `SKILL_NAMES` — [`L496`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_install_skills.py#L496)
- uses (calls/refs, reference-scoped): [`LEGACY_TOOL_MAP`](../../../tree_sitter_analyzer/mcp/facade_map.md#LEGACY_TOOL_MAP.LEGACY_TOOL_MAP)

