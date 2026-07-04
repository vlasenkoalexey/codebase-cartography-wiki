---
title: 'Module: gitgalaxy/recorders/llm_recorder.py'
type: catalog
provenance: extracted
module: gitgalaxy/recorders/llm_recorder.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.recorders.llm_recorder`/LLMRecorder#
symbols:
  LLMRecorder.RISK_SCHEMA: RISK_SCHEMA.
  LLMRecorder.SIGNAL_SCHEMA: SIGNAL_SCHEMA.
  LLMRecorder.logger: logger.
  LLMRecorder.generate_artifacts: generate_artifacts().
  LLMRecorder._build_markdown: _build_markdown().
  LLMRecorder._generate_sqlite_graph: _generate_sqlite_graph().
  LLMRecorder: ''
  LLMRecorder._parse_threat_score: _parse_threat_score().
  LLMRecorder.__init__: __init__().
---
# Module: [`gitgalaxy/recorders/llm_recorder.py`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py)

## Classes
### `LLMRecorder`
- def: [`gitgalaxy/recorders/llm_recorder.py:23`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L23)
- doc: PURPOSE: Translates raw GitGalaxy telemetry into AI-optimized artifacts.
- signature: `class LLMRecorder:`
- members:
  - `_build_markdown(self, parsed_files: List[Dict[str, Any]], unparsable_files: List[Dict[str, Any]], summary: Dict[str, Any], session_meta: Dict[str, Any], forensic_report: Dict[str, Any])` — [`L133`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L133) — Constructs a high-density, context-rich Markdown brief for LLM agents.
  - `_generate_sqlite_graph(self, parsed_files: List[Dict[str, Any]], summary: Dict[str, Any], session: Dict[str, Any], db_path: Path, inbound_map: Dict[str, List[str]])` — [`L1198`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L1198) — Creates a relational database for advanced SQL-based AI analysis.
  - `_parse_threat_score(self, artifact: Dict)` — [`L48`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L48) — Safely extracts and converts the AI threat score string to a float.
  - `generate_artifacts(self, parsed_files: List[Dict[str, Any]], unparsable_files: List[Dict[str, Any]], summary: Dict[str, Any], session_meta: Dict[str, Any], output_dir: str, forensic_report: Optional[Dict[str, Any]] = None)` — [`L56`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L56) — Generates the dual-output AI artifacts: Markdown and SQLite.
  - `RISK_SCHEMA` — [`L45`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L45)
  - `SIGNAL_SCHEMA` — [`L46`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L46)
  - `logger` — [`L37`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L37)
- protocol/private: `__init__`[`L35`](../../../../../../raw/code/gitgalaxy/gitgalaxy/recorders/llm_recorder.py#L35)
- used by: [`execute_pipeline`](../galaxyscope.md#Orchestrator.execute_pipeline), [`llm_recorder`](../galaxyscope.md#Orchestrator.llm_recorder)  (1 test-only)

