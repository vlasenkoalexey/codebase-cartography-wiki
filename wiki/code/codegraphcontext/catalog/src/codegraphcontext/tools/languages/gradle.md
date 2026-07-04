---
title: 'Module: src/codegraphcontext/tools/languages/gradle.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/gradle.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.gradle`/
symbols:
  parse_repo_gradle: parse_repo_gradle().
  GradleParser.parse: GradleParser#parse().
  _DEP_PATTERN: _DEP_PATTERN.
  GradleParser: GradleParser#
  _PROJECT_DEP_PATTERN: _PROJECT_DEP_PATTERN.
  _SETTINGS_INCLUDE_PATTERN: _SETTINGS_INCLUDE_PATTERN.
  _CONFIG_PREFIX_PATTERN: _CONFIG_PREFIX_PATTERN.
---
# Module: [`src/codegraphcontext/tools/languages/gradle.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py)

## Classes
### `GradleParser`
- def: [`src/codegraphcontext/tools/languages/gradle.py:31`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py#L31)
- doc: Parses a build.gradle / build.gradle.kts and returns build graph records.
- signature: `class GradleParser:`
- members:
  - `parse(self, gradle_path: Path)` — [`L34`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py#L34) — Parse *gradle_path* and return a dict with keys:
- uses (calls/refs, reference-scoped): [`error_logger`](../../utils/debug_log.md#error_logger), [`_DEP_PATTERN`](gradle.md#_DEP_PATTERN)
- used by: [`parse_repo_gradle`](gradle.md#parse_repo_gradle)

## Functions
- `parse_repo_gradle(repo_root: Path)` — [`L94`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py#L94) — Walk *repo_root* for build.gradle / build.gradle.kts and merge into one dict.

## Module values
- `_CONFIG_PREFIX_PATTERN` — [`L25`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py#L25)
- `_DEP_PATTERN` — [`L13`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py#L13)
- `_PROJECT_DEP_PATTERN` — [`L19`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py#L19)
- `_SETTINGS_INCLUDE_PATTERN` — [`L22`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/gradle.py#L22)

