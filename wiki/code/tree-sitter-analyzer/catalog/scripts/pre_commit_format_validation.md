---
title: 'Module: scripts/pre_commit_format_validation.py'
type: catalog
provenance: extracted
module: scripts/pre_commit_format_validation.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `scripts.pre_commit_format_validation`/
symbols:
  PreCommitFormatValidator._validate_format_output: PreCommitFormatValidator#_validate_format_output().
  PreCommitFormatValidator.validate_file: PreCommitFormatValidator#validate_file().
  project_root: project_root.
  PreCommitFormatValidator.errors: PreCommitFormatValidator#errors.
  PreCommitFormatValidator.get_validation_summary: PreCommitFormatValidator#get_validation_summary().
  main: main().
  PreCommitFormatValidator.validated_files: PreCommitFormatValidator#validated_files.
  PreCommitFormatValidator.warnings: PreCommitFormatValidator#warnings.
  PreCommitFormatValidator: PreCommitFormatValidator#
  PreCommitFormatValidator._is_source_file: PreCommitFormatValidator#_is_source_file().
  PreCommitFormatValidator._detect_language: PreCommitFormatValidator#_detect_language().
  PreCommitFormatValidator._extract_class_name: PreCommitFormatValidator#_extract_class_name().
  PreCommitFormatValidator.__init__: PreCommitFormatValidator#__init__().
---
# Module: [`scripts/pre_commit_format_validation.py`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py)

## Classes
### `PreCommitFormatValidator`
- def: [`scripts/pre_commit_format_validation.py:31`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L31)
- doc: Pre-commit format validator
- signature: `class PreCommitFormatValidator:`
- members:
  - `_detect_language(self, file_path: Path)` — [`L98`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L98) — Detect programming language from file extension
  - `_extract_class_name(self, output: str, file_path: str)` — [`L164`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L164) — Extract class name from output or file path
  - `_is_source_file(self, file_path: Path)` — [`L93`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L93) — Check if file is a source file that should be validated
  - `_validate_format_output(self, output: str, format_type: str, file_path: str)` — [`L111`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L111) — Validate format output compliance
  - `get_validation_summary(self)` — [`L178`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L178) — Get validation summary
  - `validate_file(self, file_path: str)` — [`L39`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L39) — Validate format output for a single file
  - `errors` — [`L35`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L35)
  - `validated_files` — [`L37`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L37)
  - `warnings` — [`L36`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L36)
- protocol/private: `__init__`[`L34`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L34)
- uses (calls/refs, reference-scoped): [`AnalyzeCodeStructureTool`](../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool), [`execute`](../tree_sitter_analyzer/mcp/tools/analyze_code_structure_tool.md#AnalyzeCodeStructureTool.execute)  (6 test-only)
- used by: [`main`](pre_commit_format_validation.md#main)

## Functions
- `main()` — [`L191`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L191) — Main pre-commit validation function

## Module values
- `project_root` — [`L17`](../../../../../raw/code/tree-sitter-analyzer/scripts/pre_commit_format_validation.py#L17)

