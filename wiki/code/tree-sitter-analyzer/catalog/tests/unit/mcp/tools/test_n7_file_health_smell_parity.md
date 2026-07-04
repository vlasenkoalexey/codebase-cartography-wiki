---
title: 'Module: tests/unit/mcp/tools/test_n7_file_health_smell_parity.py'
type: catalog
provenance: extracted
module: tests/unit/mcp/tools/test_n7_file_health_smell_parity.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.mcp.tools.test_n7_file_health_smell_parity`/
symbols:
  TestN7FileHealthSmellParity.test_file_health_and_code_patterns_smell_types_agree: TestN7FileHealthSmellParity#test_file_health_and_code_patterns_smell_types_agree().
  TestN7FileHealthSmellParity.test_file_health_includes_mutable_default: TestN7FileHealthSmellParity#test_file_health_includes_mutable_default().
  TestN7FileHealthSmellParity.test_smell_type_no_security_prefix: TestN7FileHealthSmellParity#test_smell_type_no_security_prefix().
  _run: _run().
  TestN7CanonicalSmellTypeHelper.test_strips_security_prefix: TestN7CanonicalSmellTypeHelper#test_strips_security_prefix().
  TestN7CanonicalSmellTypeHelper.test_passthrough_for_bare_names: TestN7CanonicalSmellTypeHelper#test_passthrough_for_bare_names().
  TestN7CanonicalSmellTypeHelper.test_unknown_smell_returns_string: TestN7CanonicalSmellTypeHelper#test_unknown_smell_returns_string().
  smelly_python_file: smelly_python_file().
  TestN7FileHealthSmellParity: TestN7FileHealthSmellParity#
  TestN7CanonicalSmellTypeHelper: TestN7CanonicalSmellTypeHelper#
---
# Module: [`tests/unit/mcp/tools/test_n7_file_health_smell_parity.py`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py)

## Classes
### `TestN7CanonicalSmellTypeHelper`
- def: [`tests/unit/mcp/tools/test_n7_file_health_smell_parity.py:178`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L178)
- doc: Unit-level checks for the shared normalization helper.
- signature: `class TestN7CanonicalSmellTypeHelper:`
- members:
  - `test_passthrough_for_bare_names(self)` — [`L189`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L189)
  - `test_strips_security_prefix(self)` — [`L181`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L181)
  - `test_unknown_smell_returns_string(self)` — [`L199`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L199)
- uses (calls/refs, reference-scoped): [`canonical_smell_type`](../../../../tree_sitter_analyzer/mcp/tools/utils/file_health_smells.md#canonical_smell_type)

### `TestN7FileHealthSmellParity`
- def: [`tests/unit/mcp/tools/test_n7_file_health_smell_parity.py:72`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L72)
- doc: file_health.code_smells matches code_patterns.results.
- signature: `class TestN7FileHealthSmellParity:`
- members:
  - `test_file_health_and_code_patterns_smell_types_agree(self, tmp_path: Path, smelly_python_file: Path)` — [`L125`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L125) — The N7 contract: both tools see the same smell type strings.
  - `test_file_health_includes_mutable_default(self, tmp_path: Path, smelly_python_file: Path)` — [`L75`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L75) — file_health should now surface the mutable_default_argument
  - `test_smell_type_no_security_prefix(self, tmp_path: Path, smelly_python_file: Path)` — [`L96`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L96) — No code_smells[].type should carry the legacy ``security:`` prefix.
- uses (calls/refs, reference-scoped): [`execute`](../../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool.execute), [`CodePatternsTool`](../../../../tree_sitter_analyzer/mcp/tools/code_patterns_tool.md#CodePatternsTool), [`execute`](../../../../tree_sitter_analyzer/mcp/tools/file_health_tool.md#FileHealthTool.execute), [`FileHealthTool`](../../../../tree_sitter_analyzer/mcp/tools/file_health_tool.md#FileHealthTool)  (1 test-only)

## Functions
- `_run(coro: Any)` — [`L35`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L35) — Run an async coroutine in a fresh event loop.
- `smelly_python_file(tmp_path: Path)` — [`L50`](../../../../../../../../raw/code/tree-sitter-analyzer/tests/unit/mcp/tools/test_n7_file_health_smell_parity.py#L50) — Python file mixing security + anti-pattern + smell signals.

