---
title: Supply-chain and compliance tools — Spokes that reuse the Aperture Filter as a library
type: doc-concept
provenance: doc
source: README.md
updated: 2026-07-04
status: fresh
---
# Supply-chain and compliance tools — Spokes that reuse the Aperture Filter as a library

## Definition
Alongside the main GalaxyScope scan, the README lists a cluster of standalone CLI tools it frames as
"Decoupled Execution Controllers" that "leverage that deterministic graph to execute enterprise-grade
operations": a "Zero-Trust SBOM Generation & Dependency Auditing" tool that "refuses to blindly trust
`package.json` or `requirements.txt`... instead locating the physical dependencies on disk,
mathematically verifying their entropy and linguistic identity," and a "Software Supply Chain
Security & Pre-Commit Firewall" suite that "scans physical internals to block steganography,
byte-level XOR decryption loops, homoglyph typosquatting, and exposed cryptographic vaults."

## In gitgalaxy (grounded)
Each named capability maps to a real, independently importable module rather than a repackaging of
the main pipeline:
- **SBOM generation.** [`UniversalManifestSlicer`](../catalog/gitgalaxy/tools/compliance/sbom_generator.md#UniversalManifestSlicer)
  in `sbom_generator.py` is the class behind the "Zero-Trust SBOM" claim; its own `main()` entry point
  is already cited from [the COBOL Refractor Controller page](../concepts/gitgalaxy-cobol_refractor_controller.md)'s
  symbol list as [`main`](../catalog/gitgalaxy/tools/compliance/sbom_generator.md#main).
- **Alias resolution shared across tools.** [`ManifestParser.build_resolution_map`](../catalog/gitgalaxy/security/manifest_parser.md#ManifestParser.build_resolution_map) —
  already cited from the same page — is the one utility [`GalaxyScope's Phase 10`](../concepts/gitgalaxy-galaxyscope.md)
  explicitly reuses across the SBOM, X-Ray, and Firewall audits so a package alias only needs
  resolving once.
- **Pre-commit firewall.** [`run_firewall_audit`](../catalog/gitgalaxy/tools/supply_chain_security/supply_chain_firewall.md#run_firewall_audit)
  and its own `main()` (both already cited from the Cobol Refractor Controller page) are the
  "physical internals" scanner the README describes.
- **Vault/secrets sentinel.** [`main`](../catalog/gitgalaxy/tools/supply_chain_security/vault_sentinel.md#main)
  in `vault_sentinel.py` is a standalone CLI whose only structural dependency, per
  [the Aperture Filter concept page](../concepts/gitgalaxy-core-aperture.md)'s own Entry points
  section, is [`ApertureFilter.evaluate_path_integrity`](../catalog/gitgalaxy/core/aperture.md#ApertureFilter.evaluate_path_integrity) —
  the same Tier-0.1 "secrets radar" check the main GalaxyScope scan runs, reused here directly as a
  library call rather than re-implemented.
- **Binary/entropy anomaly detection (X-Ray).** [`main`](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md#main)
  and [`run_xray_audit`](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md#run_xray_audit)
  are the "byte-level XOR decryption loops" / entropy-anomaly scanner, and — per the same Aperture
  page — also call `evaluate_path_integrity` directly, independent of a full GalaxyScope run.

## Why it matters / when it applies
The Aperture Filter concept page already noted these two tools reuse
`ApertureFilter.evaluate_path_integrity` "outside the primary structural pipeline," but treated that
as an isolated observation about the filter. Read against the README, it is the general pattern for
this whole tool cluster: none of the five is a thin CLI wrapper around a full `Orchestrator.execute_pipeline`
run — each imports exactly the shared-core pieces it needs (the Aperture gate, the manifest resolver)
and layers its own domain logic on top, which is the concrete mechanism behind the README's own
"Decoupled Architecture" framing (`docs/wiki/01-01-project-overview.md` §1.3: "the core engine
provides the overarching structural mechanics... our specialized Decoupled Execution Controllers
leverage that deterministic graph"). Every one of these tools' `main()` also runs behind
[`enforce_licensing_guard`](../concepts/gitgalaxy-licensing.md) — the licensing page's own framing
("called from essentially every entry point in the repository") applies to this whole cluster, not
just the primary scanner.

## Connections
- Code concepts: [The Aperture Filter](../concepts/gitgalaxy-core-aperture.md) — the shared gate this
  whole cluster reuses; [COBOL Refractor Controller](../concepts/gitgalaxy-cobol_refractor_controller.md) —
  the sibling "Decoupled Execution Controller" for the legacy-migration direction, cross-linked from
  [cobol-legacy-migration-pipeline](cobol-legacy-migration-pipeline.md); [Licensing guard](../concepts/gitgalaxy-licensing.md) —
  the RSA gate every tool's `main()` calls first.
- Module catalogs: [aperture](../catalog/gitgalaxy/core/aperture.md), [manifest_parser](../catalog/gitgalaxy/security/manifest_parser.md),
  [sbom_generator](../catalog/gitgalaxy/tools/compliance/sbom_generator.md), [supply_chain_firewall](../catalog/gitgalaxy/tools/supply_chain_security/supply_chain_firewall.md),
  [vault_sentinel](../catalog/gitgalaxy/tools/supply_chain_security/vault_sentinel.md), [binary_anomaly_detector](../catalog/gitgalaxy/tools/supply_chain_security/binary_anomaly_detector.md).
- Related doc-concepts: [network-and-agent-security-tools](network-and-agent-security-tools.md) —
  the sibling tool cluster covering API/PII/agent-guardrail Spokes; [cobol-legacy-migration-pipeline](cobol-legacy-migration-pipeline.md) —
  the same Hub-and-Spoke pattern applied to code generation rather than security scanning.

## Source
Extracted from `README.md` §"Enterprise Codebase Tools & Use Cases" (kept in place); the
"Decoupled Architecture" framing is echoed in `docs/wiki/01-01-project-overview.md` §1.3, cited here
rather than duplicated into its own page.
