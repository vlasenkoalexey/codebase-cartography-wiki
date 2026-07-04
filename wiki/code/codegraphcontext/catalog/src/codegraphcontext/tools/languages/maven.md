---
title: 'Module: src/codegraphcontext/tools/languages/maven.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/maven.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.maven`/
symbols:
  MavenParser.parse: MavenParser#parse().
  _text: _text().
  parse_repo_maven: parse_repo_maven().
  _ns: _ns().
  _MVN_NS: _MVN_NS.
  MavenParser: MavenParser#
  MavenParser._resolve_version: MavenParser#_resolve_version().
---
# Module: [`src/codegraphcontext/tools/languages/maven.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py)

## Classes
### `MavenParser`
- def: [`src/codegraphcontext/tools/languages/maven.py:27`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py#L27)
- doc: Parses a pom.xml file and returns structured build graph data.
- signature: `class MavenParser:`
- members:
  - `parse(self, pom_path: Path)` — [`L30`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py#L30) — Parse *pom_path* and return a dict compatible with GraphWriter.write_maven_build_graph().
- protocol/private: `_resolve_version`[`L93`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py#L93)
- uses (calls/refs, reference-scoped): [`error_logger`](../../utils/debug_log.md#error_logger), [`_text`](maven.md#_text), [`_ns`](maven.md#_ns), [`_MVN_NS`](maven.md#_MVN_NS)
- used by: [`parse_repo_maven`](maven.md#parse_repo_maven)

## Functions
- `_ns(tag: str)` — [`L15`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py#L15) — Return a namespace-qualified tag, e.g. 'groupId' -> '{http://...}groupId'.
- `_text(element: Any, tag: str, default: str = "")` — [`L20`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py#L20)
- `parse_repo_maven(repo_root: Path)` — [`L142`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py#L142) — Walk *repo_root* for all pom.xml files and merge into a single build graph dict.

## Module values
- `_MVN_NS` — [`L12`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/maven.py#L12)

