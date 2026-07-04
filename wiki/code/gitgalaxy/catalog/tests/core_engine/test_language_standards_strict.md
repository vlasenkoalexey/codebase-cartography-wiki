---
title: 'Module: tests/core_engine/test_language_standards_strict.py'
type: catalog
provenance: extracted
module: tests/core_engine/test_language_standards_strict.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.core_engine.test_language_standards_strict`/
symbols:
  assert_redos_immune: assert_redos_immune().
  test_c_knr_ambiguity_trap: test_c_knr_ambiguity_trap().
  test_csharp_iron_wall_redos: test_csharp_iron_wall_redos().
  test_cpp_macro_multiline_spiral: test_cpp_macro_multiline_spiral().
  test_c_pointer_ambiguity_overlap: test_c_pointer_ambiguity_overlap().
  test_global_regex_syntax_integrity: test_global_regex_syntax_integrity().
  test_cobol_ghost_satellite_prevention: test_cobol_ghost_satellite_prevention().
  test_thermodynamic_operator_collisions: test_thermodynamic_operator_collisions().
  test_redos_detonator_timeout_catch: test_redos_detonator_timeout_catch().
  test_global_regex_syntax_integrity_catch: test_global_regex_syntax_integrity_catch().
  _detonate: _detonate().
---
# Module: [`tests/core_engine/test_language_standards_strict.py`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py)

## Functions
- `_detonate(pattern: re.Pattern, payload: str, result_queue: multiprocessing.Queue)` — [`L11`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L11) — Executes a regex against a payload inside an isolated OS process.
- `assert_redos_immune(pattern: re.Pattern, payload: str, timeout_sec: float = 1)` — [`L21`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L21) — Runs a regex in an isolated process. If it exceeds timeout_sec, it is
- `test_c_knr_ambiguity_trap()` — [`L51`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L51) — Proves the C/C++ function spawner does not spiral into a 32,768-permutation — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- `test_c_pointer_ambiguity_overlap()` — [`L131`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L131) — Proves that O(1) alternation `(?:\s*[*&]+\s*|\s+)` successfully prevents — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- `test_cobol_ghost_satellite_prevention()` — [`L151`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L151) — Proves that heavily indented SQL queries or data divisions are explicitly — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- `test_cpp_macro_multiline_spiral()` — [`L107`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L107) — Proves the C++ function spawner respects the (?![ 	]*#) negative lookaheads — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- `test_csharp_iron_wall_redos()` — [`L79`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L79) — Proves the C# function spawner survives pathologically massive nested return — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- `test_global_regex_syntax_integrity()` — [`L217`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L217) — A final sanity check. Iterates over EVERY regex in the entire file and — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)
- `test_global_regex_syntax_integrity_catch(monkeypatch)` — [`L258`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L258) — Proves the fuzzer catches malformed regex objects.
- `test_redos_detonator_timeout_catch()` — [`L243`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L243) — Proves the Blast Chamber successfully catches and kills hung regexes.
- `test_thermodynamic_operator_collisions()` — [`L181`](../../../../../../raw/code/gitgalaxy/tests/core_engine/test_language_standards_strict.py#L181) — Proves that common language operators (<<, |, &, !) do not trigger false — documented in [gitgalaxy-standards-language_standards](../../../concepts/gitgalaxy-standards-language_standards.md)

