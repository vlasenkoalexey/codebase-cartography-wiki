---
title: 'Module: tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.grammar_coverage.grammar_snapshot`/
symbols:
  take_snapshot: take_snapshot().
  diff_snapshot: diff_snapshot().
  s: s.
  load_snapshot: load_snapshot().
  check_snapshot: check_snapshot().
  snaps: snaps.
  LanguageSnapshot: LanguageSnapshot#
  parser: parser.
  args: args.
  SnapshotDiff.added: SnapshotDiff#added.
  SnapshotDiff.has_changes: SnapshotDiff#has_changes().
  _get_package_version: _get_package_version().
  SnapshotDiff.removed: SnapshotDiff#removed.
  snap_path: snap_path.
  SnapshotDiff: SnapshotDiff#
  _save_snapshot: _save_snapshot().
  langs: langs.
  LanguageSnapshot.node_types: LanguageSnapshot#node_types.
  LanguageSnapshot.node_count: LanguageSnapshot#node_count.
  LanguageSnapshot.package_version: LanguageSnapshot#package_version.
  SnapshotDiff.has_new_nodes: SnapshotDiff#has_new_nodes().
  DEFAULT_SNAPSHOT_PATH: DEFAULT_SNAPSHOT_PATH.
  LanguageSnapshot.language: LanguageSnapshot#language.
  SnapshotDiff.unchanged: SnapshotDiff#unchanged.
  SnapshotDiff.language: SnapshotDiff#language.
  KNOWN_LEGACY_NODES.KNOWN_LEGACY_NODES: KNOWN_LEGACY_NODES.KNOWN_LEGACY_NODES.
  lang: lang.
---
# Module: [`tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py)

## Classes
### `LanguageSnapshot`
- def: [`tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py:37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L37)
- doc: 单个语言的 grammar 快照.
- signature: `class LanguageSnapshot:`
- members:
  - `language` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L40)
  - `node_count` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L42)
  - `node_types` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L41)
  - `package_version` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L43)
- used by: [`take_snapshot`](grammar_snapshot.md#take_snapshot), [`diff_snapshot`](grammar_snapshot.md#diff_snapshot), [`s`](grammar_snapshot.md#s), [`load_snapshot`](grammar_snapshot.md#load_snapshot), [`_save_snapshot`](grammar_snapshot.md#_save_snapshot)

### `SnapshotDiff`
- def: [`tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py:47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L47)
- doc: 两个快照之间的差异.
- signature: `class SnapshotDiff:`
- members:
  - `has_changes(self)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L56)
  - `has_new_nodes(self)` — [`L60`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L60)
  - `added` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L51)
  - `language` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L50)
  - `removed` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L52)
  - `unchanged` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L53)
- used by: [`diff_snapshot`](grammar_snapshot.md#diff_snapshot), [`check_snapshot`](grammar_snapshot.md#check_snapshot)

## Functions
- `_get_package_version(language: str)` — [`L64`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L64) — 获取 tree-sitter 语言包版本号.
- `_save_snapshot(snapshots: dict[str, LanguageSnapshot], path: Path)` — [`L283`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L283) — 将快照序列化写入 JSON 文件.
- `check_snapshot(baseline_path: Path | None = None, fail_on_new: bool = True, verbose: bool = True)` — [`L221`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L221) — CI 入口：检查当前 grammar 是否与基线一致.
- `diff_snapshot(baseline: dict[str, LanguageSnapshot], languages: list[str] | None = None)` — [`L176`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L176) — 对比当前 grammar 与基线快照的差异.
- `load_snapshot(path: Path | None = None)` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L120) — 从文件加载 grammar 快照.
- `take_snapshot(languages: list[str] | None = None, output_path: Path | None = None)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L83) — 生成并保存当前 grammar 快照.

## Module values
- `DEFAULT_SNAPSHOT_PATH` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L29)
- `KNOWN_LEGACY_NODES` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L33)
- `args` — [`L307`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L307)
- `lang` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L315)
- `langs` — [`L310`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L310)
- `parser` — [`L298`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L298)
- `s` — [`L315`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L315)
- `snap_path` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L309)
- `snaps` — [`L313`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/grammar_snapshot.py#L313)

