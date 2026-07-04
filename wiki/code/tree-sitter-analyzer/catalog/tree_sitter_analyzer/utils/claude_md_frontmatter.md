---
title: 'Module: tree_sitter_analyzer/utils/claude_md_frontmatter.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/utils/claude_md_frontmatter.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.utils.claude_md_frontmatter`/
symbols:
  _build_design_rule: _build_design_rule().
  parse_intentional_design: parse_intentional_design().
  parse_fixture_allowlist: parse_fixture_allowlist().
  load_frontmatter: load_frontmatter().
  logger: logger.
  IntentionalDesignRule.id: IntentionalDesignRule#id.
  FixtureAllowlistEntry.path: FixtureAllowlistEntry#path.
  IntentionalDesignRule: IntentionalDesignRule#
  IntentionalDesignRule.action: IntentionalDesignRule#action.
  _normalise_action: _normalise_action().
  IntentionalDesignRule.file_patterns: IntentionalDesignRule#file_patterns.
  FixtureAllowlistEntry: FixtureAllowlistEntry#
  IntentionalDesignRule.symbols: IntentionalDesignRule#symbols.
  FixtureAllowlistEntry.note: FixtureAllowlistEntry#note.
  VALID_VERDICT_ACTIONS.VALID_VERDICT_ACTIONS: VALID_VERDICT_ACTIONS.VALID_VERDICT_ACTIONS.
  _coerce_globs: _coerce_globs().
  _compile_patterns: _compile_patterns().
  _coerce_symbols: _coerce_symbols().
  IntentionalDesignRule.raw_globs: IntentionalDesignRule#raw_globs.
  IntentionalDesignRule.note: IntentionalDesignRule#note.
  _FRONTMATTER_RE: _FRONTMATTER_RE.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/utils/claude_md_frontmatter.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py)

## Classes
### `FixtureAllowlistEntry`
- def: [`tree_sitter_analyzer/utils/claude_md_frontmatter.py:81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L81)
- doc: A single `fixture_allowlist` entry.
- signature: `class FixtureAllowlistEntry:`
- members:
  - `note` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L90)
  - `path` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L89)
- used by: [`_allowlist_facts`](../security/fixture_detector.md#_allowlist_facts), [`parse_fixture_allowlist`](claude_md_frontmatter.md#parse_fixture_allowlist)  (6 test-only)

### `IntentionalDesignRule`
- def: [`tree_sitter_analyzer/utils/claude_md_frontmatter.py:64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L64)
- doc: A locked design-decision rule extracted from `intentional_design`.
- signature: `class IntentionalDesignRule:`
- members:
  - `action` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L76)
  - `file_patterns` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L74)
  - `id` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L72)
  - `note` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L77)
  - `raw_globs` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L73)
  - `symbols` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L75)
- used by: [`_build_design_rule`](claude_md_frontmatter.md#_build_design_rule), [`parse_intentional_design`](claude_md_frontmatter.md#parse_intentional_design)  (14 test-only)

## Functions
- `_build_design_rule(entry: dict[str, Any], rule_id: str)` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L210) — Build one rule from a validated entry dict, or ``None`` on error.
- `_coerce_globs(raw: Any, rule_id: str)` — [`L168`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L168) — Return a non-empty tuple of glob strings, or ``None`` on validation error.
- `_coerce_symbols(raw: Any, rule_id: str)` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L196) — Coerce raw ``symbols`` value to a tuple of strings.
- `_compile_patterns(globs: tuple[str, ...], rule_id: str)` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L181) — Compile glob strings to PathSpec objects, or ``None`` on error.
- `_normalise_action(raw: Any, rule_id: str)` — [`L268`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L268) — Coerce a raw ``action_when_touched`` value to a known verdict.
- `load_frontmatter(project_root: str | Path)` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L98) — Return the parsed YAML frontmatter from ``<project_root>/CLAUDE.md``.
- `parse_fixture_allowlist(data: dict[str, Any])` — [`L301`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L301) — Compile the ``fixture_allowlist`` section into typed records.
- `parse_intentional_design(data: dict[str, Any])` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L232) — Compile the ``intentional_design`` section into typed records.

## Module values
- `VALID_VERDICT_ACTIONS` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L48)
- `_FRONTMATTER_RE` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L52)
- `__all__` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L341)
- `logger` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/utils/claude_md_frontmatter.py#L40)

