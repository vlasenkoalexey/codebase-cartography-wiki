---
title: 'Module: tree_sitter_analyzer/cli/agent_skills_metadata.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/cli/agent_skills_metadata.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.cli.agent_skills_metadata`/
symbols:
  split_front_matter: split_front_matter().
  DESCRIPTION_KEY: DESCRIPTION_KEY.
  _parse_front_matter_fields: _parse_front_matter_fields().
  NAME_KEY: NAME_KEY.
  read_skill_metadata: read_skill_metadata().
  _collect_front_matter_block: _collect_front_matter_block().
  DISABLE_MODEL_INVOCATION_KEY: DISABLE_MODEL_INVOCATION_KEY.
  metadata_bool: metadata_bool().
  _is_metadata_key: _is_metadata_key().
  _front_matter_end_index: _front_matter_end_index().
---
# Module: [`tree_sitter_analyzer/cli/agent_skills_metadata.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py)

## Functions
- `_collect_front_matter_block(lines: list[str], start_index: int)` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L72) — Collect indented block scalar lines until the next metadata key.
- `_front_matter_end_index(lines: list[str])` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L44) — Return the closing front-matter delimiter line index.
- `_is_metadata_key(line: str)` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L89) — Return True when a front-matter line starts a top-level key.
- `_parse_front_matter_fields(lines: list[str])` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L52) — Parse the small subset of YAML used in skill front matter.
- `metadata_bool(metadata: dict[str, str], key: str, default: bool = False)` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L36) — Read a front-matter boolean value.
- `read_skill_metadata(skill_path: Path)` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L12) — Read front-matter metadata and body text from a SKILL.md file.
- `split_front_matter(text: str)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L23) — Extract simple YAML front-matter keys used by Codex skills.

## Module values
- `DESCRIPTION_KEY` — [`L7`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L7)
- `DISABLE_MODEL_INVOCATION_KEY` — [`L8`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L8)
- `NAME_KEY` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/cli/agent_skills_metadata.py#L9)

