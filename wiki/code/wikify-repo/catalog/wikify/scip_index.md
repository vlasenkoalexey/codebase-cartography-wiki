---
title: 'Module: wikify/scip_index.py'
type: catalog
provenance: extracted
module: wikify/scip_index.py
status: fresh
symbol_base: scip-python python wikify-repo 0.0.0 `wikify.scip_index`/
symbols:
  build_graph: build_graph().
  _process_document: _process_document().
  _synth_symbol: _synth_symbol().
  run_indexer_sharded: run_indexer_sharded().
  parse_index: parse_index().
  index_repo: index_repo().
  Range: Range.
  run_indexer: run_indexer().
  _merge_shards_index: _merge_shards_index().
  _path_from_moniker: _path_from_moniker().
  _has_documents: _has_documents().
  merge_shards: merge_shards().
  _run_scip_tool: _run_scip_tool().
  run_clang_indexer: run_clang_indexer().
  _span_size: _span_size().
  _NODE_HEAP_MB: _NODE_HEAP_MB.
  run_indexer_sharded._one: run_indexer_sharded()._one().
  _repair_doc_path: _repair_doc_path().
  run_scip_typescript: run_scip_typescript().
  run_scip_go: run_scip_go().
  run_rust_analyzer: run_rust_analyzer().
  _occ_range: _occ_range().
  _occ_enclosing: _occ_enclosing().
  _contains: _contains().
  _DEFINITION: _DEFINITION.
  _LOCALISH_SUFFIXES: _LOCALISH_SUFFIXES.
  _IMPORT: _IMPORT.
  _KIND_NAME: _KIND_NAME.
  _SUFFIX_KIND: _SUFFIX_KIND.
  _missing_target_files: _missing_target_files().
  _signature: _signature().
---
# Module: [`wikify/scip_index.py`](../../../../../raw/code/wikify-repo/wikify/scip_index.py)

## Functions
- `_contains(span: Range, point: tuple[int, int])` — [`L414`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L414) — Is (line, char) within half-open span [start, end)? — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_has_documents(scip_path: Path)` — [`L102`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L102) — True if ``scip_path`` exists and parses to a non-empty SCIP index. — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `_merge_shards_index(project_dir: str | Path, shards: list[tuple[str, Path]])` — [`L167`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L167) — Union shard ``.scip`` files into one Index, repairing target-relative paths. — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_missing_target_files(project_dir: str | Path, targets: list[str], emitted: set[str])` — [`L259`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L259) — Repo-relative ``.py`` files under ``targets`` that ``emitted`` doesn't cover.
- `_occ_enclosing(occ)` — [`L398`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L398) — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_occ_range(occ)` — [`L382`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L382) — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_one(item: tuple[int, str])` — [`L132`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L132)
- `_path_from_moniker(doc, project_dir: Path)` — [`L227`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L227) — Derive a repo-relative file path from a document's symbol monikers.
- `_process_document(g: SymbolGraph, doc)` — [`L533`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L533) — documented in [wikify-graph](../../concepts/wikify-graph.md)
- `_repair_doc_path(doc, project_dir: Path, base: str)` — [`L205`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L205) — Restore a shard document's ``relative_path`` to repo-relative, in place.
- `_run_scip_tool(cmd: list[str], cwd: str | Path, output_path: str | Path, tool: str, produces: str | None = None)` — [`L332`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L332) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `_signature(si)` — [`L426`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L426) — Best-effort signature: first fenced code block in the documentation.
- `_span_size(span: Range)` — [`L421`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L421) — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_synth_symbol(moniker: str)` — [`L510`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L510) — Build a minimal Symbol from a moniker alone (no SymbolInformation). — documented in [wikify-graph](../../concepts/wikify-graph.md)
- `build_graph(*indexes)` — [`L442`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L442) — Build one SymbolGraph from one OR MORE SCIP indexes. — documented in [wikify-cli](../../concepts/wikify-cli.md)
- `index_repo(project_dir: str | Path, output_path: str | Path, project_name: str | None = None)` — [`L587`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L587) — End-to-end: run the indexer, parse, build the graph. — documented in [wikify-graph](../../concepts/wikify-graph.md)
- `merge_shards(project_dir: str | Path, shards: list[tuple[str, Path]], output_path: str | Path)` — [`L247`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L247) — Union shard ``.scip`` files into ``output_path`` (path-writing wrapper).
- `parse_index(scip_path: str | Path)` — [`L373`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L373) — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `run_clang_indexer(project_root: str | Path, compile_commands_path: str | Path, output_path: str | Path, scip_clang_bin: str = "scip-clang")` — [`L277`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L277) — Invoke ``scip-clang`` against a ``compile_commands.json`` → ``output_path`` (.scip).
- `run_indexer(project_dir: str | Path, output_path: str | Path, project_name: str | None = None, project_version: str = "0.0.0", target_only: str | None = None, heap_mb: str | int | None = None)` — [`L56`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L56) — Invoke ``scip-python index`` on ``project_dir`` → ``output_path`` (.scip).
- `run_indexer_sharded(project_dir: str | Path, output_path: str | Path, targets: list[str], project_name: str | None = None, project_version: str = "0.0.0", max_parallel: int = 8, heap_mb: str | int | None = None)` — [`L110`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L110) — Index ``targets`` concurrently (one scip-python per ``--target-only``), then — documented in [wikify-ast_fallback](../../concepts/wikify-ast_fallback.md)
- `run_rust_analyzer(project_dir: str | Path, output_path: str | Path, bin: str = "rust-analyzer")` — [`L366`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L366) — rust-analyzer scip (Rust). It writes ``index.scip`` into cwd; we relocate it out. — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `run_scip_go(project_dir: str | Path, output_path: str | Path, bin: str = "scip-go")` — [`L359`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L359) — scip-go (Go). Run from the module root (needs ``go.mod`` + a Go toolchain). — documented in [wikify-languages](../../concepts/wikify-languages.md)
- `run_scip_typescript(project_dir: str | Path, output_path: str | Path, bin: str = "scip-typescript")` — [`L349`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L349) — scip-typescript (TS/JS). Uses a root ``tsconfig.json`` if present, else infers one. — documented in [wikify-languages](../../concepts/wikify-languages.md)

## Module values
- `Range` — [`L35`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L35) — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_DEFINITION` — [`L29`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L29) — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_IMPORT` — [`L30`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L30)
- `_KIND_NAME` — [`L33`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L33)
- `_LOCALISH_SUFFIXES` — [`L38`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L38) — documented in [wikify-scip_index](../../concepts/wikify-scip_index.md)
- `_NODE_HEAP_MB` — [`L25`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L25)
- `_SUFFIX_KIND` — [`L44`](../../../../../raw/code/wikify-repo/wikify/scip_index.py#L44)

