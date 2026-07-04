---
title: 'Module: tree_sitter_analyzer/uml_state.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/uml_state.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.uml_state`/
symbols:
  build_state_result: build_state_result().
  _extract_transitions: _extract_transitions().
  StateResult.error: StateResult#error.
  StateResult.transitions: StateResult#transitions.
  StateResult.states: StateResult#states.
  _parse_file_for_state: _parse_file_for_state().
  StateTransition.source: StateTransition#source.
  StateTransition.target: StateTransition#target.
  StateTransition: StateTransition#
  _node_text: _node_text().
  _extract_transitions._parse_enum_ref: _extract_transitions()._parse_enum_ref().
  _extract_transitions._find_return_enum_ref: _extract_transitions()._find_return_enum_ref().
  StateResult: StateResult#
  _extract_enum_members: _extract_enum_members().
  _find_enum_classes._walk: _find_enum_classes()._walk().
  StateTransition.label: StateTransition#label.
  StateResult.truncated: StateResult#truncated.
  _extract_transitions._find_match_statements: _extract_transitions()._find_match_statements().
  _find_enum_classes: _find_enum_classes().
  _extract_transitions._find_case_pattern_member: _extract_transitions()._find_case_pattern_member().
  _extract_transitions._iter_case_clauses: _extract_transitions()._iter_case_clauses().
---
# Module: [`tree_sitter_analyzer/uml_state.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py)

## Classes
### `StateResult`
- def: [`tree_sitter_analyzer/uml_state.py:44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L44)
- doc: Result of a state-machine scan.
- signature: `class StateResult:`
- members:
  - `error` — [`L50`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L50) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `states` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L47) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `transitions` — [`L48`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L48) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `truncated` — [`L49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L49)
- uses (calls/refs, reference-scoped): [`StateTransition`](uml_state.md#StateTransition)
- used by: [`build_state_result`](uml_state.md#build_state_result), [`state_diagram`](uml_export.md#UMLExporter.state_diagram)  (24 test-only)

### `StateTransition`
- def: [`tree_sitter_analyzer/uml_state.py:35`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L35)
- doc: A directed transition between two states.
- signature: `class StateTransition:`
- members:
  - `label` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L40)
  - `source` — [`L38`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L38) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
  - `target` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L39) — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- used by: [`build_state_result`](uml_state.md#build_state_result), [`state_diagram`](uml_export.md#UMLExporter.state_diagram), [`_extract_transitions`](uml_state.md#_extract_transitions), [`transitions`](uml_state.md#StateResult.transitions)  (13 test-only)

## Functions
- `_extract_enum_members(class_node: Any)` — [`L137`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L137) — Extract Enum member names from a class_definition body.
- `_extract_transitions(root: Any, class_name: str, known_members: set[str])` — [`L162`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L162) — Walk root for match_statement nodes and extract FSM transitions. — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)
- `_find_case_pattern_member(node: Any)` — [`L227`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L227) — Extract the enum member from a case pattern like TrafficLight.RED.
- `_find_enum_classes(root: Any, class_name_filter: str | None)` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L99) — Walk the root node to find class definitions that inherit from Enum.
- `_find_match_statements(node: Any)` — [`L180`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L180)
- `_find_return_enum_ref(node: Any)` — [`L198`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L198) — Recursively search for a return_statement or assignment whose RHS is
- `_iter_case_clauses(match_stmt: Any)` — [`L248`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L248) — Return all case_clause nodes from a match_statement.
- `_node_text(node: Any, max_len: int = 60)` — [`L87`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L87) — Decode a tree-sitter node's text, capped at max_len chars.
- `_parse_enum_ref(node: Any)` — [`L188`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L188) — Return the member name if node is <class_name>.<member>.
- `_parse_file_for_state(file_path: str, language: str = "python")` — [`L58`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L58) — Parse *file_path* with tree-sitter and return (tree_root, source_bytes).
- `_walk(node: Any)` — [`L110`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L110)
- `build_state_result(file_path: str, class_name: str | None, max_nodes: int = 50, language: str = "python")` — [`L307`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/uml_state.py#L307) — Parse *file_path* and extract FSM states and transitions. — documented in [tree_sitter_analyzer-uml_export](../../concepts/tree_sitter_analyzer-uml_export.md)

