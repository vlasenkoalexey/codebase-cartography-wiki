---
title: 'Module: tests/fixtures/data_generators.py'
type: catalog
provenance: extracted
module: tests/fixtures/data_generators.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.fixtures.data_generators`/
symbols:
  generate_large_file_content: generate_large_file_content().
  generate_python_class: generate_python_class().
  generate_python_function: generate_python_function().
  generate_javascript_function: generate_javascript_function().
  generate_typescript_interface: generate_typescript_interface().
  generate_java_class: generate_java_class().
  generate_html_page: generate_html_page().
  generate_css_rules: generate_css_rules().
  generate_random_identifier: generate_random_identifier().
  __all__: __all__.
---
# Module: [`tests/fixtures/data_generators.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py)

## Functions
- `generate_css_rules(selectors: dict[str, dict[str, str]])` — [`L328`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L328) — Generate CSS rules.
- `generate_html_page(title: str = "Test Page", body_content: str = "<p>Hello, World!</p>", head_elements: list[str] | None = None)` — [`L286`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L286) — Generate HTML page code.
- `generate_java_class(name: str = "TestClass", package: str | None = None, modifiers: list[str] | None = None, extends: str | None = None, implements: list[str] | None = None, fields: list[dict[str, str]] | None = None, methods: list[dict[str, Any]] | None = None)` — [`L204`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L204) — Generate Java class code.
- `generate_javascript_function(name: str = "testFunction", params: list[str] | None = None, body: str = "return null;", is_async: bool = False, is_arrow: bool = False)` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L135) — Generate JavaScript function code.
- `generate_large_file_content(language: str = "python", num_functions: int = 100, num_classes: int = 20)` — [`L376`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L376) — Generate large file content for performance testing.
- `generate_python_class(name: str = "TestClass", bases: list[str] | None = None, methods: list[dict[str, Any]] | None = None, attributes: list[str] | None = None, docstring: str | None = None)` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L67) — Generate Python class code.
- `generate_python_function(name: str = "test_function", params: list[str] | None = None, body: str = "pass", decorators: list[str] | None = None, docstring: str | None = None)` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L16) — Generate Python function code.
- `generate_random_identifier(length: int = 8, prefix: str = "test_")` — [`L358`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L358) — Generate a random identifier.
- `generate_typescript_interface(name: str = "TestInterface", properties: dict[str, str] | None = None, methods: dict[str, str] | None = None)` — [`L170`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L170) — Generate TypeScript interface code.

## Module values
- `__all__` — [`L431`](../../../../../../raw/code/tree-sitter-analyzer/tests/fixtures/data_generators.py#L431)

