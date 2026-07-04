---
title: 'Module: gitgalaxy/core/guidestar_lens.py'
type: catalog
provenance: extracted
module: gitgalaxy/core/guidestar_lens.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.core.guidestar_lens`/GuideStarLens#
symbols:
  GuideStarLens.scan_project_config: scan_project_config().
  GuideStarLens.logger: logger.
  GuideStarLens._inject_intent_lock: _inject_intent_lock().
  GuideStarLens._deep_inspect_manifest: _deep_inspect_manifest().
  GuideStarLens.get_intent_status: get_intent_status().
  GuideStarLens._scan_package_manifests: _scan_package_manifests().
  GuideStarLens._calculate_documentation_coverage: _calculate_documentation_coverage().
  GuideStarLens._scan_gitattributes: _scan_gitattributes().
  GuideStarLens._scan_gitignore_evasion: _scan_gitignore_evasion().
  GuideStarLens._extract_execution_triggers: _extract_execution_triggers().
  GuideStarLens.root: root.
  GuideStarLens.documentation_coverage: documentation_coverage.
  GuideStarLens._gs_config: _gs_config.
  GuideStarLens._detect_ai_ecosystem: _detect_ai_ecosystem().
  GuideStarLens: ''
  GuideStarLens.intent_locks: intent_locks.
  GuideStarLens.pattern_locks: pattern_locks.
  GuideStarLens.MANIFEST_MAP: MANIFEST_MAP.
  GuideStarLens.INTENT_BIASED_SECTORS: INTENT_BIASED_SECTORS.
  GuideStarLens.EXEC_PREFIX_MAP: EXEC_PREFIX_MAP.
  GuideStarLens._inject_pattern_lock: _inject_pattern_lock().
  GuideStarLens._parse_package_json: _parse_package_json().
  GuideStarLens._parse_makefile: _parse_makefile().
  GuideStarLens._parse_toml_style_manifest: _parse_toml_style_manifest().
  GuideStarLens.whitelist: whitelist.
  GuideStarLens.README_TARGET_HEADERS: README_TARGET_HEADERS.
  GuideStarLens.__init__: __init__().
---
# Module: [`gitgalaxy/core/guidestar_lens.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py)

## Classes
### `GuideStarLens`
- def: [`gitgalaxy/core/guidestar_lens.py:25`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L25)
- doc: The GuideStar Lens provides Contextual Baselines for files by parsing repository
- signature: `class GuideStarLens:`
- members:
  - `__init__(self, root_path: Union[str, Path], priority_whitelist: Optional[List[str]] = None, parent_logger: Optional[logging.Logger] = None)` — [`L49`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L49) — Initializes the Intelligence Engine and calibrates the lock maps.
  - `_calculate_documentation_coverage(self)` — [`L421`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L421) — Scans the repository for high-value architectural literature. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_deep_inspect_manifest(self, path: Path, filename: str, lang: str)` — [`L196`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L196) — Dispatches files to specific parsers based on their format. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_detect_ai_ecosystem(self, content: str, filename: str)` — [`L213`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L213) — Scans manifest files for explicit AI/LLM orchestrators or tensor frameworks. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_extract_execution_triggers(self, text: str)` — [`L302`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L302) — Finds extensionless files used in command-line examples and infers exact language. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_inject_intent_lock(self, filename: str, lang: str, confidence: float, proof: str)` — [`L137`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L137) — Safely updates the lock map with evidence-based intelligence. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_inject_pattern_lock(self, pattern: str, lang: str, confidence: float, proof: str)` — [`L161`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L161) — Safely updates the pattern lock map with wildcard evidence. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_parse_makefile(self, path: Path)` — [`L265`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L265) — Parses Makefiles to find source variables and targets. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_parse_package_json(self, path: Path)` — [`L236`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L236) — Extracts 'main', 'bin', and 'scripts' from Node/JS manifests. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_parse_toml_style_manifest(self, path: Path, lang: str)` — [`L287`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L287) — Simple regex-based TOML parser for script/entry points. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_scan_gitattributes(self)` — [`L322`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L322) — Parses .gitattributes for explicit linguist-language overrides. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_scan_gitignore_evasion(self)` — [`L376`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L376) — Scans .gitignore for hostile force-includes (e.g., !payload.so). — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `_scan_package_manifests(self)` — [`L180`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L180) — Identifies authoritative project contextual baselines and parses their internal logic. — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `get_intent_status(self, path: Union[str, Path])` — [`L101`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L101) — Returns the specific Intent Lock for a given file path based on strict, pattern, or sector match.
  - `scan_project_config(self)` — [`L77`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L77) — Phase 0.5: Main orchestration method that dispatches scouts to scan — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `EXEC_PREFIX_MAP` — [`L41`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L41)
  - `INTENT_BIASED_SECTORS` — [`L40`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L40)
  - `MANIFEST_MAP` — [`L39`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L39) — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `README_TARGET_HEADERS` — [`L44`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L44)
  - `documentation_coverage` — [`L73`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L73) — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `intent_locks` — [`L67`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L67) — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `logger` — [`L57`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L57)
  - `pattern_locks` — [`L70`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L70) — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
  - `root` — [`L63`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L63)
  - `whitelist` — [`L64`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L64) — documented in [gitgalaxy-core-guidestar_lens](../../../concepts/gitgalaxy-core-guidestar_lens.md)
- protocol/private: `_gs_config`[`L37`](../../../../../../raw/code/gitgalaxy/gitgalaxy/core/guidestar_lens.py#L37)
- uses (calls/refs, reference-scoped): [`GUIDESTAR_CONFIG`](../standards/gitgalaxy_config.md#GUIDESTAR_CONFIG)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`_init_worker`](../galaxyscope.md#_init_worker), [`_inspect_path`](../galaxyscope.md#Orchestrator._inspect_path), [`guidestar`](../galaxyscope.md#Orchestrator.guidestar)  (1 test-only)

