---
title: 'Module: src/codegraphcontext/utils/cypher_readonly.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/utils/cypher_readonly.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.utils.cypher_readonly`/
symbols:
  is_read_only_cypher: is_read_only_cypher().
  read_only_rejection_message: read_only_rejection_message().
  _strip_comments: _strip_comments().
  strip_string_literals: strip_string_literals().
  _FORBIDDEN_KEYWORDS: _FORBIDDEN_KEYWORDS.
  _FORBIDDEN_PATTERNS: _FORBIDDEN_PATTERNS.
  _STRING_LITERAL_RE: _STRING_LITERAL_RE.
  _LINE_COMMENT_RE: _LINE_COMMENT_RE.
  _BLOCK_COMMENT_RE: _BLOCK_COMMENT_RE.
---
# Module: [`src/codegraphcontext/utils/cypher_readonly.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py)

## Functions
- `_strip_comments(query: str)` — [`L40`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L40)
- `is_read_only_cypher(query: str)` — [`L45`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L45) — Return True when *query* has no write keywords outside string literals.
- `read_only_rejection_message()` — [`L61`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L61)
- `strip_string_literals(query: str)` — [`L36`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L36)

## Module values
- `_BLOCK_COMMENT_RE` — [`L33`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L33)
- `_FORBIDDEN_KEYWORDS` — [`L6`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L6)
- `_FORBIDDEN_PATTERNS` — [`L24`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L24)
- `_LINE_COMMENT_RE` — [`L32`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L32)
- `_STRING_LITERAL_RE` — [`L31`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/cypher_readonly.py#L31)

