---
title: 'Module: benchmarks/codegraph_compare/adapters/native.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/adapters/native.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.adapters.native`/
symbols:
  NativeAdapter.build_run_config: NativeAdapter#build_run_config().
  NativeAdapter.parse_tool_metrics: NativeAdapter#parse_tool_metrics().
  NativeAdapter.prepare_index: NativeAdapter#prepare_index().
  NativeAdapter: NativeAdapter#
  _PROMPT_FILE: _PROMPT_FILE.
  _FILE_READ_TOOLS: _FILE_READ_TOOLS.
  _SEARCH_TOOLS: _SEARCH_TOOLS.
  _DEFAULT_SYSTEM_PROMPT: _DEFAULT_SYSTEM_PROMPT.
  _PROMPTS_DIR: _PROMPTS_DIR.
  _load_prompt: _load_prompt().
  NativeAdapter.arm_id: NativeAdapter#arm_id.
---
# Module: [`benchmarks/codegraph_compare/adapters/native.py`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py)

## Classes
### `NativeAdapter`  ·  implements/extends BenchmarkAdapter
- def: [`benchmarks/codegraph_compare/adapters/native.py:46`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L46)
- doc: Benchmark arm: native file-system tools only, no pre-built index.
- signature: `class NativeAdapter(BenchmarkAdapter):`
- members:
  - `build_run_config(self, repo_path: Path, question_prompt: str)` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L63)
  - `parse_tool_metrics(self, transcript_text: str)` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L79) — Count tool invocations from raw transcript text.
  - `prepare_index(self, repo_path: Path, cold: bool)` — [`L55`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L55) — No index to build. Returns zeroed stats immediately.
  - `arm_id` — [`L49`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L49)
- uses (calls/refs, reference-scoped): (23 test-only callers)
- used by: (5 test-only callers)

## Functions
- `_load_prompt(prompt_file: Path, default: str)` — [`L130`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L130) — Return the content of *prompt_file* if it exists, else *default*.

## Module values
- `_DEFAULT_SYSTEM_PROMPT` — [`L19`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L19)
- `_FILE_READ_TOOLS` — [`L42`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L42)
- `_PROMPTS_DIR` — [`L33`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L33)
- `_PROMPT_FILE` — [`L34`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L34)
- `_SEARCH_TOOLS` — [`L43`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/native.py#L43)

