---
title: 'Module: gitgalaxy/core/state_rehydrator.py'
type: catalog
provenance: extracted
module: gitgalaxy/core/state_rehydrator.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.core.state_rehydrator`/StateRehydrator#
symbols:
  StateRehydrator.load_latest_state: load_latest_state().
  StateRehydrator: ''
  StateRehydrator.db_path: db_path.
  StateRehydrator.__init__: __init__().
---
# Module: [`gitgalaxy/core/state_rehydrator.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/state_rehydrator.py)

## Classes
### `StateRehydrator`
- def: [`gitgalaxy/core/state_rehydrator.py:16`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/state_rehydrator.py#L16)
- doc: Restores the GitGalaxy engine's memory state from a previous SQLite audit.
- signature: `class StateRehydrator:`
- members:
  - `load_latest_state(self, repo_name: str)` — [`L30`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/state_rehydrator.py#L30) — Pulls the most recent commit state from SQLite and rebuilds the RAM dictionary.
  - `db_path` — [`L28`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/state_rehydrator.py#L28)
- protocol/private: `__init__`[`L27`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/state_rehydrator.py#L27)
- used by: (3 test-only callers)

