---
title: 'Module: tree_sitter_analyzer/health_notifier.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/health_notifier.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.health_notifier`/
symbols:
  build_notifier: build_notifier().
  ShellNotifier.dispatch: ShellNotifier#dispatch().
  logger: logger.
  FileNotifier.dispatch: FileNotifier#dispatch().
  StackedNotifier.dispatch: StackedNotifier#dispatch().
  FileNotifier: FileNotifier#
  StackedNotifier._channels: StackedNotifier#_channels.
  StdoutNotifier: StdoutNotifier#
  StdoutNotifier.dispatch: StdoutNotifier#dispatch().
  Notifier: Notifier#
  ShellNotifier: ShellNotifier#
  WebhookNotifier.dispatch: WebhookNotifier#dispatch().
  StackedNotifier: StackedNotifier#
  WebhookNotifier.url: WebhookNotifier#url().
  StackedNotifier.__init__: StackedNotifier#__init__().
  FileNotifier._path: FileNotifier#_path.
  WebhookNotifier: WebhookNotifier#
  WebhookNotifier._url: WebhookNotifier#_url.
  Notifier.dispatch: Notifier#dispatch().
  SafeDict: SafeDict#
  _format_event: _format_event().
  ShellNotifier._TIMEOUT_SEC: ShellNotifier#_TIMEOUT_SEC.
  ShellNotifier._template: ShellNotifier#_template.
  WebhookNotifier.implemented: WebhookNotifier#implemented.
  _stringify: _stringify().
  SafeDict.__missing__: SafeDict#__missing__().
  FileNotifier.__init__: FileNotifier#__init__().
  ShellNotifier.__init__: ShellNotifier#__init__().
  WebhookNotifier.__init__: WebhookNotifier#__init__().
---
# Module: [`tree_sitter_analyzer/health_notifier.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py)

## Classes
### `FileNotifier`
- def: [`tree_sitter_analyzer/health_notifier.py:95`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L95)
- doc: Append one JSONL record per event to `path`.
- signature: `class FileNotifier:`
- members:
  - `dispatch(self, event: dict[str, Any])` — [`L106`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L106)
- protocol/private: `__init__`[`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L103), `_path`[`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L104)
- uses (calls/refs, reference-scoped): [`logger`](health_notifier.md#logger)
- used by: [`build_notifier`](health_notifier.md#build_notifier)  (5 test-only)

### `Notifier`  ·  implements/extends Protocol
- def: [`tree_sitter_analyzer/health_notifier.py:44`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L44)
- doc: Anything with a `dispatch` method qualifies as a notifier.
- signature: `class Notifier(Protocol):`
- members:
  - `dispatch(self, event: dict[str, Any])` — [`L47`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L47)
- used by: [`build_notifier`](health_notifier.md#build_notifier), [`dispatch`](health_notifier.md#StackedNotifier.dispatch), [`_channels`](health_notifier.md#StackedNotifier._channels), [`__init__`](health_notifier.md#StackedNotifier.__init__)

### `SafeDict`  ·  implements/extends dict
- def: [`tree_sitter_analyzer/health_notifier.py:53`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L53)
- doc: Dict subclass that returns `"{key}"` for missing tokens.
- signature: `class SafeDict(dict):`
- protocol/private: `__missing__`[`L62`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L62)
- used by: [`dispatch`](health_notifier.md#ShellNotifier.dispatch)

### `ShellNotifier`
- def: [`tree_sitter_analyzer/health_notifier.py:125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L125)
- doc: Invoke a shell-style command with event tokens substituted.
- signature: `class ShellNotifier:`
- members:
  - `dispatch(self, event: dict[str, Any])` — [`L143`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L143)
- protocol/private: `_TIMEOUT_SEC`[`L138`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L138), `__init__`[`L140`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L140), `_template`[`L141`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L141)
- uses (calls/refs, reference-scoped): [`logger`](health_notifier.md#logger), [`SafeDict`](health_notifier.md#SafeDict), [`_stringify`](health_notifier.md#_stringify)
- used by: [`build_notifier`](health_notifier.md#build_notifier)  (3 test-only)

### `StackedNotifier`
- def: [`tree_sitter_analyzer/health_notifier.py:209`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L209)
- doc: Fan an event out to multiple channels; isolate failures.
- signature: `class StackedNotifier:`
- members:
  - `dispatch(self, event: dict[str, Any])` — [`L223`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L223)
- protocol/private: `__init__`[`L212`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L212), `_channels`[`L219`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L219)
- uses (calls/refs, reference-scoped): [`logger`](health_notifier.md#logger), [`Notifier`](health_notifier.md#Notifier), [`dispatch`](health_notifier.md#Notifier.dispatch)
- used by: [`build_notifier`](health_notifier.md#build_notifier)  (2 test-only)

### `StdoutNotifier`
- def: [`tree_sitter_analyzer/health_notifier.py:80`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L80)
- doc: Print one structured line per event to stdout.
- signature: `class StdoutNotifier:`
- members:
  - `dispatch(self, event: dict[str, Any])` — [`L83`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L83)
- uses (calls/refs, reference-scoped): [`_format_event`](health_notifier.md#_format_event)
- used by: [`build_notifier`](health_notifier.md#build_notifier)  (3 test-only)

### `WebhookNotifier`
- def: [`tree_sitter_analyzer/health_notifier.py:186`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L186)
- doc: Stub: construction is fine, `dispatch` raises `NotImplementedError`.
- signature: `class WebhookNotifier:`
- members:
  - `dispatch(self, event: dict[str, Any])` — [`L202`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L202)
  - `url(self)` — [`L199`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L199)
  - `implemented` — [`L193`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L193)
- protocol/private: `__init__`[`L195`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L195), `_url`[`L196`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L196)
- used by: [`build_notifier`](health_notifier.md#build_notifier)  (1 test-only)

## Functions
- `_format_event(event: dict[str, Any])` — [`L66`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L66) — Default one-line stdout summary for an event.
- `_stringify(value: Any)` — [`L287`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L287) — Best-effort string for template substitution.
- `build_notifier(channels: list[str] | None = None, *, file_path: str | Path | None = None, webhook_url: str | None = None, shell_template: str | None = None)` — [`L238`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L238) — Build a :class:`Notifier` from CLI channel strings.

## Module values
- `logger` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/health_notifier.py#L37)

