---
title: 'Module: benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.adapters.tree_sitter_analyzer`/
symbols:
  TSAAdapter.build_run_config: TSAAdapter#build_run_config().
  TSAAdapter.prepare_index: TSAAdapter#prepare_index().
  _build_cache: _build_cache().
  TSAAdapter.parse_tool_metrics: TSAAdapter#parse_tool_metrics().
  TSAAdapter: TSAAdapter#
  TSAAdapter.classify: TSAAdapter#classify().
  logger: logger.
  _delete_cache: _delete_cache().
  _ALLOWED_TOOLS: _ALLOWED_TOOLS.
  _PROMPT_FILE: _PROMPT_FILE.
  TSAAdapter.__init__: TSAAdapter#__init__().
  _ANALYZER_ROOT: _ANALYZER_ROOT.
  _dir_size: _dir_size().
  _indexed_file_count: _indexed_file_count().
  _DEFAULT_SYSTEM_PROMPT: _DEFAULT_SYSTEM_PROMPT.
  _PROMPTS_DIR: _PROMPTS_DIR.
  _CACHE_DIR: _CACHE_DIR.
  _CACHE_INDEX: _CACHE_INDEX.
  _FILE_READ_TOOLS: _FILE_READ_TOOLS.
  _SEARCH_TOOLS: _SEARCH_TOOLS.
  _TSA_MCP_PREFIX: _TSA_MCP_PREFIX.
  _count_files: _count_files().
  _load_prompt: _load_prompt().
---
# Module: [`benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py)

## Classes
### `TSAAdapter`  ·  implements/extends BenchmarkAdapter
- def: [`benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py:85`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L85)
- doc: Benchmark arm: tree-sitter-analyzer AST cache available via Bash.
- signature: `class TSAAdapter(BenchmarkAdapter):`
- members:
  - `build_run_config(self, repo_path: Path, question_prompt: str)` — [`L145`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L145)
  - `classify(name: str)` — [`L182`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L182)
  - `parse_tool_metrics(self, transcript_text: str)` — [`L170`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L170) — Count tool invocations from raw transcript text.
  - `prepare_index(self, repo_path: Path, cold: bool)` — [`L97`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L97) — Build or verify the TSA AST cache under *repo_path/.ast-cache/*.
- protocol/private: `__init__`[`L88`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L88)
- uses (calls/refs, reference-scoped): (32 test-only callers)
- used by: (10 test-only callers)

## Functions
- `_build_cache(repo_path: Path, cache_dir: Path)` — [`L226`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L226) — Run tree-sitter-analyzer's AST-cache indexer for the target repo.
- `_count_files(path: Path)` — [`L291`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L291) — Return the number of files under *path*.
- `_delete_cache(cache_dir: Path)` — [`L216`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L216) — Remove the AST cache directory if it exists.
- `_dir_size(path: Path)` — [`L284`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L284) — Return the total byte size of all files under *path*.
- `_indexed_file_count(index_db: Path)` — [`L298`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L298) — Return ast_index row count, or None for unreadable/corrupt DBs.
- `_load_prompt(prompt_file: Path, default: str)` — [`L311`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L311)

## Module values
- `_ALLOWED_TOOLS` — [`L63`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L63)
- `_ANALYZER_ROOT` — [`L53`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L53)
- `_CACHE_DIR` — [`L59`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L59)
- `_CACHE_INDEX` — [`L60`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L60)
- `_DEFAULT_SYSTEM_PROMPT` — [`L32`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L32)
- `_FILE_READ_TOOLS` — [`L79`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L79)
- `_PROMPTS_DIR` — [`L51`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L51)
- `_PROMPT_FILE` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L52)
- `_SEARCH_TOOLS` — [`L80`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L80)
- `_TSA_MCP_PREFIX` — [`L82`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L82)
- `logger` — [`L26`](../../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/adapters/tree_sitter_analyzer.py#L26)

