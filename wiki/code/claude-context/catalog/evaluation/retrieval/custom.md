---
title: 'Module: evaluation/retrieval/custom.py'
type: catalog
provenance: extracted
module: evaluation/retrieval/custom.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.retrieval.custom`/
symbols:
  CustomRetrieval.async_run: CustomRetrieval#async_run().
  CustomRetrieval.async_search: CustomRetrieval#async_search().
  CustomRetrieval.mcp_client: CustomRetrieval#mcp_client.
  logger: logger.
  CustomRetrieval.mcp_sessions_context: CustomRetrieval#mcp_sessions_context().
  CustomRetrieval.async_build_index: CustomRetrieval#async_build_index().
  CustomRetrieval.retrieval_types: CustomRetrieval#retrieval_types.
  CustomRetrieval._load_tools_from_sessions: CustomRetrieval#_load_tools_from_sessions().
  CustomRetrieval._create_mcp_client: CustomRetrieval#_create_mcp_client().
  CustomRetrieval: CustomRetrieval#
  CustomRetrieval.llm_model: CustomRetrieval#llm_model.
  CustomRetrieval.run: CustomRetrieval#run().
  CustomRetrieval.__init__: CustomRetrieval#__init__().
  CustomRetrieval.build_index: CustomRetrieval#build_index().
  CustomRetrieval.search: CustomRetrieval#search().
---
# Module: [`evaluation/retrieval/custom.py`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py)

## Classes
### `CustomRetrieval`  ·  implements/extends BaseRetrieval
- def: [`evaluation/retrieval/custom.py:26`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L26)
- signature: `class CustomRetrieval(BaseRetrieval):`
- members:
  - `__init__(self, llm_type: str, llm_model: str, retrieval_types: List[str], *, dataset_name_or_path, splits, output_dir, **kwargs)` — [`L27`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L27) — Initialize CustomRetrieval with specified retrieval types.
  - `_create_mcp_client(self)` — [`L72`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L72) — Create MCP client based on retrieval types
  - `_load_tools_from_sessions(self, sessions: Dict)` — [`L183`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L183) — Load tools from the provided sessions
  - `async_build_index(self, repo_path: str)` — [`L249`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L249) — Build index only if CC is enabled
  - `async_run(self, root_dir: str, token: str = "git")` — [`L328`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L328)
  - `async_search(self, repo_path: str, issue: str, k: int = 20)` — [`L293`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L293)
  - `build_index(self, repo_path: str)` — [`L246`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L246)
  - `mcp_sessions_context(self)` — [`L113`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L113) — Context manager for MCP sessions and tools loading
  - `run(self, root_dir: str, token: str = "git")` — [`L325`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L325)
  - `search(self, repo_path: str, issue: str, k: int = 20)` — [`L290`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L290)
  - `llm_model` — [`L69`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L69)
  - `mcp_client` — [`L70`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L70)
  - `retrieval_types` — [`L68`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L68)
- uses (calls/refs, reference-scoped): [`async_run`](../client.md#Evaluator.async_run), [`logger`](custom.md#logger), [`evaluation_path`](../utils/constant.md#evaluation_path), [`create_unified_diff_file`](../utils/format.md#create_unified_diff_file), [`clone_repo`](../utils/file_management.md#clone_repo), [`output_dir`](base.md#BaseRetrieval.output_dir), [`BaseRetrieval`](base.md#BaseRetrieval), [`instances`](base.md#BaseRetrieval.instances), [`ContextManager`](../utils/file_management.md#ContextManager), [`Evaluator`](../client.md#Evaluator), [`extract_oracle_files_from_patch`](../utils/format.md#extract_oracle_files_from_patch), [`llm_factory`](../utils/llm_factory.md#llm_factory), [`__init__`](base.md#BaseRetrieval.__init__), [`prompt`](base.md#BaseRetrieval.prompt)
- used by: [`run`](base.md#BaseRetrieval.run), [`main`](../run_evaluation.md#main), [`BaseRetrieval`](base.md#BaseRetrieval), [`build_index`](base.md#BaseRetrieval.build_index), [`search`](base.md#BaseRetrieval.search)

## Module values
- `logger` — [`L23`](../../../../../../raw/code/claude-context/evaluation/retrieval/custom.py#L23)

