---
title: 'Module: tests/test_obsidian_dangling_member.py'
type: catalog
provenance: extracted
module: tests/test_obsidian_dangling_member.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `tests.test_obsidian_dangling_member`/
symbols:
  test_obsidian_dangling_community_member_does_not_crash: test_obsidian_dangling_community_member_does_not_crash().
  test_canvas_dangling_community_member_does_not_crash: test_canvas_dangling_community_member_does_not_crash().
  test_obsidian_community_of_only_dangling_members: test_obsidian_community_of_only_dangling_members().
  _graph_with_dangling_member: _graph_with_dangling_member().
---
# Module: [`tests/test_obsidian_dangling_member.py`](../../../../../raw/code/graphify/tests/test_obsidian_dangling_member.py)

## Functions
- `_graph_with_dangling_member()` — [`L10`](../../../../../raw/code/graphify/tests/test_obsidian_dangling_member.py#L10) — Two real nodes plus a community that references a third, non-existent id.
- `test_canvas_dangling_community_member_does_not_crash(tmp_path)` — [`L53`](../../../../../raw/code/graphify/tests/test_obsidian_dangling_member.py#L53) — #1236 follow-up: the fix landed in to_obsidian but not to_canvas, so
- `test_obsidian_community_of_only_dangling_members(tmp_path)` — [`L41`](../../../../../raw/code/graphify/tests/test_obsidian_dangling_member.py#L41) — A community whose members are all dangling should still not crash.
- `test_obsidian_dangling_community_member_does_not_crash(tmp_path)` — [`L21`](../../../../../raw/code/graphify/tests/test_obsidian_dangling_member.py#L21) — documented in [graphify-export](../../concepts/graphify-export.md)

