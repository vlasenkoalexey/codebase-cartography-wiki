---
title: COBOL legacy migration — the most heavily marketed Spoke, and what backs its numbers
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# COBOL legacy migration — the most heavily marketed Spoke, and what backs its numbers

## Definition
The README gives legacy-COBOL modernization more space than any other downstream tool, in two
directions: "Automated Legacy Migration: COBOL to Java Spring Boot" ("converts legacy COBOL into
fully compiling, modern Spring Boot architectures, mapping memory exactly and scaffolding JPA
entities, REST controllers, and Maven builds... Proven Metric: Achieved a perfect 27/27 Maven compile
success rate"), and "Mainframe Refactoring: COBOL & JCL Optimization" ("safely neutralizes legacy
lexical traps, extracts dead execution memory, maps topological DAG execution orders... Proven
Metric: removed over 6,700 lines of dead execution blocks").

## In gitgalaxy (grounded)
These are two separate controllers, not one pipeline with two output formats:
- **COBOL-to-COBOL (dead-code, JCL, schema) is [`IRStateManager`](../concepts/gitgalaxy-cobol_refractor_controller.md)'s
  domain**, already documented in depth by the existing COBOL Refractor Controller concept page:
  [`x_ray_dead_code`](../catalog/gitgalaxy/tools/cobol_to_cobol/cobol_graveyard_finder.md#x_ray_dead_code)
  finds the dead paragraphs/orphaned variables the "6,700 lines removed" claim would come from,
  [`extract_lineage`](../catalog/gitgalaxy/tools/cobol_to_cobol/cobol_dag_architect.md#extract_lineage)
  is the "topological DAG execution order" mapper, and [`generate_zero_trust_jcl`](../catalog/gitgalaxy/tools/cobol_to_cobol/cobol_jcl_forge.md#generate_zero_trust_jcl)
  produces the "Zero-Trust JCL configurations." This page does not re-explain that mechanism — see
  the linked concept page for the shared-IR design.
- **COBOL-to-Java is a *different* top-level controller.** `gitgalaxy/cobol_refractor_controller.py`'s
  own concept page notes, as an inferred caveat, that the controller "does not import from
  `gitgalaxy.core`"; reading the tree confirms COBOL-to-Java Spring Boot generation lives in a
  sibling entry point, [`main`](../catalog/gitgalaxy/cobol_to_java_controller.md#main) in
  `cobol_to_java_controller.py` (already cited from the same concept page's symbol list) — a separate
  forge-tool chain for the Java-target direction, following the same "shared IR, independent
  regex-tool stages" pattern rather than sharing code with the COBOL-to-COBOL path.
- **The "27/27 Maven compile" claim has a real, repeatable test harness behind it — but not the
  specific corpus.** [`main`](../catalog/gitgalaxy/tools/cobol_to_java/batch_test_harness.md#main) in
  `batch_test_harness.py` shells out to run Maven compilation across `n` generated repositories and
  tallies a `failed_maven` counter — exactly the mechanism that would produce a "27/27" style success
  rate. However, the `examples/ibm_cics_translation` corpus the README points to as "verify for
  yourself" is not present in this pinned checkout, so the specific 27-repo figure cannot be
  independently re-run from this packet; what *is* verifiable is that the harness generating such a
  number is real, versioned code, not a one-off manual claim.

## Why it matters / when it applies
This is the clearest instance in the repository of `docs/wiki/01-01-project-overview.md` §1.3's "our
specialized Decoupled Execution Controllers leverage that deterministic graph to execute
enterprise-grade operations" — the only Spoke in this survey's gitgalaxy silo whose output is
*generated source code* (Spring Boot services, JPA entities, Maven builds), not a report or a
database. It is also a useful calibration point for how far to trust this doc's "Proven Metric"
callouts: the mechanism that could produce them is real and testable, but the specific headline
numbers rest on example data outside this packet's reach — worth flagging honestly rather than either
accepting or dismissing the claim wholesale.

## Connections
- Code concepts: [COBOL Refractor Controller](../concepts/gitgalaxy-cobol_refractor_controller.md) —
  the deep page on the shared-IR COBOL-to-COBOL pipeline this page defers to.
- Module catalogs: [cobol_refractor_controller](../catalog/gitgalaxy/cobol_refractor_controller.md);
  no catalog page yet exists for `cobol_to_java_controller.py` or
  `tools/cobol_to_java/batch_test_harness.py` — both symbols above are read directly from source.
- Related doc-concepts: [supply-chain-and-compliance-tools](supply-chain-and-compliance-tools.md) and
  [network-and-agent-security-tools](network-and-agent-security-tools.md) — the sibling
  "Decoupled Execution Controller" clusters covering security/compliance rather than code generation.

## Source
Extracted from `README.md` §"Enterprise Codebase Tools & Use Cases" (kept in place); the
"Decoupled Execution Controllers" framing is drawn from `docs/wiki/01-01-project-overview.md` §1.3.
