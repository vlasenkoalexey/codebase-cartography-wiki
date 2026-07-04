---
title: 'Module: graphify/prs.py'
type: catalog
provenance: extracted
module: graphify/prs.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.prs`/
symbols:
  render_dashboard: render_dashboard().
  render_pr_detail: render_pr_detail().
  triage_with_opus: triage_with_opus().
  fetch_prs: fetch_prs().
  cmd_prs: cmd_prs().
  render_conflicts: render_conflicts().
  format_prs_text: format_prs_text().
  dim: dim().
  _classify: _classify().
  attach_graph_impact: attach_graph_impact().
  render_worktrees: render_worktrees().
  PRInfo.status: PRInfo#status().
  _status_color: _status_color().
  PRInfo.blast_radius: PRInfo#blast_radius().
  _detect_default_branch: _detect_default_branch().
  PRInfo: PRInfo#
  PRInfo.number: PRInfo#number.
  red: red().
  _parse_ci: _parse_ci().
  compute_pr_impact: compute_pr_impact().
  bold: bold().
  _ci_icon: _ci_icon().
  PRInfo.days_old: PRInfo#days_old().
  PRInfo.base_branch: PRInfo#base_branch.
  fetch_worktrees: fetch_worktrees().
  _resolve_triage_backend: _resolve_triage_backend().
  PRInfo.title: PRInfo#title.
  PRInfo.ci_status: PRInfo#ci_status.
  _c: _c().
  PRInfo.review_decision: PRInfo#review_decision.
  _path_match: _path_match().
  green: green().
  yellow: yellow().
  PRInfo.worktree_path: PRInfo#worktree_path.
  _pad: _pad().
  PRInfo.branch: PRInfo#branch.
  PRInfo.files_changed: PRInfo#files_changed.
  _STATUS_ORDER: _STATUS_ORDER.
  build_community_labels: build_community_labels().
  cyan: cyan().
  PRInfo.author: PRInfo#author.
  PRInfo.communities_touched: PRInfo#communities_touched.
  fetch_pr_files: fetch_pr_files().
  _truncate: _truncate().
  PRInfo.is_draft: PRInfo#is_draft.
  PRInfo.nodes_affected: PRInfo#nodes_affected.
  _gh: _gh().
  _load_graph_json: _load_graph_json().
  PRInfo.updated_at: PRInfo#updated_at.
  PRInfo.expected_base: PRInfo#expected_base.
  magenta: magenta().
  _TRIAGE_MODEL_DEFAULTS._TRIAGE_MODEL_DEFAULTS: _TRIAGE_MODEL_DEFAULTS._TRIAGE_MODEL_DEFAULTS.
  _NO_COLOR: _NO_COLOR.
  _ANSI_RE: _ANSI_RE.
  _STALE_DAYS: _STALE_DAYS.
  _CI_FAILURE_CONCLUSIONS: _CI_FAILURE_CONCLUSIONS.
---
# Module: [`graphify/prs.py`](../../../../../raw/code/graphify/graphify/prs.py)

## Classes
### `PRInfo`
- def: [`graphify/prs.py:64`](../../../../../raw/code/graphify/graphify/prs.py#L64) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- signature: `class PRInfo:`
- members:
  - `blast_radius(self)` — [`L90`](../../../../../raw/code/graphify/graphify/prs.py#L90) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `days_old(self)` — [`L86`](../../../../../raw/code/graphify/graphify/prs.py#L86) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `status(self)` — [`L82`](../../../../../raw/code/graphify/graphify/prs.py#L82) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `author` — [`L69`](../../../../../raw/code/graphify/graphify/prs.py#L69) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `base_branch` — [`L68`](../../../../../raw/code/graphify/graphify/prs.py#L68) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `branch` — [`L67`](../../../../../raw/code/graphify/graphify/prs.py#L67) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `ci_status` — [`L72`](../../../../../raw/code/graphify/graphify/prs.py#L72) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `communities_touched` — [`L77`](../../../../../raw/code/graphify/graphify/prs.py#L77) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `expected_base` — [`L74`](../../../../../raw/code/graphify/graphify/prs.py#L74) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `files_changed` — [`L79`](../../../../../raw/code/graphify/graphify/prs.py#L79) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `is_draft` — [`L70`](../../../../../raw/code/graphify/graphify/prs.py#L70) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `nodes_affected` — [`L78`](../../../../../raw/code/graphify/graphify/prs.py#L78) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `number` — [`L65`](../../../../../raw/code/graphify/graphify/prs.py#L65) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `review_decision` — [`L71`](../../../../../raw/code/graphify/graphify/prs.py#L71) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `title` — [`L66`](../../../../../raw/code/graphify/graphify/prs.py#L66) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `updated_at` — [`L73`](../../../../../raw/code/graphify/graphify/prs.py#L73) — documented in [graphify-prs](../../concepts/graphify-prs.md)
  - `worktree_path` — [`L75`](../../../../../raw/code/graphify/graphify/prs.py#L75) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- uses (calls/refs, reference-scoped): [`_classify`](prs.md#_classify)
- used by: [`render_dashboard`](prs.md#render_dashboard), [`_tool_triage_prs`](serve.md#_build_server._tool_triage_prs), [`render_pr_detail`](prs.md#render_pr_detail), [`triage_with_opus`](prs.md#triage_with_opus), [`fetch_prs`](prs.md#fetch_prs), [`cmd_prs`](prs.md#cmd_prs), [`render_conflicts`](prs.md#render_conflicts), [`format_prs_text`](prs.md#format_prs_text), [`_classify`](prs.md#_classify), [`attach_graph_impact`](prs.md#attach_graph_impact), [`render_worktrees`](prs.md#render_worktrees), [`_tool_list_prs`](serve.md#_build_server._tool_list_prs)  (1 test-only)

## Functions
- `_c(code: str, text: str)` — [`L40`](../../../../../raw/code/graphify/graphify/prs.py#L40) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_ci_icon(status: str)` — [`L135`](../../../../../raw/code/graphify/graphify/prs.py#L135) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_classify(pr: PRInfo, base: str = "v8")` — [`L104`](../../../../../raw/code/graphify/graphify/prs.py#L104) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_detect_default_branch(repo: str | None = None)` — [`L154`](../../../../../raw/code/graphify/graphify/prs.py#L154) — Auto-detect the repo's default branch via gh, then git, then fall back to 'main'. — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_gh(*args: str)` — [`L141`](../../../../../raw/code/graphify/graphify/prs.py#L141) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_load_graph_json(graph_path: Path)` — [`L324`](../../../../../raw/code/graphify/graphify/prs.py#L324) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_pad(s: str, width: int)` — [`L55`](../../../../../raw/code/graphify/graphify/prs.py#L55) — Pad an ANSI-colored string to visible width (strips escape codes for length calc). — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_parse_ci(rollup: list)` — [`L181`](../../../../../raw/code/graphify/graphify/prs.py#L181) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_path_match(graph_src: str, pr_file: str)` — [`L242`](../../../../../raw/code/graphify/graphify/prs.py#L242) — True if graph_src and pr_file refer to the same file (path-boundary safe).
- `_resolve_triage_backend()` — [`L559`](../../../../../raw/code/graphify/graphify/prs.py#L559) — Return (backend, model) using GRAPHIFY_TRIAGE_BACKEND or first available key. — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_status_color(status: str)` — [`L122`](../../../../../raw/code/graphify/graphify/prs.py#L122) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_truncate(s: str, n: int)` — [`L404`](../../../../../raw/code/graphify/graphify/prs.py#L404) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `attach_graph_impact(prs: list[PRInfo], graph_path: Path, repo: str | None = None)` — [`L348`](../../../../../raw/code/graphify/graphify/prs.py#L348) — Fetch PR file lists concurrently, compute graph impact, return community labels.
- `bold(t: str)` — [`L49`](../../../../../raw/code/graphify/graphify/prs.py#L49) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `build_community_labels(data: dict, top_n: int = 4)` — [`L335`](../../../../../raw/code/graphify/graphify/prs.py#L335) — Return {community_id: [top_labels]} extracted from graph node data.
- `cmd_prs(argv: list[str])` — [`L677`](../../../../../raw/code/graphify/graphify/prs.py#L677) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `compute_pr_impact(files: list[str], G: nx.Graph)` — [`L249`](../../../../../raw/code/graphify/graphify/prs.py#L249) — Return (communities_touched, nodes_affected) for a set of changed files. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `cyan(t: str)` — [`L48`](../../../../../raw/code/graphify/graphify/prs.py#L48) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `dim(t: str)` — [`L50`](../../../../../raw/code/graphify/graphify/prs.py#L50) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `fetch_pr_files(number: int, repo: str | None = None)` — [`L227`](../../../../../raw/code/graphify/graphify/prs.py#L227)
- `fetch_prs(repo: str | None = None, base: str | None = None, limit: int = 50)` — [`L195`](../../../../../raw/code/graphify/graphify/prs.py#L195) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `fetch_worktrees()` — [`L298`](../../../../../raw/code/graphify/graphify/prs.py#L298) — Returns {branch: worktree_path}. — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `format_prs_text(prs: list[PRInfo], base: str)` — [`L282`](../../../../../raw/code/graphify/graphify/prs.py#L282) — Plain-text PR summary for MCP output (no ANSI). — documented in [graphify-serve](../../concepts/graphify-serve.md)
- `green(t: str)` — [`L45`](../../../../../raw/code/graphify/graphify/prs.py#L45) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `magenta(t: str)` — [`L51`](../../../../../raw/code/graphify/graphify/prs.py#L51)
- `red(t: str)` — [`L46`](../../../../../raw/code/graphify/graphify/prs.py#L46) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `render_conflicts(prs: list[PRInfo], base: str = "v8", community_labels: dict[int, list[str]] | None = None)` — [`L487`](../../../../../raw/code/graphify/graphify/prs.py#L487)
- `render_dashboard(prs: list[PRInfo], base: str = "v8", show_wrong_base: bool = False)` — [`L408`](../../../../../raw/code/graphify/graphify/prs.py#L408) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `render_pr_detail(pr: PRInfo, repo: str | None = None)` — [`L522`](../../../../../raw/code/graphify/graphify/prs.py#L522) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `render_worktrees(prs: list[PRInfo], worktrees: dict[str, str])` — [`L465`](../../../../../raw/code/graphify/graphify/prs.py#L465)
- `triage_with_opus(prs: list[PRInfo], base: str)` — [`L584`](../../../../../raw/code/graphify/graphify/prs.py#L584) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `yellow(t: str)` — [`L47`](../../../../../raw/code/graphify/graphify/prs.py#L47) — documented in [graphify-prs](../../concepts/graphify-prs.md)

## Module values
- `_ANSI_RE` — [`L53`](../../../../../raw/code/graphify/graphify/prs.py#L53) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_CI_FAILURE_CONCLUSIONS` — [`L178`](../../../../../raw/code/graphify/graphify/prs.py#L178) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_NO_COLOR` — [`L38`](../../../../../raw/code/graphify/graphify/prs.py#L38) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_STALE_DAYS` — [`L101`](../../../../../raw/code/graphify/graphify/prs.py#L101) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_STATUS_ORDER` — [`L100`](../../../../../raw/code/graphify/graphify/prs.py#L100) — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_TRIAGE_MODEL_DEFAULTS` — [`L551`](../../../../../raw/code/graphify/graphify/prs.py#L551) — documented in [graphify-prs](../../concepts/graphify-prs.md)

