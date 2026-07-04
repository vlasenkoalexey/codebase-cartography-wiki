---
title: 'Module: tree_sitter_analyzer/_exceptions_core.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/_exceptions_core.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer._exceptions_core`/
symbols:
  TreeSitterAnalyzerError.context: TreeSitterAnalyzerError#context.
  TreeSitterAnalyzerError: TreeSitterAnalyzerError#
  MCPError: MCPError#
  AnalysisError: AnalysisError#
  ValidationError: ValidationError#
  QueryError: QueryError#
  FileHandlingError: FileHandlingError#
  TreeSitterAnalyzerError.message: TreeSitterAnalyzerError#message.
  ParseError: ParseError#
  LanguageNotSupportedError: LanguageNotSupportedError#
  TreeSitterAnalyzerError.to_dict: TreeSitterAnalyzerError#to_dict().
  PluginError: PluginError#
  ConfigurationError: ConfigurationError#
  TreeSitterAnalyzerError.__init__: TreeSitterAnalyzerError#__init__().
  TreeSitterAnalyzerError.error_code: TreeSitterAnalyzerError#error_code.
  MCPError.__init__: MCPError#__init__().
  ValidationError.__init__: ValidationError#__init__().
  AnalysisError.__init__: AnalysisError#__init__().
  ParseError.__init__: ParseError#__init__().
  LanguageNotSupportedError.__init__: LanguageNotSupportedError#__init__().
  PluginError.__init__: PluginError#__init__().
  QueryError.__init__: QueryError#__init__().
  FileHandlingError.__init__: FileHandlingError#__init__().
  ConfigurationError.__init__: ConfigurationError#__init__().
---
# Module: [`tree_sitter_analyzer/_exceptions_core.py`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py)

## Classes
### `AnalysisError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:31`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L31) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when file analysis fails.
- signature: `class AnalysisError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L34`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L34)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError)  (26 test-only)

### `ConfigurationError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:139`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L139)
- doc: Raised when configuration is invalid.
- signature: `class ConfigurationError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L142`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L142)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError)  (6 test-only)

### `FileHandlingError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:121`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L121)
- doc: Raised when file operations fail.
- signature: `class FileHandlingError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L124`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L124)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError)  (12 test-only)

### `LanguageNotSupportedError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:67`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L67)
- doc: Raised when a language is not supported.
- signature: `class LanguageNotSupportedError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L70`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L70)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError)  (8 test-only)

### `MCPError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:175`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L175) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when MCP operations fail.
- signature: `class MCPError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L178`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L178)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`MCPToolError`](_exceptions_mcp_types.md#MCPToolError), [`MCPResourceError`](_exceptions_mcp_types.md#MCPResourceError), [`MCPTimeoutError`](_exceptions_mcp_types.md#MCPTimeoutError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`MCPToolError`](_exceptions_mcp_types.md#MCPToolError), [`MCPResourceError`](_exceptions_mcp_types.md#MCPResourceError), [`MCPTimeoutError`](_exceptions_mcp_types.md#MCPTimeoutError), [`__init__`](_exceptions_mcp_types.md#MCPToolError.__init__), [`__init__`](_exceptions_mcp_types.md#MCPResourceError.__init__), [`__init__`](_exceptions_mcp_types.md#MCPTimeoutError.__init__)  (16 test-only)

### `ParseError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:49`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L49)
- doc: Raised when parsing fails.
- signature: `class ParseError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L52`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L52)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError)  (9 test-only)

### `PluginError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:82`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L82)
- doc: Raised when plugin operations fail.
- signature: `class PluginError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L85`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L85)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError)  (6 test-only)

### `QueryError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:100`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L100) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when query execution fails.
- signature: `class QueryError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L103`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L103)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError)  (15 test-only)

### `TreeSitterAnalyzerError`  ·  implements/extends Exception
- def: [`tree_sitter_analyzer/_exceptions_core.py:7`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L7) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Base exception for all tree-sitter analyzer errors.
- signature: `class TreeSitterAnalyzerError(Exception):`
- members:
  - `to_dict(self)` — [`L21`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L21) — Convert exception to dictionary format.
  - `context` — [`L19`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L19)
  - `error_code` — [`L18`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L18)
  - `message` — [`L17`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L17)
- protocol/private: `__init__`[`L10`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L10)
- uses (calls/refs, reference-scoped): [`SecurityError`](_exceptions_security.md#SecurityError), [`MCPError`](_exceptions_core.md#MCPError), [`AnalysisError`](_exceptions_core.md#AnalysisError), [`ValidationError`](_exceptions_core.md#ValidationError), [`QueryError`](_exceptions_core.md#QueryError), [`FileHandlingError`](_exceptions_core.md#FileHandlingError), [`ParseError`](_exceptions_core.md#ParseError), [`LanguageNotSupportedError`](_exceptions_core.md#LanguageNotSupportedError), [`ConfigurationError`](_exceptions_core.md#ConfigurationError), [`PluginError`](_exceptions_core.md#PluginError)
- used by: [`SecurityError`](_exceptions_security.md#SecurityError), [`MCPError`](_exceptions_core.md#MCPError), [`AnalysisError`](_exceptions_core.md#AnalysisError), [`ValidationError`](_exceptions_core.md#ValidationError), [`QueryError`](_exceptions_core.md#QueryError), [`FileHandlingError`](_exceptions_core.md#FileHandlingError), [`handle_exception`](_exceptions_execution.md#handle_exception), [`ParseError`](_exceptions_core.md#ParseError), [`LanguageNotSupportedError`](_exceptions_core.md#LanguageNotSupportedError), [`ConfigurationError`](_exceptions_core.md#ConfigurationError), [`PluginError`](_exceptions_core.md#PluginError), [`__init__`](_exceptions_core.md#MCPError.__init__), [`__init__`](_exceptions_security.md#SecurityError.__init__), [`__init__`](_exceptions_core.md#ValidationError.__init__), [`__init__`](_exceptions_core.md#AnalysisError.__init__), [`__init__`](_exceptions_core.md#ConfigurationError.__init__), [`__init__`](_exceptions_core.md#FileHandlingError.__init__), [`__init__`](_exceptions_core.md#LanguageNotSupportedError.__init__), [`__init__`](_exceptions_core.md#ParseError.__init__), [`__init__`](_exceptions_core.md#PluginError.__init__), [`__init__`](_exceptions_core.md#QueryError.__init__)  (106 test-only)

### `ValidationError`  ·  implements/extends TreeSitterAnalyzerError
- def: [`tree_sitter_analyzer/_exceptions_core.py:157`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L157) — documented in [tree_sitter_analyzer-security-validator](../../concepts/tree_sitter_analyzer-security-validator.md)
- doc: Raised when validation fails.
- signature: `class ValidationError(TreeSitterAnalyzerError):`
- protocol/private: `__init__`[`L160`](../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/_exceptions_core.py#L160)
- uses (calls/refs, reference-scoped): [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`MCPValidationError`](_exceptions_mcp_types.md#MCPValidationError), [`__init__`](_exceptions_core.md#TreeSitterAnalyzerError.__init__)
- used by: [`TreeSitterAnalyzerError`](_exceptions_core.md#TreeSitterAnalyzerError), [`MCPValidationError`](_exceptions_mcp_types.md#MCPValidationError), [`__init__`](_exceptions_mcp_types.md#MCPValidationError.__init__)  (18 test-only)

