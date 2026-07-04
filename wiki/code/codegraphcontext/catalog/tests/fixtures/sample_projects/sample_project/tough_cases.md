---
title: 'Module: tests/fixtures/sample_projects/sample_project/tough_cases.py'
type: catalog
provenance: extracted
module: tests/fixtures/sample_projects/sample_project/tough_cases.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `tests.fixtures.sample_projects.sample_project.tough_cases`/
symbols:
  debug_logger: debug_logger().
  debug_logger.decorator: debug_logger().decorator().
  outer_scope.middle_scope: outer_scope().middle_scope().
  Service.process_data: Service#process_data().
  MethodInjector.__new__: MethodInjector#__new__().
  MagicClass: MagicClass#
  outer_scope: outer_scope().
  PlatformManager.run: PlatformManager#run().
  platform_action: platform_action().
  debug_logger.decorator.wrapper: debug_logger().decorator().wrapper().
  MethodInjector: MethodInjector#
  MethodInjector.dynamic_method: MethodInjector#dynamic_method().
  outer_scope.middle_scope.inner_scope: outer_scope().middle_scope().inner_scope().
  Service: Service#
  MagicClass.static_method: MagicClass#static_method().
  hidden_function: hidden_function().
  DynamicCaller: DynamicCaller#
  DynamicCaller.call_by_name: DynamicCaller#call_by_name().
  DynamicCaller.helper_method: DynamicCaller#helper_method().
  PlatformManager: PlatformManager#
---
# Module: [`tests/fixtures/sample_projects/sample_project/tough_cases.py`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py)

## Classes
### `DynamicCaller`
- def: [`tests/fixtures/sample_projects/sample_project/tough_cases.py:45`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L45)
- signature: `class DynamicCaller:`
- members:
  - `call_by_name(self, func_name)` — [`L46`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L46)
  - `helper_method(self)` — [`L56`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L56)

### `MagicClass`
- def: [`tests/fixtures/sample_projects/sample_project/tough_cases.py:35`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L35)
- signature: `class MagicClass(metaclass=MethodInjector):`
- members:
  - `static_method(self)` — [`L36`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L36)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `MethodInjector`  ·  implements/extends type
- def: [`tests/fixtures/sample_projects/sample_project/tough_cases.py:28`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L28)
- signature: `class MethodInjector(type):`
- members:
  - `dynamic_method(self)` — [`L30`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L30)
- protocol/private: `__new__`[`L29`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L29)
- used by: (1 test-only callers)

### `PlatformManager`
- def: [`tests/fixtures/sample_projects/sample_project/tough_cases.py:81`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L81)
- signature: `class PlatformManager:`
- members:
  - `run(self)` — [`L82`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L82)
- uses (calls/refs, reference-scoped): (1 test-only callers)

### `Service`
- def: [`tests/fixtures/sample_projects/sample_project/tough_cases.py:19`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L19)
- signature: `class Service:`
- members:
  - `process_data(self, data)` — [`L21`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L21)
- uses (calls/refs, reference-scoped): (1 test-only callers)

## Functions
- `debug_logger(prefix="")` — [`L8`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L8)
- `decorator(func)` — [`L9`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L9)
- `hidden_function()` — [`L42`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L42)
- `inner_scope()` — [`L67`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L67)
- `middle_scope()` — [`L64`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L64)
- `outer_scope()` — [`L62`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L62)
- `platform_action()` — [`L77`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L77)
- `wrapper(*args, **kwargs)` — [`L11`](../../../../../../../../raw/code/codegraphcontext/tests/fixtures/sample_projects/sample_project/tough_cases.py#L11)

