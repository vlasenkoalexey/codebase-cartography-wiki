---
title: 'Module: tree_sitter_analyzer/ast_path.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/ast_path.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.ast_path`/
symbols:
  ASTPathNavigator.path_at_line: ASTPathNavigator#path_at_line().
  _build_ast_node: _build_ast_node().
  ASTNode.name: ASTNode#name.
  ASTPathNavigator._parse: ASTPathNavigator#_parse().
  ASTPathNavigator.outline: ASTPathNavigator#outline().
  ASTPathResult.to_dict: ASTPathResult#to_dict().
  ASTPathNavigator: ASTPathNavigator#
  ASTNode.to_dict: ASTNode#to_dict().
  _find_and_collect_siblings: _find_and_collect_siblings().
  ASTPathNavigator.scope_at: ASTPathNavigator#scope_at().
  ASTPathResult.path: ASTPathResult#path.
  ASTNode: ASTNode#
  ASTPathResult.enclosing_scope: ASTPathResult#enclosing_scope.
  ASTPathNavigator._collect: ASTPathNavigator#_collect().
  ASTPathNavigator._get_siblings: ASTPathNavigator#_get_siblings().
  ASTPathResult.target_line: ASTPathResult#target_line.
  ASTPathNavigator._walk: ASTPathNavigator#_walk().
  ASTPathResult.node_at_line: ASTPathResult#node_at_line.
  ASTPathResult.siblings: ASTPathResult#siblings.
  _is_named_scope: _is_named_scope().
  ASTNode.start_line: ASTNode#start_line.
  ASTNode.end_line: ASTNode#end_line.
  ASTPathResult: ASTPathResult#
  ASTPathResult.language: ASTPathResult#language.
  ASTPathNavigator._parser: ASTPathNavigator#_parser.
  ASTPathNavigator._detector: ASTPathNavigator#_detector.
  ASTNode.is_named_scope: ASTNode#is_named_scope.
  ASTNode.field_name: ASTNode#field_name.
  ASTPathResult.file_path: ASTPathResult#file_path.
  logger: logger.
  ASTNode.children_count: ASTNode#children_count.
  _node_name: _node_name().
  _NAMED_SCOPE_TYPES._NAMED_SCOPE_TYPES: _NAMED_SCOPE_TYPES._NAMED_SCOPE_TYPES.
  ASTPathNavigator.__init__: ASTPathNavigator#__init__().
---
# Module: [`tree_sitter_analyzer/ast_path.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py)

## Classes
### `ASTNode`
- def: [`tree_sitter_analyzer/ast_path.py:93`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L93)
- doc: A single node in the AST path.
- signature: `class ASTNode:`
- members:
  - `to_dict(self)` — [`L104`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L104)
  - `children_count` — [`L101`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L101)
  - `end_line` — [`L99`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L99)
  - `field_name` — [`L102`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L102)
  - `is_named_scope` — [`L100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L100)
  - `name` — [`L97`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L97)
  - `start_line` — [`L98`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L98)
- used by: [`path_at_line`](ast_path.md#ASTPathNavigator.path_at_line), [`_build_ast_node`](ast_path.md#_build_ast_node), [`outline`](ast_path.md#ASTPathNavigator.outline), [`to_dict`](ast_path.md#ASTPathResult.to_dict), [`_find_and_collect_siblings`](ast_path.md#_find_and_collect_siblings), [`path`](ast_path.md#ASTPathResult.path), [`enclosing_scope`](ast_path.md#ASTPathResult.enclosing_scope), [`_collect`](ast_path.md#ASTPathNavigator._collect), [`_get_siblings`](ast_path.md#ASTPathNavigator._get_siblings), [`node_at_line`](ast_path.md#ASTPathResult.node_at_line), [`siblings`](ast_path.md#ASTPathResult.siblings)  (12 test-only)

### `ASTPathNavigator`
- def: [`tree_sitter_analyzer/ast_path.py:239`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L239)
- doc: Navigate the AST of a source file to answer scope/path queries.
- signature: `class ASTPathNavigator:`
- members:
  - `_get_siblings(self, file_path: str, scope_node: ASTNode, language: str, source: str | None = None)` — [`L391`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L391) — Get sibling declarations at the same scope level.
  - `_parse(self, file_path: str, language: str | None = None)` — [`L254`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L254) — Parse file and return (tree, source, language).
  - `outline(self, file_path: str, language: str | None = None, max_depth: int = 3)` — [`L353`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L353) — Return the hierarchical outline of a file (top-level declarations).
  - `path_at_line(self, file_path: str, line: int, language: str | None = None)` — [`L271`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L271) — Find the full AST path from root to the node at the given line.
  - `scope_at(self, file_path: str, line: int, language: str | None = None)` — [`L335`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L335) — Find the innermost named scope enclosing the given line.
- protocol/private: `__init__`[`L250`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L250), `_collect`[`L368`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L368), `_detector`[`L252`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L252), `_parser`[`L251`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L251), `_walk`[`L288`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L288)
- uses (calls/refs, reference-scoped): [`Parser`](core/parser.md#Parser), [`tree`](core/parser.md#ParseResult.tree), [`success`](core/parser.md#ParseResult.success), [`parse_file`](core/parser.md#Parser.parse_file), [`detect_language`](language_detector.md#LanguageDetector.detect_language), [`LanguageDetector`](language_detector.md#LanguageDetector), [`error_message`](core/parser.md#ParseResult.error_message), [`source_code`](core/parser.md#ParseResult.source_code), [`_build_ast_node`](ast_path.md#_build_ast_node), [`name`](ast_path.md#ASTNode.name), [`_find_and_collect_siblings`](ast_path.md#_find_and_collect_siblings), [`path`](ast_path.md#ASTPathResult.path), [`ASTNode`](ast_path.md#ASTNode), [`enclosing_scope`](ast_path.md#ASTPathResult.enclosing_scope), [`target_line`](ast_path.md#ASTPathResult.target_line), [`_is_named_scope`](ast_path.md#_is_named_scope), [`node_at_line`](ast_path.md#ASTPathResult.node_at_line), [`siblings`](ast_path.md#ASTPathResult.siblings), [`ASTPathResult`](ast_path.md#ASTPathResult), [`language`](ast_path.md#ASTPathResult.language), [`file_path`](ast_path.md#ASTPathResult.file_path), [`is_named_scope`](ast_path.md#ASTNode.is_named_scope)
- used by: [`execute`](mcp/tools/ast_path_tool.md#CodeGraphASTPathTool.execute), [`_get_navigator`](mcp/tools/ast_path_tool.md#CodeGraphASTPathTool._get_navigator), [`__init__`](mcp/tools/ast_path_tool.md#CodeGraphASTPathTool.__init__)  (17 test-only)

### `ASTPathResult`
- def: [`tree_sitter_analyzer/ast_path.py:119`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L119)
- doc: Full result of an AST path query.
- signature: `class ASTPathResult:`
- members:
  - `to_dict(self)` — [`L130`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L130)
  - `enclosing_scope` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L127)
  - `file_path` — [`L122`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L122)
  - `language` — [`L123`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L123)
  - `node_at_line` — [`L126`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L126)
  - `path` — [`L125`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L125)
  - `siblings` — [`L128`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L128)
  - `target_line` — [`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L124)
- uses (calls/refs, reference-scoped): [`to_dict`](ast_path.md#ASTNode.to_dict), [`ASTNode`](ast_path.md#ASTNode)
- used by: [`path_at_line`](ast_path.md#ASTPathNavigator.path_at_line), [`outline`](ast_path.md#ASTPathNavigator.outline), [`execute`](mcp/tools/ast_path_tool.md#CodeGraphASTPathTool.execute), [`scope_at`](ast_path.md#ASTPathNavigator.scope_at)  (16 test-only)

## Functions
- `_build_ast_node(node: Any, source: str, language: str, field_name: str | None = None)` — [`L224`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L224) — Build an ASTNode from a tree-sitter node.
- `_find_and_collect_siblings(node: Any, scope_node: ASTNode, language: str, source: str, siblings: list[ASTNode])` — [`L187`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L187) — Collect sibling scope nodes at the same AST level as scope_node.
- `_is_named_scope(node_type: str, language: str)` — [`L182`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L182) — Check if a node type represents a named scope.
- `_node_name(node: Any, source: str, language: str)` — [`L147`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L147) — Extract a human-readable name from an AST node.

## Module values
- `_NAMED_SCOPE_TYPES` — [`L30`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L30)
- `logger` — [`L28`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/ast_path.py#L28)

