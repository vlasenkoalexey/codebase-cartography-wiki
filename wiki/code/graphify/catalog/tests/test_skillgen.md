---
title: 'Module: tests/test_skillgen.py'
type: catalog
provenance: extracted
module: tests/test_skillgen.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_skillgen`/
symbols:
  _platform_artifacts: _platform_artifacts().
  REPO_ROOT: REPO_ROOT.
  _claude_artifacts: _claude_artifacts().
  test_no_version_or_timestamp_in_output: test_no_version_or_timestamp_in_output().
  test_lean_core_has_no_reference_only_content: test_lean_core_has_no_reference_only_content().
  test_lean_core_runs_default_pipeline_with_zero_references: test_lean_core_runs_default_pipeline_with_zero_references().
  test_references_contain_no_core_pipeline_content: test_references_contain_no_core_pipeline_content().
  test_reference_pointers_in_core_resolve_to_real_fragments: test_reference_pointers_in_core_resolve_to_real_fragments().
  test_query_heading_is_homed_in_core_stub_only: test_query_heading_is_homed_in_core_stub_only().
  test_eight_references_render_for_claude: test_eight_references_render_for_claude().
  test_enum_is_full_six_value_superset_in_extraction_spec: test_enum_is_full_six_value_superset_in_extraction_spec().
  test_descriptions_are_unified: test_descriptions_are_unified().
  test_windows_frontmatter_name_and_shell_and_extra: test_windows_frontmatter_name_and_shell_and_extra().
  test_codex_dispatch_is_agenttask_and_collects_in_memory: test_codex_dispatch_is_agenttask_and_collects_in_memory().
  test_codex_and_windows_unify_enum_to_six_values: test_codex_and_windows_unify_enum_to_six_values().
  test_codex_uses_compact_extraction_windows_uses_verbose: test_codex_uses_compact_extraction_windows_uses_verbose().
  test_every_platform_query_has_expansion_and_fallback: test_every_platform_query_has_expansion_and_fallback().
  test_all_progressive_hosts_check_and_audit_clean: test_all_progressive_hosts_check_and_audit_clean().
  test_no_host_has_trigger_in_frontmatter: test_no_host_has_trigger_in_frontmatter().
  test_kilo_renders_its_rules_tail_section: test_kilo_renders_its_rules_tail_section().
  test_dispatch_variants_are_host_specific: test_dispatch_variants_are_host_specific().
  test_compact_extraction_hosts_use_the_compact_spec: test_compact_extraction_hosts_use_the_compact_spec().
  test_every_split_host_renders_eight_references: test_every_split_host_renders_eight_references().
  test_monoliths_change_only_sanctioned_lines: test_monoliths_change_only_sanctioned_lines().
  test_generated_runbooks_pass_root_to_save_manifest: test_generated_runbooks_pass_root_to_save_manifest().
  test_trae_renders_native_agents_md_integration_not_claude: test_trae_renders_native_agents_md_integration_not_claude().
  test_trae_dispatch_carries_the_no_pretooluse_caveat: test_trae_dispatch_carries_the_no_pretooluse_caveat().
  test_trae_hooks_reference_includes_the_pretooluse_note: test_trae_hooks_reference_includes_the_pretooluse_note().
  test_claude_flavored_hosts_keep_their_hooks_text_unchanged: test_claude_flavored_hosts_keep_their_hooks_text_unchanged().
  test_amp_renders_native_agents_md_integration_v8_faithfully: test_amp_renders_native_agents_md_integration_v8_faithfully().
  test_amp_has_no_pretooluse_caveat_anywhere: test_amp_has_no_pretooluse_caveat_anywhere().
  test_agents_renders_its_own_agents_md_hooks_wording: test_agents_renders_its_own_agents_md_hooks_wording().
  UNIFIED_DESCRIPTION: UNIFIED_DESCRIPTION.
  _PROGRESSIVE_HOSTS: _PROGRESSIVE_HOSTS.
  test_audit_coverage_passes: test_audit_coverage_passes().
  test_check_passes: test_check_passes().
  test_render_is_idempotent: test_render_is_idempotent().
  test_render_output_is_lf_only: test_render_output_is_lf_only().
  test_extraction_states_no_api_key_required_for_every_host: test_extraction_states_no_api_key_required_for_every_host().
  test_headings_helper_ignores_code_fence_comments: test_headings_helper_ignores_code_fence_comments().
  test_check_passes_for_codex_and_windows: test_check_passes_for_codex_and_windows().
  test_audit_coverage_passes_for_codex_and_windows: test_audit_coverage_passes_for_codex_and_windows().
  test_schema_singleton_passes_across_all_platforms: test_schema_singleton_passes_across_all_platforms().
  test_schema_singleton_catches_legacy_enums: test_schema_singleton_catches_legacy_enums().
  test_monoliths_render_inline_single_file_no_references: test_monoliths_render_inline_single_file_no_references().
  test_monolith_roundtrip_passes_for_aider_and_devin: test_monolith_roundtrip_passes_for_aider_and_devin().
  test_monoliths_carry_the_1392_runbook_fixes: test_monoliths_carry_the_1392_runbook_fixes().
  test_devin_keeps_its_multi_field_frontmatter: test_devin_keeps_its_multi_field_frontmatter().
  test_always_on_renders_six_blocks: test_always_on_renders_six_blocks().
  test_always_on_included_in_full_render_not_per_platform: test_always_on_included_in_full_render_not_per_platform().
  test_always_on_roundtrip_is_byte_faithful: test_always_on_roundtrip_is_byte_faithful().
  test_extracted_constants_equal_the_packaged_always_on_files: test_extracted_constants_equal_the_packaged_always_on_files().
  test_always_on_files_are_guarded_by_check: test_always_on_files_are_guarded_by_check().
  test_audit_coverage_passes_for_every_split_host: test_audit_coverage_passes_for_every_split_host().
  test_audit_reads_each_host_against_its_own_v8_body: test_audit_reads_each_host_against_its_own_v8_body().
  test_audit_catches_an_induced_per_host_drop: test_audit_catches_an_induced_per_host_drop().
  test_audit_catches_a_dropped_non_allowlisted_heading: test_audit_catches_a_dropped_non_allowlisted_heading().
  test_git_show_validators_skip_cleanly_without_origin_v8: test_git_show_validators_skip_cleanly_without_origin_v8().
  test_audit_allowlist_documents_only_consolidations: test_audit_allowlist_documents_only_consolidations().
  test_amp_audit_coverage_passes_against_its_own_v8: test_amp_audit_coverage_passes_against_its_own_v8().
  test_agents_body_matches_amp_modulo_hooks_wording: test_agents_body_matches_amp_modulo_hooks_wording().
  test_agents_audit_baseline_is_amps_v8_body: test_agents_audit_baseline_is_amps_v8_body().
---
# Module: [`tests/test_skillgen.py`](../../../../../raw/code/graphify/tests/test_skillgen.py)

## Functions
- `_claude_artifacts()` — [`L70`](../../../../../raw/code/graphify/tests/test_skillgen.py#L70)
- `_platform_artifacts(key)` — [`L233`](../../../../../raw/code/graphify/tests/test_skillgen.py#L233)
- `test_agents_audit_baseline_is_amps_v8_body()` — [`L932`](../../../../../raw/code/graphify/tests/test_skillgen.py#L932) — `agents` is a post-v8 platform, so its audit baseline is amp's v8 body.
- `test_agents_body_matches_amp_modulo_hooks_wording()` — [`L911`](../../../../../raw/code/graphify/tests/test_skillgen.py#L911) — The agents skill body is amp's body verbatim (it re-homes amp's bundle).
- `test_agents_renders_its_own_agents_md_hooks_wording()` — [`L887`](../../../../../raw/code/graphify/tests/test_skillgen.py#L887) — `agents` re-homes amp's agents-md body but with its OWN install wording.
- `test_all_progressive_hosts_check_and_audit_clean()` — [`L388`](../../../../../raw/code/graphify/tests/test_skillgen.py#L388) — check + audit-coverage pass for every rendered progressive host.
- `test_always_on_files_are_guarded_by_check(tmp_path)` — [`L654`](../../../../../raw/code/graphify/tests/test_skillgen.py#L654) — A hand-edit of an always_on/*.md is caught by --check (the drift guard).
- `test_always_on_included_in_full_render_not_per_platform()` — [`L587`](../../../../../raw/code/graphify/tests/test_skillgen.py#L587) — A full render carries the always-on files; a --platform render does not.
- `test_always_on_renders_six_blocks()` — [`L573`](../../../../../raw/code/graphify/tests/test_skillgen.py#L573) — render_always_on yields exactly the six always-on instruction files.
- `test_always_on_roundtrip_is_byte_faithful()` — [`L596`](../../../../../raw/code/graphify/tests/test_skillgen.py#L596) — Each always_on/*.md reproduces its former __main__.py constant byte for byte.
- `test_amp_audit_coverage_passes_against_its_own_v8()` — [`L871`](../../../../../raw/code/graphify/tests/test_skillgen.py#L871) — The per-host audit (the guard amp is the exact case for) passes for amp.
- `test_amp_has_no_pretooluse_caveat_anywhere()` — [`L853`](../../../../../raw/code/graphify/tests/test_skillgen.py#L853) — amp's v8 had no no-PreToolUse-hooks note, so neither its core nor hooks may.
- `test_amp_renders_native_agents_md_integration_v8_faithfully()` — [`L823`](../../../../../raw/code/graphify/tests/test_skillgen.py#L823) — amp wires `graphify amp install` -> AGENTS.md exactly as its v8 body had it.
- `test_audit_allowlist_documents_only_consolidations()` — [`L753`](../../../../../raw/code/graphify/tests/test_skillgen.py#L753) — The allowlist holds only the wave-2/3 consolidations, nothing genuine.
- `test_audit_catches_a_dropped_non_allowlisted_heading()` — [`L711`](../../../../../raw/code/graphify/tests/test_skillgen.py#L711) — A core fragment that drops a real v8 heading fails the audit.
- `test_audit_catches_an_induced_per_host_drop()` — [`L694`](../../../../../raw/code/graphify/tests/test_skillgen.py#L694) — Re-inducing the trae regression (claude-flavored hooks) fails the audit.
- `test_audit_coverage_passes()` — [`L25`](../../../../../raw/code/graphify/tests/test_skillgen.py#L25) — Every v8 heading lands in the lean core or exactly one reference.
- `test_audit_coverage_passes_for_codex_and_windows()` — [`L251`](../../../../../raw/code/graphify/tests/test_skillgen.py#L251) — Every v8 heading single-homes for the cli-inline split hosts too.
- `test_audit_coverage_passes_for_every_split_host()` — [`L674`](../../../../../raw/code/graphify/tests/test_skillgen.py#L674) — Every split host's render single-homes its own v8 body's headings.
- `test_audit_reads_each_host_against_its_own_v8_body()` — [`L684`](../../../../../raw/code/graphify/tests/test_skillgen.py#L684) — The audit baseline is the host's OWN v8 skill body, not claude's monolith.
- `test_check_passes()` — [`L32`](../../../../../raw/code/graphify/tests/test_skillgen.py#L32) — The committed artifacts and the expected/ snapshot match a fresh render.
- `test_check_passes_for_codex_and_windows()` — [`L242`](../../../../../raw/code/graphify/tests/test_skillgen.py#L242) — The committed codex/windows artifacts match a fresh render and expected/.
- `test_claude_flavored_hosts_keep_their_hooks_text_unchanged()` — [`L804`](../../../../../raw/code/graphify/tests/test_skillgen.py#L804) — Hosts whose v8 shipped the claude-flavored hooks keep it (faithful to them).
- `test_codex_and_windows_unify_enum_to_six_values()` — [`L316`](../../../../../raw/code/graphify/tests/test_skillgen.py#L316) — codex (was 4-value) and windows (was 5-value) now carry the superset.
- `test_codex_dispatch_is_agenttask_and_collects_in_memory()` — [`L300`](../../../../../raw/code/graphify/tests/test_skillgen.py#L300) — codex: spawn/wait/close_agent dispatch needing multi_agent = true.
- `test_codex_uses_compact_extraction_windows_uses_verbose()` — [`L328`](../../../../../raw/code/graphify/tests/test_skillgen.py#L328) — The extraction variant differs: codex compact, windows verbose.
- `test_compact_extraction_hosts_use_the_compact_spec()` — [`L429`](../../../../../raw/code/graphify/tests/test_skillgen.py#L429) — kiro, pi, claw use the compact extraction body; the rest use verbose.
- `test_descriptions_are_unified()` — [`L268`](../../../../../raw/code/graphify/tests/test_skillgen.py#L268) — Every platform now carries one unified frontmatter description, byte for byte.
- `test_devin_keeps_its_multi_field_frontmatter()` — [`L560`](../../../../../raw/code/graphify/tests/test_skillgen.py#L560) — devin renders inline, so its 4+-field frontmatter is preserved verbatim.
- `test_dispatch_variants_are_host_specific()` — [`L414`](../../../../../raw/code/graphify/tests/test_skillgen.py#L414) — Each dispatch variant lands in the right host's B2 slot.
- `test_eight_references_render_for_claude()` — [`L192`](../../../../../raw/code/graphify/tests/test_skillgen.py#L192) — claude renders exactly the eight on-demand fragments from the design.
- `test_enum_is_full_six_value_superset_in_extraction_spec()` — [`L222`](../../../../../raw/code/graphify/tests/test_skillgen.py#L222) — Decision A: the file_type enum is the full six-value superset.
- `test_every_platform_query_has_expansion_and_fallback()` — [`L336`](../../../../../raw/code/graphify/tests/test_skillgen.py#L336) — #1325: the unified query reference ships BOTH the vocab-expansion step and
- `test_every_split_host_renders_eight_references()` — [`L439`](../../../../../raw/code/graphify/tests/test_skillgen.py#L439) — All twelve split hosts render exactly the eight on-demand references.
- `test_extracted_constants_equal_the_packaged_always_on_files()` — [`L636`](../../../../../raw/code/graphify/tests/test_skillgen.py#L636) — The live module constants now equal the packaged files they read at load.
- `test_extraction_states_no_api_key_required_for_every_host()` — [`L124`](../../../../../raw/code/graphify/tests/test_skillgen.py#L124) — Regression for #1461: every skill body that describes Step 3 extraction must
- `test_generated_runbooks_pass_root_to_save_manifest()` — [`L534`](../../../../../raw/code/graphify/tests/test_skillgen.py#L534) — #1417: every save_manifest call in a shipped runbook threads root=.
- `test_git_show_validators_skip_cleanly_without_origin_v8(monkeypatch, tmp_path, capsys)` — [`L733`](../../../../../raw/code/graphify/tests/test_skillgen.py#L733) — On a shallow checkout (no origin/v8) the validators skip with exit 0.
- `test_headings_helper_ignores_code_fence_comments()` — [`L207`](../../../../../raw/code/graphify/tests/test_skillgen.py#L207) — The fence-aware heading scanner must skip '#' lines inside code fences.
- `test_kilo_renders_its_rules_tail_section()` — [`L407`](../../../../../raw/code/graphify/tests/test_skillgen.py#L407) — kilo gets the Kilo-specific rules tail before Honesty Rules.
- `test_lean_core_has_no_reference_only_content()` — [`L78`](../../../../../raw/code/graphify/tests/test_skillgen.py#L78) — The core must not inline the execution detail of an on-demand reference.
- `test_lean_core_runs_default_pipeline_with_zero_references()` — [`L103`](../../../../../raw/code/graphify/tests/test_skillgen.py#L103) — The default code-corpus run must be fully described inside the core.
- `test_monolith_roundtrip_passes_for_aider_and_devin()` — [`L473`](../../../../../raw/code/graphify/tests/test_skillgen.py#L473) — Each monolith is diff-clean vs v8 except the file_type enum unification.
- `test_monoliths_carry_the_1392_runbook_fixes()` — [`L498`](../../../../../raw/code/graphify/tests/test_skillgen.py#L498) — The four #1392 data-loss/correctness fixes are present in both monoliths.
- `test_monoliths_change_only_sanctioned_lines()` — [`L481`](../../../../../raw/code/graphify/tests/test_skillgen.py#L481) — Every line that differs from pristine v8 is a sanctioned change-class.
- `test_monoliths_render_inline_single_file_no_references()` — [`L462`](../../../../../raw/code/graphify/tests/test_skillgen.py#L462) — aider and devin render one inline body, no split and no references dir.
- `test_no_host_has_trigger_in_frontmatter()` — [`L398`](../../../../../raw/code/graphify/tests/test_skillgen.py#L398) — No split host emits a trigger: field — not part of Agent Skills spec (#1180).
- `test_no_version_or_timestamp_in_output()` — [`L61`](../../../../../raw/code/graphify/tests/test_skillgen.py#L61) — No generated artifact carries the package version string.
- `test_query_heading_is_homed_in_core_stub_only()` — [`L179`](../../../../../raw/code/graphify/tests/test_skillgen.py#L179) — The query section heading is the lean-core stub; query.md re-homes the rest.
- `test_reference_pointers_in_core_resolve_to_real_fragments()` — [`L168`](../../../../../raw/code/graphify/tests/test_skillgen.py#L168) — Every references/<name>.md the core points at is actually rendered.
- `test_references_contain_no_core_pipeline_content()` — [`L152`](../../../../../raw/code/graphify/tests/test_skillgen.py#L152) — No reference fragment may duplicate the core build pipeline.
- `test_render_is_idempotent()` — [`L44`](../../../../../raw/code/graphify/tests/test_skillgen.py#L44) — Rendering twice yields byte-identical output (no timestamps/versions).
- `test_render_output_is_lf_only()` — [`L52`](../../../../../raw/code/graphify/tests/test_skillgen.py#L52) — Generated artifacts use LF newlines and end in exactly one newline.
- `test_schema_singleton_catches_legacy_enums()` — [`L360`](../../../../../raw/code/graphify/tests/test_skillgen.py#L360) — The guard's line scanner flags 4- and 5-value pipe enums, not the superset.
- `test_schema_singleton_passes_across_all_platforms()` — [`L353`](../../../../../raw/code/graphify/tests/test_skillgen.py#L353) — The file_type enum is the six-value superset in every rendered artifact.
- `test_trae_dispatch_carries_the_no_pretooluse_caveat()` — [`L788`](../../../../../raw/code/graphify/tests/test_skillgen.py#L788) — trae's B2 dispatch block restores the v8 no-PreToolUse-hook caveat.
- `test_trae_hooks_reference_includes_the_pretooluse_note()` — [`L796`](../../../../../raw/code/graphify/tests/test_skillgen.py#L796) — The trae hooks reference keeps the v8 PreToolUse note in full.
- `test_trae_renders_native_agents_md_integration_not_claude()` — [`L770`](../../../../../raw/code/graphify/tests/test_skillgen.py#L770) — trae wires `graphify trae install` -> AGENTS.md, never `graphify claude install`.
- `test_windows_frontmatter_name_and_shell_and_extra()` — [`L287`](../../../../../raw/code/graphify/tests/test_skillgen.py#L287) — windows: graphify-windows name, powershell install, troubleshooting tail.

## Module values
- `REPO_ROOT` — [`L18`](../../../../../raw/code/graphify/tests/test_skillgen.py#L18)
- `UNIFIED_DESCRIPTION` — [`L259`](../../../../../raw/code/graphify/tests/test_skillgen.py#L259)
- `_PROGRESSIVE_HOSTS` — [`L374`](../../../../../raw/code/graphify/tests/test_skillgen.py#L374)

