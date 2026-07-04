---
title: 'Module: evaluation/client.py'
type: catalog
provenance: extracted
module: evaluation/client.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.client`/Evaluator#
symbols:
  Evaluator.async_run: async_run().
  Evaluator.agent: agent.
  Evaluator.loop: loop.
  Evaluator.run: run().
  Evaluator: ''
  Evaluator.llm_model: llm_model.
  Evaluator.tools: tools.
  Evaluator.__init__: __init__().
---
# Module: [`evaluation/client.py`](../../../../../raw/code/claude-context/evaluation/client.py)

## Classes
### `Evaluator`
- def: [`evaluation/client.py:10`](../../../../../raw/code/claude-context/evaluation/client.py#L10)
- doc: Evaluator class for running LLM queries with MCP tools
- signature: `class Evaluator:`
- members:
  - `__init__(self, llm_model, tools)` — [`L13`](../../../../../raw/code/claude-context/evaluation/client.py#L13) — Initialize the Evaluator
  - `async_run(self, query, codebase_path=None)` — [`L32`](../../../../../raw/code/claude-context/evaluation/client.py#L32) — Internal async method to run the query
  - `run(self, query: str, codebase_path=None)` — [`L50`](../../../../../raw/code/claude-context/evaluation/client.py#L50) — Run a query synchronously
  - `agent` — [`L23`](../../../../../raw/code/claude-context/evaluation/client.py#L23)
  - `llm_model` — [`L21`](../../../../../raw/code/claude-context/evaluation/client.py#L21)
  - `loop` — [`L27`](../../../../../raw/code/claude-context/evaluation/client.py#L27)
  - `tools` — [`L22`](../../../../../raw/code/claude-context/evaluation/client.py#L22)
- uses (calls/refs, reference-scoped): [`extract_conversation_summary`](utils/format.md#extract_conversation_summary), [`extract_file_paths_from_edits`](utils/format.md#extract_file_paths_from_edits), [`calculate_total_tokens`](utils/format.md#calculate_total_tokens)
- used by: [`async_search`](retrieval/custom.md#CustomRetrieval.async_search)

