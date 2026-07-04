---
title: 'Module: tests/unit/cli/test_agent_skills.py'
type: catalog
provenance: extracted
module: tests/unit/cli/test_agent_skills.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.cli.test_agent_skills`/test_
symbols:
  test_split_front_matter_supports_folded_descriptions: split_front_matter_supports_folded_descriptions().
  test_agent_skills_inventory_exposes_decision_fields: agent_skills_inventory_exposes_decision_fields().
  test_agent_skills_inventory_reports_missing_completion_without_brief_noise: agent_skills_inventory_reports_missing_completion_without_brief_noise().
  test_skill_validation_separates_blocking_caution_and_optional_gaps: skill_validation_separates_blocking_caution_and_optional_gaps().
---
# Module: [`tests/unit/cli/test_agent_skills.py`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_agent_skills.py)

## Functions
- `test_agent_skills_inventory_exposes_decision_fields(tmp_path)` — [`L39`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_agent_skills.py#L39) — Inventory records should expose the fields an agent needs before loading.
- `test_agent_skills_inventory_reports_missing_completion_without_brief_noise(tmp_path)` — [`L86`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_agent_skills.py#L86) — Missing AGENT-BRIEF is optional, while missing completion guidance is a gap.
- `test_skill_validation_separates_blocking_caution_and_optional_gaps()` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_agent_skills.py#L119) — Validation summary should distinguish hard blockers from metadata polish.
- `test_split_front_matter_supports_folded_descriptions()` — [`L14`](../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/cli/test_agent_skills.py#L14) — Folded YAML front matter should become useful trigger text.

