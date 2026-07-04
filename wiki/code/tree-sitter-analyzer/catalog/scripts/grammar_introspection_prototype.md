---
title: 'Module: scripts/grammar_introspection_prototype.py'
type: catalog
provenance: extracted
module: scripts/grammar_introspection_prototype.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.grammar_introspection_prototype`/
symbols:
  main: main().
  analyze_parent_child_relationships.traverse: analyze_parent_child_relationships().traverse().
  enumerate_syntactic_paths_sample.traverse: enumerate_syntactic_paths_sample().traverse().
  analyze_parent_child_relationships: analyze_parent_child_relationships().
  enumerate_syntactic_paths_sample: enumerate_syntactic_paths_sample().
  get_all_node_types: get_all_node_types().
  get_all_field_names: get_all_field_names().
  infer_wrapper_patterns_heuristic: infer_wrapper_patterns_heuristic().
---
# Module: [`scripts/grammar_introspection_prototype.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py)

## Functions
- `analyze_parent_child_relationships(lang: tree_sitter.Language, sample_code: str)` — [`L89`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L89) — 通过解析示例代码分析父子关系
- `enumerate_syntactic_paths_sample(lang: tree_sitter.Language, sample_code: str, max_depth: int = 3)` — [`L113`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L113) — 通过解析示例代码枚举语法路径
- `get_all_field_names(lang: tree_sitter.Language)` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L39) — 枚举所有字段名称
- `get_all_node_types(lang: tree_sitter.Language)` — [`L17`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L17) — 枚举 language 中的所有 node types
- `infer_wrapper_patterns_heuristic(node_types: dict[str, dict[str, Any]])` — [`L57`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L57) — 启发式推断 wrapper nodes
- `main()` — [`L142`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L142) — 运行原型验证
- `traverse(node: tree_sitter.Node)` — [`L103`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L103)
- `traverse(node: tree_sitter.Node, parent_path: tuple[str, ...])` — [`L127`](../../../../../raw/code/tree-sitter-analyzer/scripts/grammar_introspection_prototype.py#L127)

