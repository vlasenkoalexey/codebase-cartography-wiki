---
title: 'Module: benchmarks/codegraph_compare/schemas.py'
type: catalog
provenance: extracted
module: benchmarks/codegraph_compare/schemas.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `benchmarks.codegraph_compare.schemas`/
symbols:
  RunRecord: RunRecord#
  QuestionSpec.__post_init__: QuestionSpec#__post_init__().
  RunRecord.cache_read_tokens: RunRecord#cache_read_tokens.
  RunRecord.cache_creation_tokens: RunRecord#cache_creation_tokens.
  RunRecord.total_cost_usd: RunRecord#total_cost_usd.
  RunRecord.num_turns: RunRecord#num_turns.
  QuestionSpec.category: QuestionSpec#category.
  RunRecord.session_id: RunRecord#session_id.
  QuestionSpec.anti_hallucination_checks: QuestionSpec#anti_hallucination_checks.
  RunRecord.run_id: RunRecord#run_id.
  RunRecord.repo: RunRecord#repo.
  RunRecord.question_id: RunRecord#question_id.
  RunRecord.arm: RunRecord#arm.
  RunRecord.repeat: RunRecord#repeat.
  RunRecord.started_at: RunRecord#started_at.
  RunRecord.ended_at: RunRecord#ended_at.
  RunRecord.elapsed_seconds: RunRecord#elapsed_seconds.
  RunRecord.input_tokens: RunRecord#input_tokens.
  RunRecord.output_tokens: RunRecord#output_tokens.
  RunRecord.total_tokens: RunRecord#total_tokens.
  RunRecord.estimated_cost_usd: RunRecord#estimated_cost_usd.
  RunRecord.tool_calls: RunRecord#tool_calls.
  RunRecord.file_reads: RunRecord#file_reads.
  RunRecord.search_calls: RunRecord#search_calls.
  RunRecord.index_queries: RunRecord#index_queries.
  RunRecord.answer: RunRecord#answer.
  RunRecord.citations: RunRecord#citations.
  RunRecord.transcript_path: RunRecord#transcript_path.
  RunRecord.error: RunRecord#error.
  RunRecord.agent_backend: RunRecord#agent_backend.
  RunRecord.model: RunRecord#model.
  RunRecord.cached_input_tokens: RunRecord#cached_input_tokens.
  RunRecord.reasoning_output_tokens: RunRecord#reasoning_output_tokens.
  RunRecord.make_id: RunRecord#make_id().
  EvalRecord: EvalRecord#
  EvalRecord.run_id: EvalRecord#run_id.
  EvalRecord.correctness: EvalRecord#correctness.
  EvalRecord.completeness: EvalRecord#completeness.
  EvalRecord.citation_quality: EvalRecord#citation_quality.
  EvalRecord.hallucination_risk: EvalRecord#hallucination_risk.
  EvalRecord.overall: EvalRecord#overall.
  EvalRecord.missing_key_points: EvalRecord#missing_key_points.
  EvalRecord.bad_citations: EvalRecord#bad_citations.
  EvalRecord.evaluator_model: EvalRecord#evaluator_model.
  EvalRecord.evaluated_at: EvalRecord#evaluated_at.
  RepoSpec: RepoSpec#
  RepoSpec.id: RepoSpec#id.
  RepoSpec.name: RepoSpec#name.
  RepoSpec.language: RepoSpec#language.
  RepoSpec.url: RepoSpec#url.
  RepoSpec.commit: RepoSpec#commit.
  RepoSpec.approx_files: RepoSpec#approx_files.
  QuestionSpec: QuestionSpec#
  QuestionSpec.id: QuestionSpec#id.
  QuestionSpec.repo: QuestionSpec#repo.
  QuestionSpec.prompt: QuestionSpec#prompt.
  QuestionSpec.expected_key_points: QuestionSpec#expected_key_points.
  QuestionSpec.must_cite_files: QuestionSpec#must_cite_files.
  ArmSpec: ArmSpec#
  ArmSpec.id: ArmSpec#id.
  ArmSpec.adapter: ArmSpec#adapter.
  ArmSpec.index_mode: ArmSpec#index_mode.
  IndexStats: IndexStats#
  IndexStats.build_seconds: IndexStats#build_seconds.
  IndexStats.index_size_bytes: IndexStats#index_size_bytes.
  IndexStats.file_count: IndexStats#file_count.
  ToolMetrics: ToolMetrics#
  ToolMetrics.tool_calls: ToolMetrics#tool_calls.
  ToolMetrics.file_reads: ToolMetrics#file_reads.
  ToolMetrics.search_calls: ToolMetrics#search_calls.
  ToolMetrics.index_queries: ToolMetrics#index_queries.
---
# Module: [`benchmarks/codegraph_compare/schemas.py`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py)

## Classes
### `ArmSpec`
- def: [`benchmarks/codegraph_compare/schemas.py:125`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L125)
- doc: One treatment arm (tool combination) in the benchmark.
- signature: `class ArmSpec:`
- members:
  - `adapter` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L129)
  - `id` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L128)
  - `index_mode` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L130)

### `EvalRecord`
- def: [`benchmarks/codegraph_compare/schemas.py:69`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L69)
- doc: LLM-judge scores for one RunRecord.
- signature: `class EvalRecord:`
- members:
  - `bad_citations` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L79)
  - `citation_quality` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L75)
  - `completeness` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L74)
  - `correctness` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L73)
  - `evaluated_at` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L81)
  - `evaluator_model` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L80)
  - `hallucination_risk` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L76)
  - `missing_key_points` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L78)
  - `overall` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L77)
  - `run_id` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L72)

### `IndexStats`
- def: [`benchmarks/codegraph_compare/schemas.py:134`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L134)
- doc: Timing and size stats from a single index build.
- signature: `class IndexStats:`
- members:
  - `build_seconds` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L137)
  - `file_count` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L139)
  - `index_size_bytes` — [`L138`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L138)

### `QuestionSpec`
- def: [`benchmarks/codegraph_compare/schemas.py:97`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L97)
- doc: One benchmark question bound to a specific repo.
- signature: `class QuestionSpec:`
- members:
  - `anti_hallucination_checks` — [`L106`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L106)
  - `category` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L102)
  - `expected_key_points` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L104)
  - `id` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L100)
  - `must_cite_files` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L105)
  - `prompt` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L103)
  - `repo` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L101)
- protocol/private: `__post_init__`[`L108`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L108)

### `RepoSpec`
- def: [`benchmarks/codegraph_compare/schemas.py:85`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L85)
- doc: A pinned repository entry from repos.yaml.
- signature: `class RepoSpec:`
- members:
  - `approx_files` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L93)
  - `commit` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L92)
  - `id` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L88)
  - `language` — [`L90`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L90)
  - `name` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L89)
  - `url` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L91)

### `RunRecord`
- def: [`benchmarks/codegraph_compare/schemas.py:15`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L15)
- doc: One execution of a question under one arm at one repeat index.
- signature: `class RunRecord:`
- members:
  - `make_id(cls, question_id: str, arm: str, repeat: int, agent_backend: str = "claude")` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L61) — Return the canonical run_id string.
  - `agent_backend` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L38)
  - `answer` — [`L34`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L34)
  - `arm` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L21)
  - `cache_creation_tokens` — [`L51`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L51)
  - `cache_read_tokens` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L50)
  - `cached_input_tokens` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L40)
  - `citations` — [`L35`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L35)
  - `elapsed_seconds` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L25)
  - `ended_at` — [`L24`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L24)
  - `error` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L37)
  - `estimated_cost_usd` — [`L29`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L29)
  - `file_reads` — [`L31`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L31)
  - `index_queries` — [`L33`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L33)
  - `input_tokens` — [`L26`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L26)
  - `model` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L39)
  - `num_turns` — [`L53`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L53)
  - `output_tokens` — [`L27`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L27)
  - `question_id` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L20)
  - `reasoning_output_tokens` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L41)
  - `repeat` — [`L22`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L22)
  - `repo` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L19)
  - `run_id` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L18)
  - `search_calls` — [`L32`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L32)
  - `session_id` — [`L58`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L58)
  - `started_at` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L23)
  - `tool_calls` — [`L30`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L30)
  - `total_cost_usd` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L52)
  - `total_tokens` — [`L28`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L28)
  - `transcript_path` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L36)
- used by: (4 test-only callers)

### `ToolMetrics`
- def: [`benchmarks/codegraph_compare/schemas.py:143`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L143)
- doc: Tool-call breakdown extracted from a single run transcript.
- signature: `class ToolMetrics:`
- members:
  - `file_reads` — [`L147`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L147)
  - `index_queries` — [`L149`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L149)
  - `search_calls` — [`L148`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L148)
  - `tool_calls` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/benchmarks/codegraph_compare/schemas.py#L146)

