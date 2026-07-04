---
title: 'Module: src/codegraphcontext/tools/scip_indexer.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/scip_indexer.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.scip_indexer`/
symbols:
  ScipIndexer.run: ScipIndexer#run().
  ScipIndexParser.parse: ScipIndexParser#parse().
  ScipIndexer._build_command: ScipIndexer#_build_command().
  EXTENSION_TO_SCIP.EXTENSION_TO_SCIP: EXTENSION_TO_SCIP.EXTENSION_TO_SCIP.
  detect_project_lang: detect_project_lang().
  ScipIndexParser._name_from_symbol: ScipIndexParser#_name_from_symbol().
  is_scip_available: is_scip_available().
  ScipIndexer._get_binary: ScipIndexer#_get_binary().
  ScipIndexer._find_csharp_project: ScipIndexer#_find_csharp_project().
  ScipIndexParser._lang_from_path: ScipIndexParser#_lang_from_path().
  ScipIndexer: ScipIndexer#
  ScipIndexer._find_compdb: ScipIndexer#_find_compdb().
  ScipIndexParser._infer_cxx_zero_kind: ScipIndexParser#_infer_cxx_zero_kind().
  ScipIndexer._resolve_compdb_paths: ScipIndexer#_resolve_compdb_paths().
  ScipIndexer._compdb_host_paths_to_container: ScipIndexer#_compdb_host_paths_to_container().
  ScipIndexParser._parse_signature: ScipIndexParser#_parse_signature().
  ScipIndexParser._find_enclosing_definition: ScipIndexParser#_find_enclosing_definition().
  ScipIndexParser: ScipIndexParser#
---
# Module: [`src/codegraphcontext/tools/scip_indexer.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py)

## Classes
### `ScipIndexParser`
- def: [`src/codegraphcontext/tools/scip_indexer.py:438`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L438)
- doc: Parses an index.scip (Protobuf) file and extracts function calls,
- signature: `class ScipIndexParser:`
- members:
  - `_infer_cxx_zero_kind(self, sym: str, line: int, source_lines: List[str])` — [`L693`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L693) — Infer SCIP SymbolKind when indexer reports 0 (scip-clang). Returns SCIP kind int.
  - `parse(self, index_scip_path: Path, project_path: Path)` — [`L444`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L444)
- protocol/private: `_find_enclosing_definition`[`L747`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L747), `_lang_from_path`[`L726`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L726), `_name_from_symbol`[`L676`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L676), `_parse_signature`[`L732`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L732)
- uses (calls/refs, reference-scoped): [`error_logger`](../utils/debug_log.md#error_logger), [`Index`](scip_pb2.md#Index), [`EXTENSION_TO_SCIP`](scip_indexer.md#EXTENSION_TO_SCIP.EXTENSION_TO_SCIP)

### `ScipIndexer`
- def: [`src/codegraphcontext/tools/scip_indexer.py:124`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L124)
- doc: Handles running the external SCIP indexer binaries.
- signature: `class ScipIndexer:`
- members:
  - `_build_command(self, lang: str, binary: str, project_path: Path, output_file: Path, scratch_dir: Optional[Path] = None)` — [`L359`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L359) — Build the CLI command for each supported SCIP indexer.
  - `_compdb_host_paths_to_container(compdb_host_path: str, project_host: Path, out_dir_host: Path)` — [`L328`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L328) — Rewrite compile_commands.json so directory/file use /src paths for Docker.
  - `_find_compdb(project_path: Path)` — [`L270`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L270) — Search for compile_commands.json in common locations relative to project_path.
  - `_find_csharp_project(project_path: Path)` — [`L350`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L350) — Find the first .sln or .csproj file for scip-dotnet.
  - `_resolve_compdb_paths(compdb_path: str, project_path: Path, scratch_dir: Optional[Path])` — [`L286`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L286) — Ensure all 'directory' fields in the compile_commands.json are absolute.
  - `run(self, project_path: Path, lang: str, output_dir: Path)` — [`L131`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L131) — Run the SCIP indexer for `lang` on `project_path`.
- protocol/private: `_get_binary`[`L262`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L262)
- uses (calls/refs, reference-scoped): [`info_logger`](../utils/debug_log.md#info_logger), [`warning_logger`](../utils/debug_log.md#warning_logger), [`error_logger`](../utils/debug_log.md#error_logger), [`file_path_has_ignore_dir_segment`](../utils/path_ignore.md#file_path_has_ignore_dir_segment), [`EXTENSION_TO_SCIP`](scip_indexer.md#EXTENSION_TO_SCIP.EXTENSION_TO_SCIP)
- used by: [`build_graph_from_path_async`](graph_builder.md#GraphBuilder.build_graph_from_path_async)

## Functions
- `detect_project_lang(path: Path, scip_languages: List[str])` — [`L99`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L99) — Detect the primary language of a project folder by counting files.
- `is_scip_available(lang: str)` — [`L87`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L87) — Check whether the SCIP indexer (binary or docker) for this language is available.

## Module values
- `EXTENSION_TO_SCIP` — [`L54`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/scip_indexer.py#L54)

