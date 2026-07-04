---
title: 'Module: tree_sitter_analyzer/cli/agent_skills.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/agent_skills.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.agent_skills`/
symbols:
  _build_skill_record: _build_skill_record().
  build_agent_skills_inventory: build_agent_skills_inventory().
  _skill_gaps: _skill_gaps().
  _extract_description: _extract_description().
  _build_read_order: _build_read_order().
  _display_path: _display_path().
  _skill_actionability: _skill_actionability().
  _list_support_files: _list_support_files().
  _build_agent_trigger: _build_agent_trigger().
  _contains_completion_guidance: _contains_completion_guidance().
  _display_optional_path: _display_optional_path().
  _discover_skills: _discover_skills().
  _list_script_files: _list_script_files().
  _build_agent_summary: _build_agent_summary().
  _top_actionable_skills: _top_actionable_skills().
  _truncate: _truncate().
  SKILL_FILE: SKILL_FILE.
  SUPPORT_FILE_LIMIT: SUPPORT_FILE_LIMIT.
  _detect_labels: _detect_labels().
  AGENT_BRIEF_FILE: AGENT_BRIEF_FILE.
  OUT_OF_SCOPE_FILE: OUT_OF_SCOPE_FILE.
  READ_ORDER_SUPPORT_LIMIT: READ_ORDER_SUPPORT_LIMIT.
  ACCEPTANCE_MARKERS: ACCEPTANCE_MARKERS.
  CONTEXT_MARKERS: CONTEXT_MARKERS.
  SIDE_EFFECT_MARKERS: SIDE_EFFECT_MARKERS.
  ACTIONABILITY_PREVIEW_LIMIT: ACTIONABILITY_PREVIEW_LIMIT.
  _skills_verdict: _skills_verdict().
  _build_summary_line: _build_summary_line().
  _resolve_skills_root: _resolve_skills_root().
  _combined_skill_text: _combined_skill_text().
  _has_trigger_text: _has_trigger_text().
  _extract_title: _extract_title().
  _body_paragraphs: _body_paragraphs().
  _dedupe: _dedupe().
  _build_gaps: _build_gaps().
  _build_toon_content: _build_toon_content().
---
# Module: [`tree_sitter_analyzer/cli/agent_skills.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py)

## Functions
- `_body_paragraphs(skill_text: str)` — [`L365`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L365) — Collect non-empty Markdown body paragraphs.
- `_build_agent_summary(skills: list[dict[str, Any]], gaps: dict[str, Any], validation: dict[str, Any])` — [`L441`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L441) — Build the compact decision surface agents read first.
- `_build_agent_trigger(metadata: dict[str, str], fallback_name: str)` — [`L388`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L388) — Build a short instruction for when an agent should load the skill.
- `_build_gaps(skills: list[dict[str, Any]], root_path: Path)` — [`L422`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L422) — Aggregate skill inventory gaps for fast agent decisions.
- `_build_read_order(project_path: Path, skill_path: Path, brief_path: Path, support_files: list[str])` — [`L396`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L396) — Suggest a stable reading order for an agent using the skill.
- `_build_skill_record(project_path: Path, skill_dir: Path)` — [`L173`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L173) — Build a compact inventory record for one skill directory.
- `_build_summary_line(result: dict[str, Any])` — [`L132`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L132) — Build the canonical one-line headline for agent_skills output.
- `_build_toon_content(result: dict[str, Any])` — [`L500`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L500) — Build a compact text representation for --format toon.
- `_combined_skill_text(skill_text: str, brief_path: Path)` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L313) — Combine primary skill text and optional agent brief text.
- `_contains_completion_guidance(combined: str)` — [`L321`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L321) — Detect whether a skill exposes completion or verification criteria.
- `_dedupe(items: list[str])` — [`L410`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L410) — De-duplicate while preserving the preferred reading order.
- `_detect_labels(text: str, marker_groups: dict[str, tuple[str, ...]])` — [`L335`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L335) — Detect named labels from marker groups.
- `_discover_skills(project_path: Path, root_path: Path)` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L161) — Discover skill directories in stable name order.
- `_display_optional_path(path: Path, project_path: Path)` — [`L530`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L530) — Display a path only when it exists.
- `_display_path(path: Path, project_path: Path)` — [`L535`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L535) — Display project-relative paths when possible.
- `_extract_description(metadata: dict[str, str], skill_text: str)` — [`L353`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L353) — Return front-matter description or the first useful body paragraph.
- `_extract_title(skill_text: str, fallback: str)` — [`L345`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L345) — Extract the first Markdown H1 title.
- `_has_trigger_text(description: str)` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L327) — Return True when front matter gives a useful skill activation hint.
- `_list_script_files(skill_dir: Path, project_path: Path)` — [`L281`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L281) — List bundled script files separately from docs-style support files.
- `_list_support_files(skill_dir: Path, project_path: Path)` — [`L271`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L271) — List non-SKILL support files for a skill directory.
- `_resolve_skills_root(project_path: Path, skills_root: str | None)` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L153) — Resolve the skills root relative to the project when needed.
- `_skill_actionability(metadata: dict[str, str], has_skill_md: bool, has_agent_brief: bool, gaps: list[str], support_file_count: int)` — [`L233`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L233) — Compute a compact actionability score from metadata and guidance gaps.
- `_skill_gaps(skill_path: Path, metadata: dict[str, str], combined_text: str)` — [`L293`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L293) — Return inventory gaps that make a skill harder for agents to apply.
- `_skills_verdict(validation: dict[str, Any], gaps: dict[str, Any], root_path: Path)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L51) — Canonical verdict for the agent-skills envelope.
- `_top_actionable_skills(skills: list[dict[str, Any]])` — [`L494`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L494) — Return highest-actionability skills by score.
- `_truncate(text: str, limit: int = 220)` — [`L382`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L382) — Keep CLI JSON compact without hiding useful trigger text.
- `build_agent_skills_inventory(project_root: str, skills_root: str | None = None)` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L84) — Build an agent-friendly inventory of project-local skills.

## Module values
- `ACCEPTANCE_MARKERS` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L22)
- `ACTIONABILITY_PREVIEW_LIMIT` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L48)
- `AGENT_BRIEF_FILE` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L18)
- `CONTEXT_MARKERS` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L31)
- `OUT_OF_SCOPE_FILE` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L19)
- `READ_ORDER_SUPPORT_LIMIT` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L21)
- `SIDE_EFFECT_MARKERS` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L37)
- `SKILL_FILE` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L17)
- `SUPPORT_FILE_LIMIT` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills.py#L20)

