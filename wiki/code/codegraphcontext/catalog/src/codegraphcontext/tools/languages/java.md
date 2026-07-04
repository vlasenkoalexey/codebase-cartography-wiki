---
title: 'Module: src/codegraphcontext/tools/languages/java.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/tools/languages/java.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.tools.languages.java`/
symbols:
  JavaTreeSitterParser.index_source: JavaTreeSitterParser#index_source.
  JavaTreeSitterParser._walk: JavaTreeSitterParser#_walk().
  JavaTreeSitterParser._parse_functions: JavaTreeSitterParser#_parse_functions().
  JavaTreeSitterParser._get_node_text: JavaTreeSitterParser#_get_node_text().
  JavaTreeSitterParser._parse_classes: JavaTreeSitterParser#_parse_classes().
  JavaTreeSitterParser._parse_calls: JavaTreeSitterParser#_parse_calls().
  JavaTreeSitterParser._extract_orm_mappings: JavaTreeSitterParser#_extract_orm_mappings().
  JavaTreeSitterParser._get_node_annotations: JavaTreeSitterParser#_get_node_annotations().
  JavaTreeSitterParser._parse_variables: JavaTreeSitterParser#_parse_variables().
  JavaTreeSitterParser._parse_imports: JavaTreeSitterParser#_parse_imports().
  JavaTreeSitterParser._extract_parameter_types: JavaTreeSitterParser#_extract_parameter_types().
  JavaTreeSitterParser.language_name: JavaTreeSitterParser#language_name.
  JavaTreeSitterParser._extract_parameter_names: JavaTreeSitterParser#_extract_parameter_names().
  JavaTreeSitterParser._get_parent_context: JavaTreeSitterParser#_get_parent_context().
  _sql_operation: _sql_operation().
  JavaTreeSitterParser._strip_parameter_annotations_and_modifiers: JavaTreeSitterParser#_strip_parameter_annotations_and_modifiers().
  JavaTreeSitterParser._get_annotation_details: JavaTreeSitterParser#_get_annotation_details().
  JavaTreeSitterParser._extract_spring_injections: JavaTreeSitterParser#_extract_spring_injections().
  pre_scan_java: pre_scan_java().
  JavaTreeSitterParser._strip_generic: JavaTreeSitterParser#_strip_generic().
  _parse_sql_tables: _parse_sql_tables().
  _extract_annotation_path: _extract_annotation_path().
  JavaTreeSitterParser: JavaTreeSitterParser#
  JavaTreeSitterParser._class_at_line: JavaTreeSitterParser#_class_at_line().
  JavaTreeSitterParser._split_parameters: JavaTreeSitterParser#_split_parameters().
  _SPRING_CLASS_STEREOTYPES._SPRING_CLASS_STEREOTYPES: _SPRING_CLASS_STEREOTYPES._SPRING_CLASS_STEREOTYPES.
  _SPRING_HTTP_MAPPINGS._SPRING_HTTP_MAPPINGS: _SPRING_HTTP_MAPPINGS._SPRING_HTTP_MAPPINGS.
  _SPRING_INJECT_ANNOTATIONS: _SPRING_INJECT_ANNOTATIONS.
  _SQL_QUERY_ANNOTATIONS: _SQL_QUERY_ANNOTATIONS.
  _WRITE_PREFIXES: _WRITE_PREFIXES.
  _SPRING_DATA_REPO_BASES: _SPRING_DATA_REPO_BASES.
  _SPRING_DATA_READS_PREFIXES: _SPRING_DATA_READS_PREFIXES.
  _SPRING_DATA_WRITES_PREFIXES: _SPRING_DATA_WRITES_PREFIXES.
  JAVA_QUERIES: JAVA_QUERIES.
  JavaTreeSitterParser.language: JavaTreeSitterParser#language.
  JavaTreeSitterParser.parser: JavaTreeSitterParser#parser.
  JavaTreeSitterParser._matching_paren_index: JavaTreeSitterParser#_matching_paren_index().
  _JPA_TABLE_ANNOTATIONS: _JPA_TABLE_ANNOTATIONS.
  _CASSANDRA_TABLE_ANNOTATIONS: _CASSANDRA_TABLE_ANNOTATIONS.
  _REDIS_HASH_ANNOTATIONS: _REDIS_HASH_ANNOTATIONS.
  JavaTreeSitterParser.__init__: JavaTreeSitterParser#__init__().
  JavaTreeSitterParser.generic_parser_wrapper: JavaTreeSitterParser#generic_parser_wrapper.
  JavaTreeSitterParser.parse: JavaTreeSitterParser#parse().
---
# Module: [`src/codegraphcontext/tools/languages/java.py`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py)

## Classes
### `JavaTreeSitterParser`
- def: [`src/codegraphcontext/tools/languages/java.py:164`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L164)
- signature: `class JavaTreeSitterParser:`
- members:
  - `_extract_orm_mappings(self, tree: Any, path: Path, parsed_classes: List[Dict[str, Any]], parsed_functions: List[Dict[str, Any]])` — [`L578`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L578) — Walk the tree and emit ORM mapping records for #843.
  - `_extract_spring_injections(self, tree: Any, path: Path, parsed_classes: List[Dict[str, Any]])` — [`L800`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L800) — Walk field_declaration nodes and emit injection records for @Autowired/@Inject fields.
  - `_get_annotation_details(self, ann_node: Any)` — [`L299`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L299) — Return (annotation_name, annotation_args_text) for an annotation/marker_annotation node.
  - `_get_node_annotations(self, node: Any)` — [`L307`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L307) — Return list of (name, args_text) for all annotations on a node's modifiers.
  - `_strip_generic(type_str: str)` — [`L172`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L172) — Return the raw type name without generic parameters, e.g. 'List<String>' -> 'List'.
  - `parse(self, path: Path, is_dependency: bool = False, index_source: bool = False)` — [`L177`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L177)
  - `generic_parser_wrapper` — [`L166`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L166)
  - `index_source` — [`L179`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L179) — documented in [codegraphcontext-utils-tree_sitter_manager](../../../../../concepts/codegraphcontext-utils-tree_sitter_manager.md)
  - `language` — [`L168`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L168)
  - `language_name` — [`L167`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L167)
  - `parser` — [`L169`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L169)
- protocol/private: `__init__`[`L165`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L165), `_class_at_line`[`L607`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L607), `_extract_parameter_names`[`L966`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L966), `_extract_parameter_types`[`L1089`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L1089), `_get_node_text`[`L293`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L293), `_get_parent_context`[`L273`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L273), `_matching_paren_index`[`L1040`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L1040), `_parse_calls`[`L884`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L884), `_parse_classes`[`L404`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L404), `_parse_functions`[`L325`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L325), `_parse_imports`[`L857`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L857), `_parse_variables`[`L525`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L525), `_split_parameters`[`L985`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L985), `_strip_parameter_annotations_and_modifiers`[`L1065`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L1065), `_walk`[`L615`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L615)
- uses (calls/refs, reference-scoped): [`warning_logger`](../../utils/debug_log.md#warning_logger), [`execute_query`](../../utils/tree_sitter_manager.md#execute_query), [`debug_log`](../../utils/debug_log.md#debug_log), [`error_logger`](../../utils/debug_log.md#error_logger), [`_sql_operation`](java.md#_sql_operation), [`_SPRING_CLASS_STEREOTYPES`](java.md#_SPRING_CLASS_STEREOTYPES._SPRING_CLASS_STEREOTYPES), [`_SPRING_HTTP_MAPPINGS`](java.md#_SPRING_HTTP_MAPPINGS._SPRING_HTTP_MAPPINGS), [`_extract_annotation_path`](java.md#_extract_annotation_path), [`_parse_sql_tables`](java.md#_parse_sql_tables), [`JAVA_QUERIES`](java.md#JAVA_QUERIES), [`_SPRING_DATA_READS_PREFIXES`](java.md#_SPRING_DATA_READS_PREFIXES), [`_SPRING_DATA_REPO_BASES`](java.md#_SPRING_DATA_REPO_BASES), [`_SPRING_DATA_WRITES_PREFIXES`](java.md#_SPRING_DATA_WRITES_PREFIXES), [`_SPRING_INJECT_ANNOTATIONS`](java.md#_SPRING_INJECT_ANNOTATIONS), [`_SQL_QUERY_ANNOTATIONS`](java.md#_SQL_QUERY_ANNOTATIONS)
- used by: [`language_specific_parser`](../tree_sitter_parser.md#TreeSitterParser.language_specific_parser)

## Functions
- `_extract_annotation_path(args_text: str)` — [`L104`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L104) — Extract the first string literal from annotation arguments, e.g. '("/api/users")' -> '/api/users'.
- `_parse_sql_tables(sql: str)` — [`L79`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L79) — Extract table names from a SQL/CQL string without a full parser.
- `_sql_operation(sql: str)` — [`L95`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L95) — Return 'READS' or 'WRITES' based on SQL DML prefix.
- `pre_scan_java(files: list[Path], parser_wrapper)` — [`L1114`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L1114)

## Module values
- `JAVA_QUERIES` — [`L109`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L109)
- `_CASSANDRA_TABLE_ANNOTATIONS` — [`L39`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L39)
- `_JPA_TABLE_ANNOTATIONS` — [`L36`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L36)
- `_REDIS_HASH_ANNOTATIONS` — [`L43`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L43)
- `_SPRING_CLASS_STEREOTYPES` — [`L9`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L9)
- `_SPRING_DATA_READS_PREFIXES` — [`L62`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L62)
- `_SPRING_DATA_REPO_BASES` — [`L53`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L53)
- `_SPRING_DATA_WRITES_PREFIXES` — [`L70`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L70)
- `_SPRING_HTTP_MAPPINGS` — [`L21`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L21)
- `_SPRING_INJECT_ANNOTATIONS` — [`L31`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L31)
- `_SQL_QUERY_ANNOTATIONS` — [`L46`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L46)
- `_WRITE_PREFIXES` — [`L50`](../../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/tools/languages/java.py#L50)

