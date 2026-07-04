---
title: 'Module: src/codegraphcontext/tools/languages/mybatis.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/mybatis.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.mybatis`/
symbols:
  parse_mybatis_mapper: parse_mybatis_mapper().
  find_and_parse_mybatis_mappers: find_and_parse_mybatis_mappers().
  _ALL_OP_TAGS: _ALL_OP_TAGS.
  _class_name_to_table: _class_name_to_table().
  _READ_TAGS: _READ_TAGS.
  _WRITE_TAGS: _WRITE_TAGS.
  _camel_to_snake: _camel_to_snake().
  _extract_sql: _extract_sql().
  _parse_sql_tables: _parse_sql_tables().
---
# Module: [`src/codegraphcontext/tools/languages/mybatis.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py)

## Functions
- `_camel_to_snake(name: str)` — [`L33`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L33) — Convert CamelCase to snake_case (e.g. MailHistory → mail_history).
- `_class_name_to_table(class_name: str)` — [`L39`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L39) — Derive a table name heuristic from a mapper class name.
- `_extract_sql(element: ET.Element)` — [`L52`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L52) — Return the concatenated text content of an XML element (handles CDATA).
- `_parse_sql_tables(sql: str)` — [`L67`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L67) — Extract table names from a SQL string (best-effort, no full parser).
- `find_and_parse_mybatis_mappers(repo_path: Path)` — [`L149`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L149) — Walk *repo_path* for MyBatis mapper XML files and return all operation records.
- `parse_mybatis_mapper(file_path: Path)` — [`L86`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L86) — Parse a single MyBatis XML mapper file and return operation records.

## Module values
- `_ALL_OP_TAGS` — [`L30`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L30)
- `_READ_TAGS` — [`L29`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L29)
- `_WRITE_TAGS` — [`L28`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/mybatis.py#L28)

