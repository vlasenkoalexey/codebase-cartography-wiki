---
title: 'Module: tree_sitter_analyzer/plugins/__init__.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/plugins/__init__.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.plugins`/
symbols:
  DefaultExtractor._traverse_for_functions: DefaultExtractor#_traverse_for_functions().
  DefaultExtractor._traverse_for_classes: DefaultExtractor#_traverse_for_classes().
  DefaultExtractor._traverse_for_variables: DefaultExtractor#_traverse_for_variables().
  DefaultExtractor._traverse_for_imports: DefaultExtractor#_traverse_for_imports().
  ElementExtractor.extract_functions: ElementExtractor#extract_functions().
  ElementExtractor.extract_classes: ElementExtractor#extract_classes().
  ElementExtractor.extract_variables: ElementExtractor#extract_variables().
  ElementExtractor.extract_imports: ElementExtractor#extract_imports().
  DefaultExtractor.extract_functions: DefaultExtractor#extract_functions().
  DefaultExtractor.extract_classes: DefaultExtractor#extract_classes().
  DefaultExtractor.extract_variables: DefaultExtractor#extract_variables().
  DefaultExtractor.extract_imports: DefaultExtractor#extract_imports().
  DefaultExtractor: DefaultExtractor#
  LanguagePlugin.create_extractor: LanguagePlugin#create_extractor().
  _safe_node_line_range: _safe_node_line_range().
  DefaultExtractor._extract_node_name: DefaultExtractor#_extract_node_name().
  LanguagePlugin.is_applicable: LanguagePlugin#is_applicable().
  ElementExtractor: ElementExtractor#
  LanguagePlugin.get_file_extensions: LanguagePlugin#get_file_extensions().
  __all__: __all__.
  LanguagePlugin: LanguagePlugin#
  LanguagePlugin.get_language_name: LanguagePlugin#get_language_name().
---
# Module: [`tree_sitter_analyzer/plugins/__init__.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py)

## Classes
### `DefaultExtractor`
- def: [`tree_sitter_analyzer/plugins/__init__.py:107`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L107)
- members:
  - `_extract_node_name(self, node: tree_sitter.Node)` — [`L264`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L264) — Extract name from a tree-sitter node.
  - `_traverse_for_classes(self, node: tree_sitter.Node, classes: list[ModelClass], lines: list[str])` — [`L196`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L196) — Traverse tree to find class-like nodes.
  - `_traverse_for_functions(self, node: tree_sitter.Node, functions: list[ModelFunction], lines: list[str])` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L170) — Traverse tree to find function-like nodes.
  - `_traverse_for_imports(self, node: tree_sitter.Node, imports: list[ModelImport], lines: list[str])` — [`L242`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L242) — Traverse tree to find import statements
  - `_traverse_for_variables(self, node: tree_sitter.Node, variables: list[ModelVariable], lines: list[str])` — [`L218`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L218) — Traverse tree to find variable declarations
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L125) — Basic class extraction implementation
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L110) — Basic function extraction implementation
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L155) — Basic import extraction implementation
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L140) — Basic variable extraction implementation
- uses (calls/refs, reference-scoped): [`name`](../models/base.md#CodeElement.name), [`start_line`](../models/base.md#CodeElement.start_line), [`end_line`](../models/base.md#CodeElement.end_line), [`log_debug`](../utils/logging.md#log_debug), [`language`](../models/base.md#CodeElement.language), [`Function`](../models/base.md#Function), [`raw_text`](../models/base.md#CodeElement.raw_text), [`log_error`](../utils/logging.md#log_error), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`_safe_node_line_range`](__init__.md#_safe_node_line_range), [`ElementExtractor`](__init__.md#ElementExtractor)
- used by: [`extract_classes`](__init__.md#ElementExtractor.extract_classes), [`extract_functions`](__init__.md#ElementExtractor.extract_functions), [`extract_imports`](__init__.md#ElementExtractor.extract_imports), [`extract_variables`](__init__.md#ElementExtractor.extract_variables), [`create_extractor`](__init__.md#LanguagePlugin.create_extractor)  (1 test-only)

### `ElementExtractor`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/plugins/__init__.py:47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L47)
- doc: Abstract base class for language-specific element extractors
- signature: `class ElementExtractor(ABC):`
- members:
  - `extract_classes(self, tree: tree_sitter.Tree, source_code: str)` — [`L59`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L59) — Extract class definitions from the syntax tree
  - `extract_functions(self, tree: tree_sitter.Tree, source_code: str)` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L51) — Extract function definitions from the syntax tree
  - `extract_imports(self, tree: tree_sitter.Tree, source_code: str)` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L75) — Extract import statements from the syntax tree
  - `extract_variables(self, tree: tree_sitter.Tree, source_code: str)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L67) — Extract variable declarations from the syntax tree
- uses (calls/refs, reference-scoped): [`Function`](../models/base.md#Function), [`Class`](../models/base.md#Class), [`Variable`](../models/base.md#Variable), [`Import`](../models/base.md#Import), [`log_warning`](../utils/logging.md#log_warning), [`extract_classes`](__init__.md#DefaultExtractor.extract_classes), [`extract_functions`](__init__.md#DefaultExtractor.extract_functions), [`extract_imports`](__init__.md#DefaultExtractor.extract_imports), [`extract_variables`](__init__.md#DefaultExtractor.extract_variables)
- used by: [`DefaultExtractor`](__init__.md#DefaultExtractor), [`create_extractor`](__init__.md#LanguagePlugin.create_extractor)

### `LanguagePlugin`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/plugins/__init__.py:83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L83)
- doc: Abstract base class for language-specific plugins
- signature: `class LanguagePlugin(ABC):`
- members:
  - `create_extractor(self)` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L97) — Create and return an element extractor for this language
  - `get_file_extensions(self)` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L92) — Return list of file extensions this plugin supports
  - `get_language_name(self)` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L87) — Return the name of the programming language this plugin supports
  - `is_applicable(self, file_path: str)` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L101) — Check if this plugin is applicable for the given file
- uses (calls/refs, reference-scoped): [`DefaultExtractor`](__init__.md#DefaultExtractor), [`ElementExtractor`](__init__.md#ElementExtractor)

## Functions
- `_safe_node_line_range(node: tree_sitter.Node)` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L31) — Return ``(start_line, end_line)`` from a tree-sitter node.

## Module values
- `__all__` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/plugins/__init__.py#L24)

