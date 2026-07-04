---
title: 'Module: understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py'
type: catalog
provenance: extracted
module: understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py
status: fresh
symbol_base: scip-python python understand-anything 0.0.0 `understand-anything-plugin.skills.understand-knowledge.parse-knowledge-base`/
symbols:
  parse_wiki: parse_wiki().
  extract_first_paragraph: extract_first_paragraph().
  extract_frontmatter: extract_frontmatter().
  extract_wikilinks: extract_wikilinks().
  extract_headings: extract_headings().
  extract_code_blocks: extract_code_blocks().
  extract_h1: extract_h1().
  parse_index: parse_index().
  main: main().
  WIKILINK_RE: WIKILINK_RE.
  FRONTMATTER_RE: FRONTMATTER_RE.
  HEADING_RE: HEADING_RE.
  INFRA_FILES: INFRA_FILES.
  extract_first_paragraph._collect_paragraph: extract_first_paragraph()._collect_paragraph().
  resolve_wikilink: resolve_wikilink().
  CODE_BLOCK_RE: CODE_BLOCK_RE.
  detect_format: detect_format().
  parse_log: parse_log().
  build_name_to_stem_map: build_name_to_stem_map().
  INDEX_SECTION_RE: INDEX_SECTION_RE.
---
# Module: [`understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py)

## Functions
- `_collect_paragraph(start_lines: list[str])` — [`L121`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L121) — Collect the first paragraph from the given lines.
- `build_name_to_stem_map(wiki_root: Path)` — [`L223`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L223) — Build a case-insensitive map from filename stem to relative stem path.
- `detect_format(root: Path)` — [`L38`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L38) — Detect if directory follows the Karpathy LLM wiki three-layer pattern.
- `extract_code_blocks(text: str)` — [`L108`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L108) — Extract languages from fenced code blocks.
- `extract_first_paragraph(text: str)` — [`L113`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L113) — Extract the first non-empty paragraph after frontmatter and H1.
- `extract_frontmatter(text: str)` — [`L76`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L76) — Extract YAML frontmatter as a simple key-value dict.
- `extract_h1(text: str)` — [`L157`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L157) — Extract the first H1 heading.
- `extract_headings(text: str)` — [`L100`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L100) — Extract all markdown headings with level and text.
- `extract_wikilinks(text: str)` — [`L89`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L89) — Extract all [[target]] and [[target|display]] wikilinks.
- `main()` — [`L482`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L482)
- `parse_index(index_path: Path)` — [`L170`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L170) — Parse index.md to extract categories from ## headings and their wikilinks.
- `parse_log(log_path: Path)` — [`L201`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L201) — Parse log.md to extract chronological entries.
- `parse_wiki(root: Path)` — [`L278`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L278) — Parse a Karpathy-pattern wiki and produce the scan manifest.
- `resolve_wikilink(target: str, name_map: dict[str, str], node_ids: set[str] | None = None)` — [`L252`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L252) — Resolve a wikilink target to an article node ID.

## Module values
- `CODE_BLOCK_RE` — [`L27`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L27)
- `FRONTMATTER_RE` — [`L26`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L26)
- `HEADING_RE` — [`L28`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L28)
- `INDEX_SECTION_RE` — [`L29`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L29)
- `INFRA_FILES` — [`L32`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L32)
- `WIKILINK_RE` — [`L25`](../../../../../../../raw/code/understand-anything/understand-anything-plugin/skills/understand-knowledge/parse-knowledge-base.py#L25)

