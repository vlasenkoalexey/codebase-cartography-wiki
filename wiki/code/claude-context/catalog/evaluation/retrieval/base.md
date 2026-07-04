---
title: 'Module: evaluation/retrieval/base.py'
type: catalog
provenance: extracted
module: evaluation/retrieval/base.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.retrieval.base`/
symbols:
  BaseRetrieval.run: BaseRetrieval#run().
  BaseRetrieval._prepare_instances: BaseRetrieval#_prepare_instances().
  logger: logger.
  BaseRetrieval._filter_existing_instances: BaseRetrieval#_filter_existing_instances().
  BaseRetrieval.dataset_name_or_path: BaseRetrieval#dataset_name_or_path.
  BaseRetrieval.max_instances: BaseRetrieval#max_instances.
  BaseRetrieval.output_dir: BaseRetrieval#output_dir.
  BaseRetrieval: BaseRetrieval#
  BaseRetrieval.instances: BaseRetrieval#instances.
  BaseRetrieval.build_index: BaseRetrieval#build_index().
  BaseRetrieval.search: BaseRetrieval#search().
  BaseRetrieval.splits: BaseRetrieval#splits.
  BaseRetrieval.__init__: BaseRetrieval#__init__().
  BaseRetrieval.prompt: BaseRetrieval#prompt.
---
# Module: [`evaluation/retrieval/base.py`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py)

## Classes
### `BaseRetrieval`
- def: [`evaluation/retrieval/base.py:21`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L21)
- signature: `class BaseRetrieval:`
- members:
  - `_filter_existing_instances(self, instances: List[Dict], output_file: Path)` — [`L126`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L126) — Filter instances to exclude those that have already been processed.
  - `build_index(self, repo_path: str)` — [`L176`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L176)
  - `run(self, root_dir: str, token: str = "git")` — [`L182`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L182)
  - `search(self, repo_path: str, issue: str, k: int = 20)` — [`L179`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L179)
  - `dataset_name_or_path` — [`L25`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L25)
  - `instances` — [`L29`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L29)
  - `max_instances` — [`L28`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L28)
  - `output_dir` — [`L27`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L27)
  - `prompt` — [`L30`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L30)
  - `splits` — [`L26`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L26)
- protocol/private: `__init__`[`L22`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L22), `_prepare_instances`[`L42`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L42)
- uses (calls/refs, reference-scoped): [`logger`](base.md#logger), [`clone_repo`](../utils/file_management.md#clone_repo), [`CustomRetrieval`](custom.md#CustomRetrieval), [`get_remaining_instances`](../utils/file_management.md#get_remaining_instances), [`ContextManager`](../utils/file_management.md#ContextManager), [`run`](custom.md#CustomRetrieval.run), [`build_index`](custom.md#CustomRetrieval.build_index), [`search`](custom.md#CustomRetrieval.search)
- used by: [`async_run`](custom.md#CustomRetrieval.async_run), [`async_search`](custom.md#CustomRetrieval.async_search), [`CustomRetrieval`](custom.md#CustomRetrieval), [`__init__`](custom.md#CustomRetrieval.__init__)

## Module values
- `logger` — [`L18`](../../../../../../raw/code/claude-context/evaluation/retrieval/base.py#L18)

