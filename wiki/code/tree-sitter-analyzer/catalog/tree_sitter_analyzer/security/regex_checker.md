---
title: 'Module: tree_sitter_analyzer/security/regex_checker.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/security/regex_checker.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.security.regex_checker`/
symbols:
  RegexSafetyChecker: RegexSafetyChecker#
  RegexSafetyChecker.validate_pattern: RegexSafetyChecker#validate_pattern().
  RegexSafetyChecker.create_safe_pattern: RegexSafetyChecker#create_safe_pattern().
  RegexSafetyChecker._check_dangerous_patterns: RegexSafetyChecker#_check_dangerous_patterns().
  RegexSafetyChecker._check_performance: RegexSafetyChecker#_check_performance().
  RegexSafetyChecker.analyze_complexity: RegexSafetyChecker#analyze_complexity().
  RegexSafetyChecker.suggest_safer_pattern: RegexSafetyChecker#suggest_safer_pattern().
  RegexSafetyChecker.DANGEROUS_PATTERNS: RegexSafetyChecker#DANGEROUS_PATTERNS.
  RegexSafetyChecker._check_compilation: RegexSafetyChecker#_check_compilation().
  RegexSafetyChecker._time_pattern_on: RegexSafetyChecker#_time_pattern_on().
  RegexSafetyChecker.MAX_PATTERN_LENGTH: RegexSafetyChecker#MAX_PATTERN_LENGTH.
  RegexSafetyChecker.MAX_EXECUTION_TIME: RegexSafetyChecker#MAX_EXECUTION_TIME.
  RegexSafetyChecker.__init__: RegexSafetyChecker#__init__().
  RegexSafetyChecker.get_safe_flags: RegexSafetyChecker#get_safe_flags().
  _REGEX_BACKTRACKING_PROBES._REGEX_BACKTRACKING_PROBES: _REGEX_BACKTRACKING_PROBES._REGEX_BACKTRACKING_PROBES.
---
# Module: [`tree_sitter_analyzer/security/regex_checker.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py)

## Classes
### `RegexSafetyChecker`
- def: [`tree_sitter_analyzer/security/regex_checker.py:24`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L24)
- doc: Regex safety checker for ReDoS attack prevention.
- signature: `class RegexSafetyChecker:`
- members:
  - `__init__(self)` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L65) — Initialize regex safety checker.
  - `_check_compilation(self, pattern: str)` — [`L145`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L145) — Check if pattern compiles successfully.
  - `_check_dangerous_patterns(self, pattern: str)` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L121) — Check for known dangerous regex patterns.
  - `_check_performance(self, pattern: str)` — [`L162`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L162) — Check pattern performance with test strings.
  - `_time_pattern_on(self, compiled_pattern: re.Pattern[str], test_string: str)` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L180) — Run search+match on ``test_string``, return error message or ``None``.
  - `analyze_complexity(self, pattern: str)` — [`L205`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L205) — Analyze regex pattern complexity.
  - `create_safe_pattern(self, pattern: str, flags: int | None = None)` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L280) — Create a safely compiled regex pattern.
  - `get_safe_flags(self)` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L270) — Get recommended safe regex flags.
  - `suggest_safer_pattern(self, pattern: str)` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L241) — Suggest a safer alternative for dangerous patterns.
  - `validate_pattern(self, pattern: str)` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L69) — Validate regex pattern for safety. — documented in [tree_sitter_analyzer-utils-logging](../../../concepts/tree_sitter_analyzer-utils-logging.md)
  - `DANGEROUS_PATTERNS` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L45)
  - `MAX_EXECUTION_TIME` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L42)
  - `MAX_PATTERN_LENGTH` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L39)
- uses (calls/refs, reference-scoped): [`log_debug`](../utils/logging.md#log_debug), [`log_warning`](../utils/logging.md#log_warning), [`_REGEX_BACKTRACKING_PROBES`](regex_checker.md#_REGEX_BACKTRACKING_PROBES._REGEX_BACKTRACKING_PROBES)
- used by: [`_resolve_query`](../cli/commands/query_command.md#QueryCommand._resolve_query), [`HAS_CTYPES`](validator.md#HAS_CTYPES), [`validate_regex_pattern`](validator.md#SecurityValidator.validate_regex_pattern), [`regex_checker`](validator.md#SecurityValidator.regex_checker)  (80 test-only)

## Module values
- `_REGEX_BACKTRACKING_PROBES` — [`L16`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/security/regex_checker.py#L16)

