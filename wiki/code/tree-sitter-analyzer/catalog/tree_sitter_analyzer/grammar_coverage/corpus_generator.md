---
title: 'Module: tree_sitter_analyzer/grammar_coverage/corpus_generator.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/grammar_coverage/corpus_generator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.grammar_coverage.corpus_generator`/
symbols:
  generate_corpus_by_category: generate_corpus_by_category().
  generate_minimal_code_for_node_type: generate_minimal_code_for_node_type().
  validate_generated_code: validate_generated_code().
  generate_and_save_corpus: generate_and_save_corpus().
  save_corpus_files: save_corpus_files().
  CODE_TEMPLATES.CODE_TEMPLATES: CODE_TEMPLATES.CODE_TEMPLATES.
  validate_generated_code.has_error_node: validate_generated_code().has_error_node().
  LANGUAGE_EXTENSIONS: LANGUAGE_EXTENSIONS.
  LANGUAGE_MODULE_MAP: LANGUAGE_MODULE_MAP.
  NODE_TYPE_CATEGORIES: NODE_TYPE_CATEGORIES.
  PYTHON_TEMPLATES: PYTHON_TEMPLATES.
  JAVASCRIPT_TEMPLATES: JAVASCRIPT_TEMPLATES.
  JAVA_TEMPLATES: JAVA_TEMPLATES.
  _get_comment_prefix: _get_comment_prefix().
---
# Module: [`tree_sitter_analyzer/grammar_coverage/corpus_generator.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py)

## Functions
- `_get_comment_prefix(language: str)` — [`L341`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L341) — 获取语言的注释前缀。
- `generate_and_save_corpus(language: str, base_dir: str = "corpus/", validate: bool = True)` — [`L489`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L489) — 生成并保存完整的语料库（便捷函数）。
- `generate_corpus_by_category(language: str)` — [`L285`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L285) — 生成按分类组织的完整语料库。
- `generate_minimal_code_for_node_type(language: str, node_type: str)` — [`L255`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L255) — 生成指定节点类型的最小化代码示例。
- `has_error_node(node: tree_sitter.Node)` — [`L424`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L424)
- `save_corpus_files(language: str, corpus: dict[str, str], base_dir: str = "corpus/")` — [`L444`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L444) — 将语料库文件保存到磁盘。
- `validate_generated_code(language: str, code: str)` — [`L373`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L373) — 验证生成的代码是否可被 tree-sitter 成功解析。

## Module values
- `CODE_TEMPLATES` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L159)
- `JAVASCRIPT_TEMPLATES` — [`L109`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L109)
- `JAVA_TEMPLATES` — [`L134`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L134)
- `LANGUAGE_EXTENSIONS` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L38)
- `LANGUAGE_MODULE_MAP` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L59)
- `NODE_TYPE_CATEGORIES` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L166)
- `PYTHON_TEMPLATES` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/grammar_coverage/corpus_generator.py#L80)

