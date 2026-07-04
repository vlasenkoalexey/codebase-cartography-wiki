---
title: 'Module: tests/unit/test_go_method_resolution.py'
type: catalog
provenance: extracted
module: tests/unit/test_go_method_resolution.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tests.unit.test_go_method_resolution`/
symbols:
  _ctx: _ctx().
  test_resolve_callee_routes_go_to_go_resolver: test_resolve_callee_routes_go_to_go_resolver().
  test_resolve_callee_go_stdlib_through_registry: test_resolve_callee_go_stdlib_through_registry().
  test_build_context_built_when_go_file_present: test_build_context_built_when_go_file_present().
  test_no_cross_language_mis_wire_end_to_end: test_no_cross_language_mis_wire_end_to_end().
  test_end_to_end_variable_named_like_stdlib_stays_unknown: test_end_to_end_variable_named_like_stdlib_stays_unknown().
  test_end_to_end_go_stdlib_and_local: test_end_to_end_go_stdlib_and_local().
  test_go_is_registered_via_discovery: test_go_is_registered_via_discovery().
  test_same_file_func_resolves_local: test_same_file_func_resolves_local().
  test_stdlib_package_call_classifies_stdlib: test_stdlib_package_call_classifies_stdlib().
  test_strings_package_call_classifies_stdlib: test_strings_package_call_classifies_stdlib().
  test_stdlib_qualifier_without_import_stays_unknown: test_stdlib_qualifier_without_import_stays_unknown().
  test_blank_import_does_not_enable_stdlib_qualifier: test_blank_import_does_not_enable_stdlib_qualifier().
  test_aliased_stdlib_import_uses_alias_not_package_name: test_aliased_stdlib_import_uses_alias_not_package_name().
  test_aliased_stdlib_import_resolves_under_alias: test_aliased_stdlib_import_resolves_under_alias().
  test_commented_import_does_not_enable_stdlib_qualifier: test_commented_import_does_not_enable_stdlib_qualifier().
  test_third_party_subpath_collision_through_resolver_stays_unknown: test_third_party_subpath_collision_through_resolver_stays_unknown().
  test_receiver_method_call_stays_unknown: test_receiver_method_call_stays_unknown().
  test_unknown_package_qualifier_stays_unknown: test_unknown_package_qualifier_stays_unknown().
  test_project_shadows_stdlib_package_name: test_project_shadows_stdlib_package_name().
  test_bare_name_not_in_file_stays_unknown: test_bare_name_not_in_file_stays_unknown().
  test_no_cross_language_mis_wire_direct: test_no_cross_language_mis_wire_direct().
  test_build_context_returns_none_without_go_files: test_build_context_returns_none_without_go_files().
  test_line_comment_in_import_block_is_not_an_import: test_line_comment_in_import_block_is_not_an_import().
  test_trailing_line_comment_after_spec_is_not_an_import: test_trailing_line_comment_after_spec_is_not_an_import().
  test_block_comment_in_import_block_is_not_an_import: test_block_comment_in_import_block_is_not_an_import().
  test_third_party_path_ending_in_stdlib_name_is_not_import_evidence: test_third_party_path_ending_in_stdlib_name_is_not_import_evidence().
  test_third_party_plain_import_ending_in_stdlib_name_is_not_evidence: test_third_party_plain_import_ending_in_stdlib_name_is_not_evidence().
  test_canonical_stdlib_subpath_is_import_evidence: test_canonical_stdlib_subpath_is_import_evidence().
---
# Module: [`tests/unit/test_go_method_resolution.py`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py)

## Functions
- `_ctx(symbols: dict[str, list[tuple[str, str, int]]], *, imports: dict[str, str] | None = None)` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L83) — Build a Go context for unit tests.
- `test_aliased_stdlib_import_resolves_under_alias()` — [`L190`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L190) — The alias qualifier itself resolves to stdlib when it aliases a stdlib
- `test_aliased_stdlib_import_uses_alias_not_package_name()` — [`L175`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L175) — ``jsonx "encoding/json"`` makes ``jsonx`` the qualifier; a bare
- `test_bare_name_not_in_file_stays_unknown()` — [`L336`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L336)
- `test_blank_import_does_not_enable_stdlib_qualifier()` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L164) — A blank import (``_ "net/http"``) is side-effect only — the package
- `test_block_comment_in_import_block_is_not_an_import()` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L230) — A ``/* "net/http" */`` block comment must be stripped before matching —
- `test_build_context_built_when_go_file_present()` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L68)
- `test_build_context_returns_none_without_go_files()` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L57)
- `test_canonical_stdlib_subpath_is_import_evidence()` — [`L280`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L280) — Genuine multi-segment stdlib paths (``net/http``, ``encoding/json``,
- `test_commented_import_does_not_enable_stdlib_qualifier()` — [`L241`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L241) — End-to-end of finding 2 through the resolver: a ``// "net/http"`` comment
- `test_end_to_end_go_stdlib_and_local(tmp_path: Path)` — [`L471`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L471) — Full index: a same-file func call stays ``local``; a stdlib
- `test_end_to_end_variable_named_like_stdlib_stays_unknown(tmp_path: Path)` — [`L435`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L435) — Codex P2 end-to-end: a local variable named ``http`` (no ``net/http``
- `test_go_is_registered_via_discovery()` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L42) — Dropping ``languages/go.py`` auto-registers the Go resolver — no edit to
- `test_line_comment_in_import_block_is_not_an_import()` — [`L208`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L208) — A ``// "net/http"`` line comment inside a grouped import must NOT be
- `test_no_cross_language_mis_wire_direct()` — [`L379`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L379) — A Go caller's bare ``helper`` must NEVER resolve to a Python file that
- `test_no_cross_language_mis_wire_end_to_end(tmp_path: Path)` — [`L398`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L398) — Index a polyglot repo where ``ToUpper`` exists as a Python def AND is
- `test_project_shadows_stdlib_package_name()` — [`L327`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L327) — If the project itself defines a symbol named like a stdlib package
- `test_receiver_method_call_stays_unknown()` — [`L309`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L309) — ``s.Run()`` — ``s`` is a local variable whose struct type the edge does
- `test_resolve_callee_go_stdlib_through_registry()` — [`L364`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L364)
- `test_resolve_callee_routes_go_to_go_resolver()` — [`L347`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L347)
- `test_same_file_func_resolves_local()` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L123)
- `test_stdlib_package_call_classifies_stdlib()` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L129)
- `test_stdlib_qualifier_without_import_stays_unknown()` — [`L151`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L151) — Codex P2: a receiver whose name collides with a stdlib package
- `test_strings_package_call_classifies_stdlib()` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L140)
- `test_third_party_path_ending_in_stdlib_name_is_not_import_evidence()` — [`L260`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L260) — ``import jsonx "github.com/acme/json"`` must NOT register ``json`` (nor
- `test_third_party_plain_import_ending_in_stdlib_name_is_not_evidence()` — [`L270`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L270) — A plain ``import "example.com/fmt"`` ends in ``fmt`` but is third-party —
- `test_third_party_subpath_collision_through_resolver_stays_unknown()` — [`L295`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L295) — End-to-end of finding 3: a file importing only ``github.com/acme/json``
- `test_trailing_line_comment_after_spec_is_not_an_import()` — [`L219`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L219) — A trailing ``// "net/http"`` after a real ``"fmt"`` import must be
- `test_unknown_package_qualifier_stays_unknown()` — [`L317`](../../../../../../raw/code/tree-sitter-analyzer/tests/unit/test_go_method_resolution.py#L317) — A non-stdlib package qualifier (third-party / domain) is conservatively

