---
title: 'Module: tree_sitter_analyzer/constraints/schema.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/constraints/schema.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.constraints.schema`/
symbols:
  Constraint: Constraint#
  Constraint.id: Constraint#id.
  Violation: Violation#
  Violation.rule_id: Violation#rule_id.
  Violation.caller_file: Violation#caller_file.
  Violation.caller_line: Violation#caller_line.
  Violation.callee_file: Violation#callee_file.
  Violation.callee_name: Violation#callee_name.
  Constraint.severity: Constraint#severity.
  Constraint.exceptions: Constraint#exceptions.
  Violation.caller_name: Violation#caller_name.
  Violation.severity: Violation#severity.
  Constraint.from_glob: Constraint#from_glob.
  Constraint.to_glob: Constraint#to_glob.
  Violation.detected_at: Violation#detected_at.
  Constraint.rule: Constraint#rule.
  Constraint.reason: Constraint#reason.
---
# Module: [`tree_sitter_analyzer/constraints/schema.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py)

## Classes
### `Constraint`
- def: [`tree_sitter_analyzer/constraints/schema.py:25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L25)
- doc: One parsed architectural rule.
- signature: `class Constraint:`
- members:
  - `exceptions` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L53)
  - `from_glob` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L50)
  - `id` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L47)
  - `reason` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L52)
  - `rule` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L49)
  - `severity` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L48)
  - `to_glob` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L51)
- used by: [`_iter_violations`](evaluator.md#_iter_violations), [`load_constraints`](parser.md#load_constraints), [`_parse_rule`](parser.md#_parse_rule), [`evaluate`](evaluator.md#evaluate), [`compile_constraints`](parser.md#compile_constraints), [`constraint`](parser.md#_CompiledConstraint.constraint)  (3 test-only)

### `Violation`
- def: [`tree_sitter_analyzer/constraints/schema.py:57`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L57)
- doc: One offending call edge produced by `evaluate()`.
- signature: `class Violation:`
- members:
  - `callee_file` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L74)
  - `callee_name` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L73)
  - `caller_file` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L70)
  - `caller_line` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L72)
  - `caller_name` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L71)
  - `detected_at` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L76)
  - `rule_id` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L69)
  - `severity` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/constraints/schema.py#L75)
- used by: [`_iter_violations`](evaluator.md#_iter_violations), [`_run_and_persist`](../cli/commands/constraint_check_command.md#_run_and_persist), [`_run_and_persist`](../mcp/tools/constraint_check_tool.md#ConstraintCheckTool._run_and_persist), [`evaluate`](evaluator.md#evaluate)  (4 test-only)

