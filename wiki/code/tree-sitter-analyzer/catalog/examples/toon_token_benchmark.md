---
title: 'Module: examples/toon_token_benchmark.py'
type: catalog
provenance: extracted
module: examples/toon_token_benchmark.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `examples.toon_token_benchmark`/
symbols:
  main: main().
  TokenCounter.count_tokens: TokenCounter#count_tokens().
  run_benchmark: run_benchmark().
  print_benchmark_result: print_benchmark_result().
  TokenCounter._encoding: TokenCounter#_encoding.
  TokenCount: TokenCount#
  TokenCount.token_count: TokenCount#token_count.
  TokenCount.char_count: TokenCount#char_count.
  TokenCount.is_estimated: TokenCount#is_estimated.
  TokenCount.format_name: TokenCount#format_name.
  TokenCounter: TokenCounter#
  TokenCounter.CHARS_PER_TOKEN: TokenCounter#CHARS_PER_TOKEN.
  TokenCounter._tiktoken: TokenCounter#_tiktoken.
  create_sample_analysis_result: create_sample_analysis_result().
  create_mcp_response: create_mcp_response().
  create_simple_dict: create_simple_dict().
  TokenCounter.__init__: TokenCounter#__init__().
---
# Module: [`examples/toon_token_benchmark.py`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py)

## Classes
### `TokenCount`
- def: [`examples/toon_token_benchmark.py:28`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L28)
- doc: Token count result.
- signature: `class TokenCount:`
- members:
  - `char_count` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L32)
  - `format_name` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L31)
  - `is_estimated` — [`L34`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L34)
  - `token_count` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L33)
- used by: (3 test-only callers)

### `TokenCounter`
- def: [`examples/toon_token_benchmark.py:37`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L37)
- doc: Token counter that uses tiktoken if available, otherwise estimates.
- signature: `class TokenCounter:`
- members:
  - `__init__(self)` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L47) — Initialize token counter.
  - `count_tokens(self, text: str, format_name: str)` — [`L62`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L62) — Count tokens in text.
  - `CHARS_PER_TOKEN` — [`L45`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L45)
- protocol/private: `_encoding`[`L50`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L50), `_tiktoken`[`L49`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L49)
- uses (calls/refs, reference-scoped): (5 test-only callers)
- used by: (2 test-only callers)

## Functions
- `create_mcp_response()` — [`L215`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L215) — Create a typical MCP tool response for benchmarking.
- `create_sample_analysis_result()` — [`L95`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L95) — Create a realistic code analysis result for benchmarking.
- `create_simple_dict()` — [`L248`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L248) — Create a simple dictionary for benchmarking.
- `main()` — [`L327`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L327) — Run token reduction benchmarks.
- `print_benchmark_result(name: str, json_count: TokenCount, toon_count: TokenCount, reduction: float)` — [`L298`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L298) — Print formatted benchmark result.
- `run_benchmark(data: dict, name: str, counter: TokenCounter)` — [`L264`](../../../../../raw/code/tree-sitter-analyzer/examples/toon_token_benchmark.py#L264) — Run benchmark comparing JSON and TOON formats.

