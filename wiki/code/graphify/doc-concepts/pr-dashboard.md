---
title: The PR dashboard
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# The PR dashboard

## Definition
`graphify prs` applies the graph to code review. The bare command is a dashboard (CI state, review status, worktree→branch→PR mapping); `graphify prs 42` is a deep dive on one PR with its graph impact; `graphify prs --triage` uses an LLM to rank your review queue; and `graphify prs --conflicts` finds PRs that touch the same graph communities — i.e. merge-order risk that file-level diffs miss.

## In graphify (grounded)
- The command is `prs.py`: [`cmd_prs`](../catalog/graphify/prs.md#cmd_prs) dispatches to [`render_dashboard`](../catalog/graphify/prs.md#render_dashboard), [`render_pr_detail`](../catalog/graphify/prs.md#render_pr_detail), [`render_worktrees`](../catalog/graphify/prs.md#render_worktrees), and [`render_conflicts`](../catalog/graphify/prs.md#render_conflicts).
- GitHub data is pulled via [`fetch_prs`](../catalog/graphify/prs.md#fetch_prs) / [`fetch_pr_files`](../catalog/graphify/prs.md#fetch_pr_files) / [`fetch_worktrees`](../catalog/graphify/prs.md#fetch_worktrees) (the `gh` CLI).
- The graph tie-in is [`compute_pr_impact`](../catalog/graphify/prs.md#compute_pr_impact) / [`attach_graph_impact`](../catalog/graphify/prs.md#attach_graph_impact) — mapping changed files to affected nodes/communities — and triage ranking is [`triage_with_opus`](../catalog/graphify/prs.md#triage_with_opus). The same data is exposed to MCP as `list_prs` / `get_pr_impact` / `triage_prs`.

## Why it matters / when it applies
The `--conflicts` view is the clearest example of graph-native comprehension paying off in a real workflow: two PRs that never touch the same file can still collide because they share a community, and only the graph sees that. It shows the persistent graph being reused for a second, distinct question class beyond "how does this code work".

## Connections
- Code concepts: [prs](../concepts/graphify-prs.md), [serve](../concepts/graphify-serve.md)
- Module catalogs: [prs](../catalog/graphify/prs.md), [serve](../catalog/graphify/serve.md)
- Related doc-concepts: [mcp-server](mcp-server.md), [community-detection](community-detection.md)

## Source
Extracted from `README.md` ("Common commands", "Full command reference") (kept in place).
