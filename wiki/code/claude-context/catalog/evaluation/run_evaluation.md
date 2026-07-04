---
title: 'Module: evaluation/run_evaluation.py'
type: catalog
provenance: extracted
module: evaluation/run_evaluation.py
status: fresh
symbol_base: scip-python python claude-context 0.0.0 `evaluation.run_evaluation`/
symbols:
  parser: parser.
  main: main().
  args: args.
  logger: logger.
  parse_retrieval_types: parse_retrieval_types().
---
# Module: [`evaluation/run_evaluation.py`](../../../../../raw/code/claude-context/evaluation/run_evaluation.py)

## Functions
- `main(dataset_name_or_path: str, output_dir: str, retrieval_types: List[str], llm_type: str = "openai", llm_model: Optional[str] = None, splits: List[str] = ["test"], root_dir: str = str(evaluation_path / "repos"), max_instances: Optional[int] = 5)` — [`L14`](../../../../../raw/code/claude-context/evaluation/run_evaluation.py#L14) — Main function to run custom retrieval.
- `parse_retrieval_types(value: str)` — [`L52`](../../../../../raw/code/claude-context/evaluation/run_evaluation.py#L52) — Parse comma-separated retrieval types string into list

## Module values
- `args` — [`L122`](../../../../../raw/code/claude-context/evaluation/run_evaluation.py#L122)
- `logger` — [`L11`](../../../../../raw/code/claude-context/evaluation/run_evaluation.py#L11)
- `parser` — [`L67`](../../../../../raw/code/claude-context/evaluation/run_evaluation.py#L67)

