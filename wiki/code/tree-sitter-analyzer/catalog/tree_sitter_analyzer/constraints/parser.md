---
title: 'Module: tree_sitter_analyzer/constraints/parser.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/constraints/parser.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.constraints.parser`/
symbols:
  load_constraints: load_constraints().
  _parse_rule: _parse_rule().
  compile_constraints: compile_constraints().
  ConstraintParseError: ConstraintParseError#
  _compile_glob: _compile_glob().
  _CompiledConstraint.constraint: _CompiledConstraint#constraint.
  match_glob: match_glob().
  logger: logger.
  _CompiledConstraint: _CompiledConstraint#
  _ALLOWED_RULE_KEYS._ALLOWED_RULE_KEYS: _ALLOWED_RULE_KEYS._ALLOWED_RULE_KEYS.
  _CompiledConstraint.from_re: _CompiledConstraint#from_re.
  _CompiledConstraint.to_re: _CompiledConstraint#to_re.
  _CompiledConstraint.exception_res: _CompiledConstraint#exception_res.
  _ALLOWED_TOP_LEVEL._ALLOWED_TOP_LEVEL: _ALLOWED_TOP_LEVEL._ALLOWED_TOP_LEVEL.
  _REQUIRED_RULE_KEYS._REQUIRED_RULE_KEYS: _REQUIRED_RULE_KEYS._REQUIRED_RULE_KEYS.
  _ALLOWED_SEVERITIES._ALLOWED_SEVERITIES: _ALLOWED_SEVERITIES._ALLOWED_SEVERITIES.
  _ALLOWED_RULES._ALLOWED_RULES: _ALLOWED_RULES._ALLOWED_RULES.
  _find_config_file: _find_config_file().
  _extract_line: _extract_line().
  _OPTIONAL_RULE_KEYS._OPTIONAL_RULE_KEYS: _OPTIONAL_RULE_KEYS._OPTIONAL_RULE_KEYS.
---
# Module: [`tree_sitter_analyzer/constraints/parser.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py)

## Classes
### `ConstraintParseError`  ·  implements/extends ValueError
- def: [`tree_sitter_analyzer/constraints/parser.py:42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L42)
- doc: Raised on malformed YAML or schema violations.
- signature: `class ConstraintParseError(ValueError):`
- used by: [`load_constraints`](parser.md#load_constraints), [`execute`](../mcp/tools/constraint_check_tool.md#ConstraintCheckTool.execute), [`_evaluate_with_explicit_file`](../cli/commands/constraint_check_command.md#_evaluate_with_explicit_file)  (3 test-only)

### `_CompiledConstraint`
- def: [`tree_sitter_analyzer/constraints/parser.py:58`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L58)
- doc: A constraint with its globs pre-compiled to regex.
- signature: `class _CompiledConstraint:`
- members:
  - `constraint` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L66)
  - `exception_res` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L69)
  - `from_re` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L67)
  - `to_re` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L68)
- uses (calls/refs, reference-scoped): [`Constraint`](schema.md#Constraint)
- used by: [`_iter_violations`](evaluator.md#_iter_violations), [`compile_constraints`](parser.md#compile_constraints), [`_is_excepted`](evaluator.md#_is_excepted)

## Functions
- `_compile_glob(pattern: str)` — [`L276`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L276) — Compile an fnmatch-style glob to a regex with ``**`` support.
- `_extract_line(exc: yaml.YAMLError)` — [`L321`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L321) — Pull a 1-based line number out of a PyYAML error, or '?' as fallback.
- `_find_config_file(project_root: Path)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L77) — Return the constraints YAML path or None when nothing is configured.
- `_parse_rule(rule_raw: Any, index: int, config_path: Path)` — [`L193`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L193) — Validate one rule mapping; return the Constraint or None to skip.
- `compile_constraints(constraints: list[Constraint])` — [`L297`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L297) — Pre-compile each constraint's globs to regex.
- `load_constraints(project_root: str | Path)` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L109) — Load and validate architectural-constraints from ``project_root``.
- `match_glob(pattern: str, path: str)` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L175) — Return True when ``path`` matches ``pattern`` under our glob model.

## Module values
- `_ALLOWED_RULES` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L106)
- `_ALLOWED_RULE_KEYS` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L104)
- `_ALLOWED_SEVERITIES` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L105)
- `_ALLOWED_TOP_LEVEL` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L99)
- `_OPTIONAL_RULE_KEYS` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L103)
- `_REQUIRED_RULE_KEYS` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L100)
- `logger` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/parser.py#L34)

