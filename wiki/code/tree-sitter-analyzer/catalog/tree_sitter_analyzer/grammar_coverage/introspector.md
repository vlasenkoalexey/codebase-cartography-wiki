---
title: 'Module: tree_sitter_analyzer/grammar_coverage/introspector.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/grammar_coverage/introspector.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.grammar_coverage.introspector`/
symbols:
  get_all_node_types: get_all_node_types().
  auto_detect_extractable_types: auto_detect_extractable_types().
  get_structural_types: get_structural_types().
  get_language_summary: get_language_summary().
  LANGUAGE_MODULE_MAP: LANGUAGE_MODULE_MAP.
  _validate_language: _validate_language().
  _import_ts_module: _import_ts_module().
  _get_language_capsule: _get_language_capsule().
  EXTRACTABLE_SUFFIXES: EXTRACTABLE_SUFFIXES.
  STRUCTURAL_PATTERNS: STRUCTURAL_PATTERNS.
  EXTRACTABLE_EXACT_NAMES: EXTRACTABLE_EXACT_NAMES.
  _collect_named_node_types: _collect_named_node_types().
---
# Module: [`tree_sitter_analyzer/grammar_coverage/introspector.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py)

## Functions
- `_collect_named_node_types(lang_obj: object)` — [`L113`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L113) — Walk ``lang_obj.node_kind_count`` and return sorted named node types.
- `_get_language_capsule(ts_module: object, language: str, module_name: str)` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L90) — Probe the module for a known language-getter function and return its capsule.
- `_import_ts_module(module_name: str)` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L76) — Dynamically import the tree-sitter language module; raise ImportError if missing.
- `_validate_language(language: str)` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L68) — Validate ``language`` against ``LANGUAGE_MODULE_MAP``; return module name.
- `auto_detect_extractable_types(node_types: list[str])` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L159) — 基于命名模式自动检测可提取节点类型。
- `get_all_node_types(language: str)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L125) — 获取指定语言的所有命名节点类型。
- `get_language_summary(language: str)` — [`L234`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L234) — 获取指定语言的语法节点类型摘要。
- `get_structural_types(node_types: list[str])` — [`L202`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L202) — 识别结构性节点类型（非可提取）。

## Module values
- `EXTRACTABLE_EXACT_NAMES` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L47)
- `EXTRACTABLE_SUFFIXES` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L39)
- `LANGUAGE_MODULE_MAP` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L17)
- `STRUCTURAL_PATTERNS` — [`L55`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/introspector.py#L55)

