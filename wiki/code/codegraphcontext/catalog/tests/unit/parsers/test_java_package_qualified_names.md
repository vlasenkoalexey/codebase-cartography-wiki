---
title: 'Module: tests/unit/parsers/test_java_package_qualified_names.py'
type: catalog
provenance: extracted
module: tests/unit/parsers/test_java_package_qualified_names.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.unit.parsers.test_java_package_qualified_names`/
symbols:
  _write_and_parse: _write_and_parse().
  BILLING_SERVICE_SRC: BILLING_SERVICE_SRC.
  NO_PACKAGE_SRC: NO_PACKAGE_SRC.
  TestPackageNameExtraction.test_package_name_present_when_declared: TestPackageNameExtraction#test_package_name_present_when_declared().
  TestPackageNameExtraction.test_package_name_for_interface: TestPackageNameExtraction#test_package_name_for_interface().
  TestPackageNameExtraction.test_package_name_is_none_without_declaration: TestPackageNameExtraction#test_package_name_is_none_without_declaration().
  TestPackageNameExtraction.test_package_name_key_always_present: TestPackageNameExtraction#test_package_name_key_always_present().
  TestFunctionQualifiedName.test_method_qualified_name_includes_package_and_class: TestFunctionQualifiedName#test_method_qualified_name_includes_package_and_class().
  TestFunctionQualifiedName.test_all_methods_have_qualified_name: TestFunctionQualifiedName#test_all_methods_have_qualified_name().
  TestFunctionQualifiedName.test_method_qualified_name_uses_actual_method_name: TestFunctionQualifiedName#test_method_qualified_name_uses_actual_method_name().
  TestFunctionQualifiedName.test_no_qualified_name_without_package: TestFunctionQualifiedName#test_no_qualified_name_without_package().
  TestClassQualifiedName.test_class_qualified_name_is_package_dot_classname: TestClassQualifiedName#test_class_qualified_name_is_package_dot_classname().
  TestClassQualifiedName.test_interface_qualified_name: TestClassQualifiedName#test_interface_qualified_name().
  TestClassQualifiedName.test_no_class_qualified_name_without_package: TestClassQualifiedName#test_no_class_qualified_name_without_package().
  INTERFACE_SRC: INTERFACE_SRC.
  TestPreScanJavaFQNEntries.test_pre_scan_adds_fqn_entry: TestPreScanJavaFQNEntries#test_pre_scan_adds_fqn_entry().
  TestPreScanJavaFQNEntries.test_pre_scan_retains_short_name_entry: TestPreScanJavaFQNEntries#test_pre_scan_retains_short_name_entry().
  TestPreScanJavaFQNEntries.test_pre_scan_adds_interface_fqn: TestPreScanJavaFQNEntries#test_pre_scan_adds_interface_fqn().
  TestPreScanJavaFQNEntries.test_pre_scan_no_fqn_without_package: TestPreScanJavaFQNEntries#test_pre_scan_no_fqn_without_package().
  parser: parser().
  INNER_CLASS_SRC: INNER_CLASS_SRC.
  TestPackageNameExtraction: TestPackageNameExtraction#
  TestFunctionQualifiedName: TestFunctionQualifiedName#
  TestClassQualifiedName: TestClassQualifiedName#
  TestPreScanJavaFQNEntries: TestPreScanJavaFQNEntries#
---
# Module: [`tests/unit/parsers/test_java_package_qualified_names.py`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py)

## Classes
### `TestClassQualifiedName`
- def: [`tests/unit/parsers/test_java_package_qualified_names.py:163`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L163)
- signature: `class TestClassQualifiedName:`
- members:
  - `test_class_qualified_name_is_package_dot_classname(self, parser)` — [`L165`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L165) — Class qualified_name must be package.ClassName.
  - `test_interface_qualified_name(self, parser)` — [`L175`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L175) — Interface nodes must also carry qualified_name.
  - `test_no_class_qualified_name_without_package(self, parser)` — [`L182`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L182) — Classes in packageless files must not have qualified_name.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestFunctionQualifiedName`
- def: [`tests/unit/parsers/test_java_package_qualified_names.py:125`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L125)
- signature: `class TestFunctionQualifiedName:`
- members:
  - `test_all_methods_have_qualified_name(self, parser)` — [`L137`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L137) — Every method in a packaged class must have a non-empty qualified_name.
  - `test_method_qualified_name_includes_package_and_class(self, parser)` — [`L127`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L127) — A class method qualified_name must be package.ClassName.methodName.
  - `test_method_qualified_name_uses_actual_method_name(self, parser)` — [`L144`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L144) — calculateTotal qualified_name must end with the correct method name.
  - `test_no_qualified_name_without_package(self, parser)` — [`L150`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L150) — Methods in files with no package declaration must not have qualified_name.
- uses (calls/refs, reference-scoped): (3 test-only callers)

### `TestPackageNameExtraction`
- def: [`tests/unit/parsers/test_java_package_qualified_names.py:98`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L98)
- signature: `class TestPackageNameExtraction:`
- members:
  - `test_package_name_for_interface(self, parser)` — [`L105`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L105) — Interface files must also export package_name.
  - `test_package_name_is_none_without_declaration(self, parser)` — [`L110`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L110) — Files with no package statement must return package_name=None.
  - `test_package_name_key_always_present(self, parser)` — [`L115`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L115) — The package_name key must always be in the result dict, even when None.
  - `test_package_name_present_when_declared(self, parser)` — [`L100`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L100) — parse() must return package_name matching the Java package statement.
- uses (calls/refs, reference-scoped): (4 test-only callers)

### `TestPreScanJavaFQNEntries`
- def: [`tests/unit/parsers/test_java_package_qualified_names.py:193`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L193)
- signature: `class TestPreScanJavaFQNEntries:`
- members:
  - `test_pre_scan_adds_fqn_entry(self, tmp_path)` — [`L195`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L195) — pre_scan_java must add com.example.acme.billing.BillingService -> [path] entry.
  - `test_pre_scan_adds_interface_fqn(self, tmp_path)` — [`L229`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L229) — pre_scan_java must add FQN entries for interfaces as well as classes.
  - `test_pre_scan_no_fqn_without_package(self, tmp_path)` — [`L245`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L245) — Files without a package declaration must not produce FQN entries.
  - `test_pre_scan_retains_short_name_entry(self, tmp_path)` — [`L213`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L213) — pre_scan_java must still register the short name BillingService -> [path].
- uses (calls/refs, reference-scoped): (3 test-only callers)

## Functions
- `_write_and_parse(parser, src: str)` — [`L37`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L37)
- `parser()` — [`L28`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L28)

## Module values
- `BILLING_SERVICE_SRC` — [`L53`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L53)
- `INNER_CLASS_SRC` — [`L81`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L81)
- `INTERFACE_SRC` — [`L67`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L67)
- `NO_PACKAGE_SRC` — [`L75`](../../../../../../../raw/code/codegraphcontext/tests/unit/parsers/test_java_package_qualified_names.py#L75)

