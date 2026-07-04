---
title: 'Module: benchmarks/codegraph_compare/adapters/codegraph.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/adapters/codegraph.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.adapters.codegraph`/
symbols:
  CodeGraphAdapter.build_run_config: CodeGraphAdapter#build_run_config().
  CodeGraphAdapter.prepare_index: CodeGraphAdapter#prepare_index().
  CodeGraphAdapter.parse_tool_metrics: CodeGraphAdapter#parse_tool_metrics().
  _build_index: _build_index().
  logger: logger.
  CodeGraphAdapter: CodeGraphAdapter#
  _PROMPT_FILE: _PROMPT_FILE.
  _delete_index: _delete_index().
  CodeGraphAdapter.__init__: CodeGraphAdapter#__init__().
  _FILE_READ_TOOLS: _FILE_READ_TOOLS.
  _SEARCH_TOOLS: _SEARCH_TOOLS.
  _CODEGRAPH_PREFIX: _CODEGRAPH_PREFIX.
  _dir_size: _dir_size().
  _count_files: _count_files().
  _DEFAULT_SYSTEM_PROMPT: _DEFAULT_SYSTEM_PROMPT.
  _PROMPTS_DIR: _PROMPTS_DIR.
  _INDEX_DIR: _INDEX_DIR.
  _ALLOWED_TOOLS: _ALLOWED_TOOLS.
  _load_prompt: _load_prompt().
---
# Module: [`benchmarks/codegraph_compare/adapters/codegraph.py`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py)

## Classes
### `CodeGraphAdapter`  ·  implements/extends BenchmarkAdapter
- def: [`benchmarks/codegraph_compare/adapters/codegraph.py:75`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L75)
- doc: Benchmark arm: CodeGraph AST index available to Claude.
- signature: `class CodeGraphAdapter(BenchmarkAdapter):`
- members:
  - `build_run_config(self, repo_path: Path, question_prompt: str)` — [`L126`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L126)
  - `parse_tool_metrics(self, transcript_text: str)` — [`L149`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L149) — Count tool invocations from raw transcript text.
  - `prepare_index(self, repo_path: Path, cold: bool)` — [`L89`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L89) — Build or verify the CodeGraph index under *repo_path/.codegraph/*.
- protocol/private: `__init__`[`L78`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L78)
- uses (calls/refs, reference-scoped): (31 test-only callers)
- used by: (5 test-only callers)

## Functions
- `_build_index(repo_path: Path, index_dir: Path)` — [`L207`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L207) — Run ``codegraph init -i`` and return IndexStats.
- `_count_files(path: Path)` — [`L253`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L253) — Return the number of files under *path*.
- `_delete_index(index_dir: Path)` — [`L197`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L197) — Remove the index directory if it exists.
- `_dir_size(path: Path)` — [`L246`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L246) — Return the total byte size of all files under *path*.
- `_load_prompt(prompt_file: Path, default: str)` — [`L260`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L260)

## Module values
- `_ALLOWED_TOOLS` — [`L54`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L54)
- `_CODEGRAPH_PREFIX` — [`L72`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L72)
- `_DEFAULT_SYSTEM_PROMPT` — [`L28`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L28)
- `_FILE_READ_TOOLS` — [`L70`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L70)
- `_INDEX_DIR` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L51)
- `_PROMPTS_DIR` — [`L44`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L44)
- `_PROMPT_FILE` — [`L45`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L45)
- `_SEARCH_TOOLS` — [`L71`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L71)
- `logger` — [`L22`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/codegraph.py#L22)

