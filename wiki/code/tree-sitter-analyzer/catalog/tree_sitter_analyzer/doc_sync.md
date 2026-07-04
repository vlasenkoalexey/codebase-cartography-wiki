---
title: 'Module: tree_sitter_analyzer/doc_sync.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/doc_sync.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.doc_sync`/
symbols:
  extract_file_refs: extract_file_refs().
  run_doc_sync: run_doc_sync().
  validate_file_refs: validate_file_refs().
  DocRef.path: DocRef#path.
  DocRef: DocRef#
  StaleRef.ref: StaleRef#ref.
  DocRef.line: DocRef#line.
  DocRef.doc_file: DocRef#doc_file.
  _has_validatable_ext: _has_validatable_ext().
  StaleRef: StaleRef#
  StaleRef.reason: StaleRef#reason.
  _VALIDATABLE_EXTS: _VALIDATABLE_EXTS.
  _BACKTICK_RE: _BACKTICK_RE.
  _LINK_TARGET_RE: _LINK_TARGET_RE.
  _is_skippable: _is_skippable().
  _resolve_ref: _resolve_ref().
  _collect_md_files: _collect_md_files().
---
# Module: [`tree_sitter_analyzer/doc_sync.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py)

## Classes
### `DocRef`
- def: [`tree_sitter_analyzer/doc_sync.py:28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L28)
- doc: A file-path reference found in a documentation file.
- signature: `class DocRef:`
- members:
  - `doc_file` — [`L32`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L32)
  - `line` — [`L33`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L33)
  - `path` — [`L31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L31)
- used by: [`_add_markdown_links`](knowledge_graph/builder.md#KnowledgeGraphBuilder._add_markdown_links), [`extract_file_refs`](doc_sync.md#extract_file_refs), [`run_doc_sync`](doc_sync.md#run_doc_sync), [`validate_file_refs`](doc_sync.md#validate_file_refs), [`ref`](doc_sync.md#StaleRef.ref)  (9 test-only)

### `StaleRef`
- def: [`tree_sitter_analyzer/doc_sync.py:37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L37)
- doc: A DocRef that could not be resolved to an existing file.
- signature: `class StaleRef:`
- members:
  - `reason` — [`L41`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L41)
  - `ref` — [`L40`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L40)
- uses (calls/refs, reference-scoped): [`DocRef`](doc_sync.md#DocRef)
- used by: [`run_doc_sync`](doc_sync.md#run_doc_sync), [`validate_file_refs`](doc_sync.md#validate_file_refs)  (2 test-only)

## Functions
- `_collect_md_files(project_root: str, patterns: list[str])` — [`L152`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L152) — Resolve glob *patterns* relative to *project_root*.
- `_has_validatable_ext(text: str)` — [`L44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L44)
- `_is_skippable(text: str)` — [`L56`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L56) — True for globs, URLs, anchors, bare directories, templates, or non-path spans.
- `_resolve_ref(path: str, doc_file: str, project_root: str)` — [`L120`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L120) — Return True if *path* can be resolved to an existing file.
- `extract_file_refs(content: str, doc_file: str)` — [`L81`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L81) — Extract file-path references from markdown *content*.
- `run_doc_sync(project_root: str, doc_patterns: list[str] | None = None)` — [`L161`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L161) — Scan markdown docs under *project_root* for stale file-path references.
- `validate_file_refs(refs: list[DocRef], project_root: str)` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L143) — Check each *ref* against the filesystem; return those that are missing.

## Module values
- `_BACKTICK_RE` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L21)
- `_LINK_TARGET_RE` — [`L24`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L24)
- `_VALIDATABLE_EXTS` — [`L16`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/doc_sync.py#L16)

