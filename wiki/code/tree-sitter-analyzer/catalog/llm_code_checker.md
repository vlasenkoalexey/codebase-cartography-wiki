---
title: 'Module: llm_code_checker.py'
type: catalog
provenance: extracted
module: llm_code_checker.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 llm_code_checker/
symbols:
  LLMCodeChecker.check_file: LLMCodeChecker#check_file().
  LLMCodeChecker.print_summary: LLMCodeChecker#print_summary().
  main: main().
  Colors: Colors#
  LLMCodeChecker._add_issue: LLMCodeChecker#_add_issue().
  Colors.END: Colors#END.
  Colors.BOLD: Colors#BOLD.
  LLMCodeChecker._check_type_hints: LLMCodeChecker#_check_type_hints().
  LLMCodeChecker._check_docstrings: LLMCodeChecker#_check_docstrings().
  LLMCodeChecker._check_error_handling: LLMCodeChecker#_check_error_handling().
  LLMCodeChecker._check_imports: LLMCodeChecker#_check_imports().
  LLMCodeChecker._check_naming_conventions: LLMCodeChecker#_check_naming_conventions().
  LLMCodeChecker._check_anti_patterns: LLMCodeChecker#_check_anti_patterns().
  LLMCodeChecker._check_project_patterns: LLMCodeChecker#_check_project_patterns().
  LLMCodeChecker.issues: LLMCodeChecker#issues.
  LLMCodeChecker.total_issues: LLMCodeChecker#total_issues.
  Colors.RED: Colors#RED.
  Colors.GREEN: Colors#GREEN.
  LLMCodeChecker.files_checked: LLMCodeChecker#files_checked.
  Colors.YELLOW: Colors#YELLOW.
  Colors.BLUE: Colors#BLUE.
  Colors.MAGENTA: Colors#MAGENTA.
  Colors.CYAN: Colors#CYAN.
  LLMCodeChecker: LLMCodeChecker#
  Colors.WHITE: Colors#WHITE.
  Colors.UNDERLINE: Colors#UNDERLINE.
  LLMCodeChecker.__init__: LLMCodeChecker#__init__().
---
# Module: [`llm_code_checker.py`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py)

## Classes
### `Colors`
- def: [`llm_code_checker.py:22`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L22)
- signature: `class Colors:`
- members:
  - `BLUE` — [`L26`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L26)
  - `BOLD` — [`L30`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L30)
  - `CYAN` — [`L28`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L28)
  - `END` — [`L32`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L32)
  - `GREEN` — [`L24`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L24)
  - `MAGENTA` — [`L27`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L27)
  - `RED` — [`L23`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L23)
  - `UNDERLINE` — [`L31`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L31)
  - `WHITE` — [`L29`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L29)
  - `YELLOW` — [`L25`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L25)
- used by: [`check_file`](llm_code_checker.md#LLMCodeChecker.check_file), [`print_summary`](llm_code_checker.md#LLMCodeChecker.print_summary), [`main`](llm_code_checker.md#main)

### `LLMCodeChecker`
- def: [`llm_code_checker.py:35`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L35)
- doc: Specialized code quality checker for LLM-generated code.
- signature: `class LLMCodeChecker:`
- members:
  - `_add_issue(self, file_path: Path, issue_type: str, message: str, line: int | None = None)` — [`L86`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L86) — Add an issue to the list.
  - `_check_anti_patterns(self, file_path: Path, tree: ast.AST, content: str)` — [`L232`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L232) — Check for common anti-patterns.
  - `_check_docstrings(self, file_path: Path, tree: ast.AST)` — [`L127`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L127) — Check for missing docstrings.
  - `_check_error_handling(self, file_path: Path, tree: ast.AST)` — [`L154`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L154) — Check for proper error handling.
  - `_check_imports(self, file_path: Path, tree: ast.AST, content: str)` — [`L176`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L176) — Check import organization and usage.
  - `_check_naming_conventions(self, file_path: Path, tree: ast.AST)` — [`L207`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L207) — Check naming conventions.
  - `_check_project_patterns(self, file_path: Path, tree: ast.AST, content: str)` — [`L264`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L264) — Check for project-specific patterns.
  - `_check_type_hints(self, file_path: Path, tree: ast.AST, content: str)` — [`L100`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L100) — Check for missing type hints.
  - `check_file(self, file_path: Path)` — [`L43`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L43) — Check a single Python file for LLM-specific issues.
  - `print_summary(self)` — [`L297`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L297) — Print a summary of all issues found.
  - `files_checked` — [`L40`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L40)
  - `issues` — [`L39`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L39)
  - `total_issues` — [`L41`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L41)
- protocol/private: `__init__`[`L38`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L38)
- uses (calls/refs, reference-scoped): [`Colors`](llm_code_checker.md#Colors), [`END`](llm_code_checker.md#Colors.END), [`BOLD`](llm_code_checker.md#Colors.BOLD), [`GREEN`](llm_code_checker.md#Colors.GREEN), [`RED`](llm_code_checker.md#Colors.RED), [`BLUE`](llm_code_checker.md#Colors.BLUE), [`MAGENTA`](llm_code_checker.md#Colors.MAGENTA), [`YELLOW`](llm_code_checker.md#Colors.YELLOW)
- used by: [`main`](llm_code_checker.md#main)

## Functions
- `main()` — [`L334`](../../../../raw/code/tree-sitter-analyzer/llm_code_checker.py#L334) — Main entry point.

