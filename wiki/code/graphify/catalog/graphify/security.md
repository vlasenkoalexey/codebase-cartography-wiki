---
title: 'Module: graphify/security.py'
type: catalog
provenance: extracted
module: graphify/security.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.security`/
symbols:
  sanitize_label: sanitize_label().
  check_graph_file_size_cap: check_graph_file_size_cap().
  sanitize_metadata: sanitize_metadata().
  _sanitize_metadata_value: _sanitize_metadata_value().
  validate_url: validate_url().
  safe_fetch: safe_fetch().
  _sanitize_metadata_string: _sanitize_metadata_string().
  validate_graph_path: validate_graph_path().
  safe_fetch_text: safe_fetch_text().
  _build_opener: _build_opener().
  _ip_is_blocked: _ip_is_blocked().
  _MAX_GRAPH_FILE_BYTES: _MAX_GRAPH_FILE_BYTES.
  _METADATA_MAX_VALUE_LEN: _METADATA_MAX_VALUE_LEN.
  _resolve_and_validate: _resolve_and_validate().
  _METADATA_MAX_LIST_ITEMS: _METADATA_MAX_LIST_ITEMS.
  _max_graph_file_bytes: _max_graph_file_bytes().
  _SSRFGuardedHTTPConnection.connect: _SSRFGuardedHTTPConnection#connect().
  _SSRFGuardedHTTPSConnection.connect: _SSRFGuardedHTTPSConnection#connect().
  _SSRFGuardedHTTPHandler.http_open: _SSRFGuardedHTTPHandler#http_open().
  _SSRFGuardedHTTPSHandler.https_open: _SSRFGuardedHTTPSHandler#https_open().
  _NoFileRedirectHandler.redirect_request: _NoFileRedirectHandler#redirect_request().
  _MAX_FETCH_BYTES: _MAX_FETCH_BYTES.
  _MAX_TEXT_BYTES: _MAX_TEXT_BYTES.
  _CONTROL_CHAR_RE: _CONTROL_CHAR_RE.
  _MAX_LABEL_LEN: _MAX_LABEL_LEN.
  _ALLOWED_SCHEMES: _ALLOWED_SCHEMES.
  _BLOCKED_HOSTS: _BLOCKED_HOSTS.
  _CGN_NETWORK: _CGN_NETWORK.
  _NAT64_WKP: _NAT64_WKP.
  _SSRFGuardedHTTPConnection: _SSRFGuardedHTTPConnection#
  _SSRFGuardedHTTPSConnection: _SSRFGuardedHTTPSConnection#
  _SSRFGuardedHTTPHandler: _SSRFGuardedHTTPHandler#
  _SSRFGuardedHTTPSHandler: _SSRFGuardedHTTPSHandler#
  _NoFileRedirectHandler: _NoFileRedirectHandler#
---
# Module: [`graphify/security.py`](../../../../../raw/code/graphify/graphify/security.py)

## Classes
### `_NoFileRedirectHandler`  ·  implements/extends HTTPRedirectHandler
- def: [`graphify/security.py:230`](../../../../../raw/code/graphify/graphify/security.py#L230)
- doc: Redirect handler that re-validates every redirect target.
- signature: `class _NoFileRedirectHandler(urllib.request.HTTPRedirectHandler):`
- members:
  - `redirect_request(self, req, fp, code, msg, headers, newurl)` — [`L237`](../../../../../raw/code/graphify/graphify/security.py#L237)
- uses (calls/refs, reference-scoped): [`validate_url`](security.md#validate_url)
- used by: [`_build_opener`](security.md#_build_opener)

### `_SSRFGuardedHTTPConnection`  ·  implements/extends HTTPConnection
- def: [`graphify/security.py:179`](../../../../../raw/code/graphify/graphify/security.py#L179)
- doc: HTTPConnection that resolves + validates DNS once, then connects to the
- signature: `class _SSRFGuardedHTTPConnection(http.client.HTTPConnection):`
- members:
  - `connect(self)` — [`L183`](../../../../../raw/code/graphify/graphify/security.py#L183)
- uses (calls/refs, reference-scoped): [`_resolve_and_validate`](security.md#_resolve_and_validate)
- used by: [`http_open`](security.md#_SSRFGuardedHTTPHandler.http_open)

### `_SSRFGuardedHTTPHandler`  ·  implements/extends HTTPHandler
- def: [`graphify/security.py:216`](../../../../../raw/code/graphify/graphify/security.py#L216)
- doc: urllib handler that routes http:// through _SSRFGuardedHTTPConnection.
- signature: `class _SSRFGuardedHTTPHandler(urllib.request.HTTPHandler):`
- members:
  - `http_open(self, req)` — [`L219`](../../../../../raw/code/graphify/graphify/security.py#L219)
- uses (calls/refs, reference-scoped): [`_SSRFGuardedHTTPConnection`](security.md#_SSRFGuardedHTTPConnection)
- used by: [`_build_opener`](security.md#_build_opener)

### `_SSRFGuardedHTTPSConnection`  ·  implements/extends HTTPSConnection
- def: [`graphify/security.py:194`](../../../../../raw/code/graphify/graphify/security.py#L194)
- doc: HTTPSConnection variant of _SSRFGuardedHTTPConnection.
- signature: `class _SSRFGuardedHTTPSConnection(http.client.HTTPSConnection):`
- members:
  - `connect(self)` — [`L202`](../../../../../raw/code/graphify/graphify/security.py#L202)
- uses (calls/refs, reference-scoped): [`_resolve_and_validate`](security.md#_resolve_and_validate)
- used by: [`https_open`](security.md#_SSRFGuardedHTTPSHandler.https_open)

### `_SSRFGuardedHTTPSHandler`  ·  implements/extends HTTPSHandler
- def: [`graphify/security.py:223`](../../../../../raw/code/graphify/graphify/security.py#L223)
- doc: urllib handler that routes https:// through _SSRFGuardedHTTPSConnection.
- signature: `class _SSRFGuardedHTTPSHandler(urllib.request.HTTPSHandler):`
- members:
  - `https_open(self, req)` — [`L226`](../../../../../raw/code/graphify/graphify/security.py#L226)
- uses (calls/refs, reference-scoped): [`_SSRFGuardedHTTPSConnection`](security.md#_SSRFGuardedHTTPSConnection)
- used by: [`_build_opener`](security.md#_build_opener)

## Functions
- `_build_opener()` — [`L242`](../../../../../raw/code/graphify/graphify/security.py#L242)
- `_ip_is_blocked(ip: ipaddress.IPv4Address | ipaddress.IPv6Address)` — [`L82`](../../../../../raw/code/graphify/graphify/security.py#L82) — Return True if *ip* falls in a private/reserved/internal range.
- `_max_graph_file_bytes()` — [`L35`](../../../../../raw/code/graphify/graphify/security.py#L35) — Return the graph.json size cap in bytes. — documented in [graphify-security](../../concepts/graphify-security.md)
- `_resolve_and_validate(host: str, port: int)` — [`L157`](../../../../../raw/code/graphify/graphify/security.py#L157) — Resolve *host* once and return (family, validated_ip) for the first
- `_sanitize_metadata_string(value: object)` — [`L415`](../../../../../raw/code/graphify/graphify/security.py#L415) — Return a control-character-free, HTML-escaped, bounded string. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_sanitize_metadata_value(value: object)` — [`L424`](../../../../../raw/code/graphify/graphify/security.py#L424) — Sanitize a metadata value while preserving simple JSON-compatible types. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `check_graph_file_size_cap(path: Path)` — [`L356`](../../../../../raw/code/graphify/graphify/security.py#L356) — Reject *path* if its size exceeds the configured graph-file cap. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `safe_fetch(url: str, max_bytes: int = _MAX_FETCH_BYTES, timeout: int = 30)` — [`L257`](../../../../../raw/code/graphify/graphify/security.py#L257) — Fetch *url* and return raw bytes.
- `safe_fetch_text(url: str, max_bytes: int = _MAX_TEXT_BYTES, timeout: int = 15)` — [`L301`](../../../../../raw/code/graphify/graphify/security.py#L301) — Fetch *url* and return decoded text (UTF-8, replacing bad bytes).
- `sanitize_label(text: str | None)` — [`L393`](../../../../../raw/code/graphify/graphify/security.py#L393) — Strip control characters and cap length. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `sanitize_metadata(metadata: Mapping[str, Any] | None)` — [`L440`](../../../../../raw/code/graphify/graphify/security.py#L440) — Sanitize metadata keys and values before graph export. — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `validate_graph_path(path: str | Path, base: Path | None = None)` — [`L314`](../../../../../raw/code/graphify/graphify/security.py#L314) — Resolve *path* and verify it stays inside *base*.
- `validate_url(url: str)` — [`L102`](../../../../../raw/code/graphify/graphify/security.py#L102) — Raise ValueError if *url* is not http or https, or targets a private/internal IP.

## Module values
- `_ALLOWED_SCHEMES` — [`L20`](../../../../../raw/code/graphify/graphify/security.py#L20)
- `_BLOCKED_HOSTS` — [`L68`](../../../../../raw/code/graphify/graphify/security.py#L68)
- `_CGN_NETWORK` — [`L71`](../../../../../raw/code/graphify/graphify/security.py#L71)
- `_CONTROL_CHAR_RE` — [`L389`](../../../../../raw/code/graphify/graphify/security.py#L389) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_MAX_FETCH_BYTES` — [`L21`](../../../../../raw/code/graphify/graphify/security.py#L21)
- `_MAX_GRAPH_FILE_BYTES` — [`L32`](../../../../../raw/code/graphify/graphify/security.py#L32) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_MAX_LABEL_LEN` — [`L390`](../../../../../raw/code/graphify/graphify/security.py#L390) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_MAX_TEXT_BYTES` — [`L22`](../../../../../raw/code/graphify/graphify/security.py#L22)
- `_METADATA_MAX_LIST_ITEMS` — [`L412`](../../../../../raw/code/graphify/graphify/security.py#L412) — documented in [graphify-security](../../concepts/graphify-security.md)
- `_METADATA_MAX_VALUE_LEN` — [`L411`](../../../../../raw/code/graphify/graphify/security.py#L411) — documented in [graphify-scip_ingest](../../concepts/graphify-scip_ingest.md)
- `_NAT64_WKP` — [`L75`](../../../../../raw/code/graphify/graphify/security.py#L75)

