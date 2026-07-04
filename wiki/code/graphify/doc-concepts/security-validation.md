---
title: Input security validation
type: doc-concept
provenance: doc
source: ARCHITECTURE.md
updated: 2026-07-04
status: fresh
---
# Input security validation

## Definition
All external input passes through `graphify/security.py` before use. URLs are restricted to http/https and protected against `file://` redirects; fetched content is size- and timeout-capped; graph file paths must resolve inside `graphify-out/`; and node labels are sanitized (control chars stripped, capped at 256 chars, HTML-escaped). This is graphify's trust boundary — because ingestion pulls in arbitrary files, papers, and URLs, everything that crosses in is validated first.

## In graphify (grounded)
- URL validation is [`validate_url`](../catalog/graphify/security.md#validate_url) (http/https only) with the redirect guard [`_NoFileRedirectHandler`](../catalog/graphify/security.md#_NoFileRedirectHandler.redirect_request) and SSRF-guarded openers.
- Bounded fetching is [`safe_fetch`](../catalog/graphify/security.md#safe_fetch) / [`safe_fetch_text`](../catalog/graphify/security.md#safe_fetch_text) (`_MAX_FETCH_BYTES`, timeout).
- Graph-path containment is [`validate_graph_path`](../catalog/graphify/security.md#validate_graph_path); the size cap is [`check_graph_file_size_cap`](../catalog/graphify/security.md#check_graph_file_size_cap).
- Label sanitization is [`sanitize_label`](../catalog/graphify/security.md#sanitize_label) (and [`sanitize_metadata`](../catalog/graphify/security.md#sanitize_metadata) for metadata strings).

## Why it matters / when it applies
The validators are what let graphify safely ingest untrusted input — `graphify add <url>`, fetched papers, foreign `graph.json` files pointed at by `serve` — without SSRF, path traversal, oversized-download, or HTML-injection risks. The MCP server reuses `validate_graph_path` when loading a graph.

## Connections
- Code concepts: [security](../concepts/graphify-security.md), [serve](../concepts/graphify-serve.md)
- Module catalogs: [security](../catalog/graphify/security.md)
- Related doc-concepts: [multi-source-ingestion](multi-source-ingestion.md), [mcp-server](mcp-server.md)

## Source
Extracted from `ARCHITECTURE.md` ("Security"); the doc points to `SECURITY.md` for the full threat model (kept in place).
