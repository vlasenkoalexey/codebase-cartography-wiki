---
title: 'Module: graphify/llm.py'
type: catalog
provenance: extracted
module: graphify/llm.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.llm`/
symbols:
  extract_files_direct: extract_files_direct().
  _call_claude_cli: _call_claude_cli().
  _call_llm: _call_llm().
  extract_corpus_parallel: extract_corpus_parallel().
  _call_openai_compat: _call_openai_compat().
  BACKENDS.BACKENDS: BACKENDS.BACKENDS.
  _extract_with_adaptive_retry: _extract_with_adaptive_retry().
  label_communities: label_communities().
  _estimate_file_tokens: _estimate_file_tokens().
  _pack_chunks_by_tokens: _pack_chunks_by_tokens().
  _call_claude: _call_claude().
  _build_image_refs: _build_image_refs().
  _read_files: _read_files().
  detect_backend: detect_backend().
  _parse_llm_json: _parse_llm_json().
  _get_backend_api_key: _get_backend_api_key().
  _call_bedrock: _call_bedrock().
  _anthropic_content: _anthropic_content().
  _openai_content: _openai_content().
  generate_community_labels: generate_community_labels().
  _resolve_temperature: _resolve_temperature().
  _load_custom_providers: _load_custom_providers().
  _validate_ollama_base_url: _validate_ollama_base_url().
  _ImageRef: _ImageRef#
  _label_batch_with_retry: _label_batch_with_retry().
  _bedrock_content: _bedrock_content().
  _response_is_hollow: _response_is_hollow().
  _call_azure: _call_azure().
  _extraction_system: _extraction_system().
  _image_notes: _image_notes().
  _FILE_CHAR_CAP: _FILE_CHAR_CAP.
  _resolve_api_timeout: _resolve_api_timeout().
  _ImageRef.raw: _ImageRef#raw.
  _resolve_max_retries: _resolve_max_retries().
  _partition_semantic_files: _partition_semantic_files().
  _with_image_notes: _with_image_notes().
  _format_backend_env_keys: _format_backend_env_keys().
  _default_model_for_backend: _default_model_for_backend().
  provider_base_url_ok: provider_base_url_ok().
  _ImageRef.b64: _ImageRef#b64().
  _is_vision_image: _is_vision_image().
  _backend_supports_vision: _backend_supports_vision().
  estimate_cost: estimate_cost().
  _CHARS_PER_TOKEN: _CHARS_PER_TOKEN.
  _backend_pkg_hint: _backend_pkg_hint().
  _extract_with_adaptive_retry._split_lone_slice: _extract_with_adaptive_retry()._split_lone_slice().
  _TOKENIZER: _TOKENIZER.
  _PER_FILE_OVERHEAD_CHARS: _PER_FILE_OVERHEAD_CHARS.
  _ImageRef.path: _ImageRef#path.
  _looks_like_context_exceeded: _looks_like_context_exceeded().
  _ImageRef.media_type: _ImageRef#media_type.
  _sanitize_fragment: _sanitize_fragment().
  _bedrock_inference_config: _bedrock_inference_config().
  _file_to_text: _file_to_text().
  _ImageRef.bedrock_format: _ImageRef#bedrock_format().
  _strip_pixels: _strip_pixels().
  _backend_env_keys: _backend_env_keys().
  _azure_client: _azure_client().
  _extract_with_adaptive_retry._merge_two: _extract_with_adaptive_retry()._merge_two().
  extract_corpus_parallel._run_one: extract_corpus_parallel()._run_one().
  label_communities._run_batch: label_communities()._run_batch().
  _custom_providers_path: _custom_providers_path().
  _neutralise_injection_sentinels: _neutralise_injection_sentinels().
  _wrap_untrusted: _wrap_untrusted().
  _community_label_lines: _community_label_lines().
  _parse_label_response: _parse_label_response().
  _resolve_max_tokens: _resolve_max_tokens().
  _model_requires_default_temperature: _model_requires_default_temperature().
  _EXTRACTION_SYSTEM: _EXTRACTION_SYSTEM.
  _MAX_IMAGES_PER_CHUNK: _MAX_IMAGES_PER_CHUNK.
  _ImageRef.rel: _ImageRef#rel.
  _placeholder_community_labels: _placeholder_community_labels().
  _no_window_kwargs: _no_window_kwargs().
  _resolve_under_root: _resolve_under_root().
  _MAX_IMAGE_BYTES: _MAX_IMAGE_BYTES.
  _IMAGE_TOKEN_ESTIMATE: _IMAGE_TOKEN_ESTIMATE.
  _LLM_JSON_MAX_BYTES: _LLM_JSON_MAX_BYTES.
  _claude_cli_envelope: _claude_cli_envelope().
  _merge_into: _merge_into().
  _LABEL_BATCH_SIZE: _LABEL_BATCH_SIZE.
  label_communities._merge: label_communities()._merge().
  _get_tokenizer: _get_tokenizer().
  _DEEP_EXTRACTION_SUFFIX: _DEEP_EXTRACTION_SUFFIX.
  _INJECTION_SENTINELS: _INJECTION_SENTINELS.
  _VISION_IMAGE_EXTENSIONS: _VISION_IMAGE_EXTENSIONS.
  _IMAGE_MEDIA_TYPES: _IMAGE_MEDIA_TYPES.
  _PATH_IMAGE_BACKENDS: _PATH_IMAGE_BACKENDS.
  _CONTEXT_EXCEEDED_MARKERS: _CONTEXT_EXCEEDED_MARKERS.
  _ollama_host_is_link_local_or_metadata: _ollama_host_is_link_local_or_metadata().
  _LABEL_FENCE_RE: _LABEL_FENCE_RE.
  _LABEL_TOP_K: _LABEL_TOP_K.
  _LABEL_MAXLEN: _LABEL_MAXLEN.
  _FIXED_TEMPERATURE_MODEL_MARKERS: _FIXED_TEMPERATURE_MODEL_MARKERS.
  _LABEL_MAX_COMMUNITIES: _LABEL_MAX_COMMUNITIES.
---
# Module: [`graphify/llm.py`](../../../../../raw/code/graphify/graphify/llm.py)

## Classes
### `_ImageRef`
- def: [`graphify/llm.py:576`](../../../../../raw/code/graphify/graphify/llm.py#L576) — documented in [graphify-llm](../../concepts/graphify-llm.md)
- doc: A single image destined for a vision request.
- signature: `class _ImageRef:`
- members:
  - `b64(self)` — [`L591`](../../../../../raw/code/graphify/graphify/llm.py#L591)
  - `bedrock_format(self)` — [`L595`](../../../../../raw/code/graphify/graphify/llm.py#L595)
  - `media_type` — [`L587`](../../../../../raw/code/graphify/graphify/llm.py#L587)
  - `path` — [`L585`](../../../../../raw/code/graphify/graphify/llm.py#L585) — documented in [graphify-llm](../../concepts/graphify-llm.md)
  - `raw` — [`L588`](../../../../../raw/code/graphify/graphify/llm.py#L588)
  - `rel` — [`L586`](../../../../../raw/code/graphify/graphify/llm.py#L586)
- used by: [`_call_claude_cli`](llm.md#_call_claude_cli), [`_call_openai_compat`](llm.md#_call_openai_compat), [`_call_claude`](llm.md#_call_claude), [`_build_image_refs`](llm.md#_build_image_refs), [`_call_bedrock`](llm.md#_call_bedrock), [`_anthropic_content`](llm.md#_anthropic_content), [`_openai_content`](llm.md#_openai_content), [`_bedrock_content`](llm.md#_bedrock_content), [`_image_notes`](llm.md#_image_notes), [`_with_image_notes`](llm.md#_with_image_notes), [`_strip_pixels`](llm.md#_strip_pixels)  (7 test-only)

## Functions
- `_anthropic_content(user_message: str, refs: list[_ImageRef])` — [`L719`](../../../../../raw/code/graphify/graphify/llm.py#L719) — Build the Anthropic `messages[].content` value (str, or block list with images). — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_azure_client(api_key: str, endpoint: str)` — [`L1274`](../../../../../raw/code/graphify/graphify/llm.py#L1274) — Construct an AzureOpenAI client with env-driven api_version and timeout.
- `_backend_env_keys(backend: str)` — [`L886`](../../../../../raw/code/graphify/graphify/llm.py#L886) — Return accepted API-key environment variables for a backend. — documented in [graphify-prs](../../concepts/graphify-prs.md)
- `_backend_pkg_hint(pkg: str, extra: str)` — [`L924`](../../../../../raw/code/graphify/graphify/llm.py#L924) — Package-missing message that works for the recommended `uv tool` install. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_backend_supports_vision(backend: str)` — [`L662`](../../../../../raw/code/graphify/graphify/llm.py#L662) — Whether `backend`'s configured model can see images. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_bedrock_content(user_message: str, refs: list[_ImageRef])` — [`L748`](../../../../../raw/code/graphify/graphify/llm.py#L748) — Build the Bedrock Converse user content list (raw bytes, not base64). — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_bedrock_inference_config(max_tokens: int, model: str = "")` — [`L334`](../../../../../raw/code/graphify/graphify/llm.py#L334) — Build Bedrock inferenceConfig, honouring GRAPHIFY_LLM_TEMPERATURE.
- `_build_image_refs(image_files: list[Path], root: Path, *, read_bytes: bool = True)` — [`L617`](../../../../../raw/code/graphify/graphify/llm.py#L617) — Build `_ImageRef`s for raster images. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_call_azure(api_key: str, endpoint: str, model: str, user_message: str, temperature: float | None = 0, max_tokens: int = 8192, *, deep_mode: bool = False)` — [`L1296`](../../../../../raw/code/graphify/graphify/llm.py#L1296) — Call Azure OpenAI Service via the AzureOpenAI SDK client. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_call_bedrock(model: str, user_message: str, max_tokens: int = 8192, *, deep_mode: bool = False, images: list[_ImageRef] | None = None)` — [`L1337`](../../../../../raw/code/graphify/graphify/llm.py#L1337) — Call AWS Bedrock via boto3 Converse API using the standard AWS credential chain. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_call_claude(api_key: str, model: str, user_message: str, max_tokens: int = 8192, *, deep_mode: bool = False, images: list[_ImageRef] | None = None)` — [`L1075`](../../../../../raw/code/graphify/graphify/llm.py#L1075) — Call Anthropic Claude directly (not via OpenAI compat layer). — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_call_claude_cli(user_message: str, max_tokens: int = 8192, *, deep_mode: bool = False, images: list[_ImageRef] | None = None)` — [`L1145`](../../../../../raw/code/graphify/graphify/llm.py#L1145) — Call Claude via the locally-installed Claude Code CLI (`claude -p`). — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_call_llm(prompt: str, *, backend: str, max_tokens: int = 200, model: str | None = None)` — [`L1936`](../../../../../raw/code/graphify/graphify/llm.py#L1936) — Send a plain-text prompt to `backend` and return the model's text reply. — documented in [graphify-dedup](../../concepts/graphify-dedup.md)
- `_call_openai_compat(base_url: str, api_key: str, model: str, user_message: str, temperature: float | None = 0, reasoning_effort: str | None = None, max_completion_tokens: int = 8192, *, backend: str = "", deep_mode: bool = False, images: list[_ImageRef] | None = None, extra_body: dict | None = None)` — [`L939`](../../../../../raw/code/graphify/graphify/llm.py#L939) — Call any OpenAI-compatible API (Kimi, OpenAI, etc.) and return parsed JSON. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_claude_cli_envelope(stdout: str)` — [`L1113`](../../../../../raw/code/graphify/graphify/llm.py#L1113) — Parse the JSON returned by `claude -p --output-format json`.
- `_community_label_lines(G, communities, gods, max_communities, top_k)` — [`L2215`](../../../../../raw/code/graphify/graphify/llm.py#L2215) — One prompt line per community (largest first), sampling up to ``top_k``
- `_custom_providers_path(global_: bool = True)` — [`L178`](../../../../../raw/code/graphify/graphify/llm.py#L178)
- `_default_model_for_backend(backend: str)` — [`L913`](../../../../../raw/code/graphify/graphify/llm.py#L913) — Return configured model override or backend default model. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_estimate_file_tokens(unit: Path | FileSlice)` — [`L1493`](../../../../../raw/code/graphify/graphify/llm.py#L1493) — Estimate the prompt-token cost of a file or slice under `_read_files` rules. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `_extract_with_adaptive_retry(chunk: list[Path], backend: str, api_key: str | None, model: str | None, root: Path, max_depth: int, _depth: int = 0, *, deep_mode: bool = False)` — [`L1607`](../../../../../raw/code/graphify/graphify/llm.py#L1607) — Extract a chunk; if the response is truncated (`finish_reason="length"`) — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_extraction_system(*, deep: bool = False)` — [`L431`](../../../../../raw/code/graphify/graphify/llm.py#L431) — Return the semantic-extraction system prompt, optionally in deep mode. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_file_to_text(path: Path)` — [`L438`](../../../../../raw/code/graphify/graphify/llm.py#L438) — Return a text-like file's content for the extraction prompt.
- `_format_backend_env_keys(backend: str)` — [`L907`](../../../../../raw/code/graphify/graphify/llm.py#L907) — Return user-facing accepted API-key variable names. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_get_backend_api_key(backend: str)` — [`L898`](../../../../../raw/code/graphify/graphify/llm.py#L898) — Return the first configured API key for backend, or an empty string. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_get_tokenizer()` — [`L39`](../../../../../raw/code/graphify/graphify/llm.py#L39) — Return a tiktoken encoder for accurate token counts, or None if tiktoken
- `_image_notes(refs: list[_ImageRef], *, with_paths: bool = False)` — [`L674`](../../../../../raw/code/graphify/graphify/llm.py#L674) — Text block listing the images so the model emits one node per image. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_is_vision_image(path: Path)` — [`L600`](../../../../../raw/code/graphify/graphify/llm.py#L600)
- `_label_batch_with_retry(batch_cids: list[int], batch_lines: list[str], *, backend: str, model: str | None, depth: int = 0, max_depth: int = 3)` — [`L2263`](../../../../../raw/code/graphify/graphify/llm.py#L2263) — Label a batch of communities, splitting in half and retrying on parse failure. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_load_custom_providers()` — [`L221`](../../../../../raw/code/graphify/graphify/llm.py#L221)
- `_looks_like_context_exceeded(exc: BaseException)` — [`L1593`](../../../../../raw/code/graphify/graphify/llm.py#L1593) — Heuristically classify an exception as a context-window overflow.
- `_merge(batch_idx: int, parsed, exc)` — [`L2390`](../../../../../raw/code/graphify/graphify/llm.py#L2390)
- `_merge_into(merged: dict, result: dict)` — [`L1927`](../../../../../raw/code/graphify/graphify/llm.py#L1927) — Append a chunk result into the running merged accumulator.
- `_merge_two(left_units, right_units)` — [`L1651`](../../../../../raw/code/graphify/graphify/llm.py#L1651)
- `_model_requires_default_temperature(model: str)` — [`L283`](../../../../../raw/code/graphify/graphify/llm.py#L283) — True if `model` is a reasoning model that rejects an explicit temperature.
- `_neutralise_injection_sentinels(text: str)` — [`L479`](../../../../../raw/code/graphify/graphify/llm.py#L479) — Defang known chat-template / jailbreak control tokens in untrusted text.
- `_no_window_kwargs()` — [`L348`](../../../../../raw/code/graphify/graphify/llm.py#L348) — subprocess kwargs that suppress the console window claude.cmd would
- `_ollama_host_is_link_local_or_metadata(host: str)` — [`L2092`](../../../../../raw/code/graphify/graphify/llm.py#L2092) — True if *host* is, or resolves to, a link-local / cloud-metadata address.
- `_openai_content(user_message: str, refs: list[_ImageRef])` — [`L732`](../../../../../raw/code/graphify/graphify/llm.py#L732) — Build the OpenAI-compatible user `content` value (str, or part list with images). — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_pack_chunks_by_tokens(files: list[Path | FileSlice], token_budget: int)` — [`L1532`](../../../../../raw/code/graphify/graphify/llm.py#L1532) — Greedily pack files/slices into chunks that fit a token budget. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `_parse_label_response(text: str, labeled_cids: list[int])` — [`L2242`](../../../../../raw/code/graphify/graphify/llm.py#L2242) — Parse the backend's JSON ``{cid: name}`` reply. Raises on non-JSON or a
- `_parse_llm_json(raw: str)` — [`L786`](../../../../../raw/code/graphify/graphify/llm.py#L786) — Strip optional markdown fences and parse JSON. Returns empty fragment on failure. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_partition_semantic_files(units: list[Path | FileSlice])` — [`L604`](../../../../../raw/code/graphify/graphify/llm.py#L604) — Split a chunk into (text-like units, raster-image files). — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `_placeholder_community_labels(communities)` — [`L2211`](../../../../../raw/code/graphify/graphify/llm.py#L2211)
- `_read_files(units: list[Path | FileSlice], root: Path)` — [`L505`](../../../../../raw/code/graphify/graphify/llm.py#L505) — Return file/slice contents formatted for the extraction prompt. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `_resolve_api_timeout(default: float = 600)` — [`L360`](../../../../../raw/code/graphify/graphify/llm.py#L360) — Honour GRAPHIFY_API_TIMEOUT env var override, else use default (seconds). — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_resolve_max_retries(default: int = 6)` — [`L373`](../../../../../raw/code/graphify/graphify/llm.py#L373) — How many times the provider SDK retries a transient error (notably HTTP 429
- `_resolve_max_tokens(default: int)` — [`L261`](../../../../../raw/code/graphify/graphify/llm.py#L261) — Honour GRAPHIFY_MAX_OUTPUT_TOKENS env var override, else use backend default.
- `_resolve_temperature(default: float | None, model: str = "")` — [`L302`](../../../../../raw/code/graphify/graphify/llm.py#L302) — Resolve the temperature to send, honouring GRAPHIFY_LLM_TEMPERATURE. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_resolve_under_root(path: Path, root: Path)` — [`L452`](../../../../../raw/code/graphify/graphify/llm.py#L452) — Return the resolved path only when it stays inside ``root``.
- `_response_is_hollow(raw_content: str | None, parsed: dict)` — [`L866`](../../../../../raw/code/graphify/graphify/llm.py#L866) — Detect a successful HTTP response that yielded no usable extraction. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_run_batch(batch_idx: int)` — [`L2376`](../../../../../raw/code/graphify/graphify/llm.py#L2376)
- `_run_one(idx: int, chunk: list[Path])` — [`L1848`](../../../../../raw/code/graphify/graphify/llm.py#L1848)
- `_sanitize_fragment(parsed: dict)` — [`L762`](../../../../../raw/code/graphify/graphify/llm.py#L762) — Force ``nodes``/``edges``/``hyperedges`` to lists of dicts, in place.
- `_split_lone_slice()` — [`L1668`](../../../../../raw/code/graphify/graphify/llm.py#L1668) — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `_strip_pixels(refs: list[_ImageRef])` — [`L657`](../../../../../raw/code/graphify/graphify/llm.py#L657) — Return refs with pixel data dropped (for non-vision backends).
- `_validate_ollama_base_url(url: str, *, warn: bool = True)` — [`L2119`](../../../../../raw/code/graphify/graphify/llm.py#L2119) — Warn if OLLAMA_BASE_URL looks unsafe; hard-block link-local/metadata (F3). — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_with_image_notes(user_message: str, refs: list[_ImageRef], *, with_paths: bool = False)` — [`L710`](../../../../../raw/code/graphify/graphify/llm.py#L710) — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_wrap_untrusted(rel: str, content: str)` — [`L489`](../../../../../raw/code/graphify/graphify/llm.py#L489) — Wrap one file's content in a labelled, hash-stamped untrusted-data block.
- `detect_backend()` — [`L2166`](../../../../../raw/code/graphify/graphify/llm.py#L2166) — Return the name of whichever backend has an API key set, or None. — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `estimate_cost(backend: str, input_tokens: int, output_tokens: int)` — [`L2084`](../../../../../raw/code/graphify/graphify/llm.py#L2084) — Estimate USD cost for a given token count using published pricing.
- `extract_corpus_parallel(files: list[Path], backend: str = "kimi", api_key: str | None = None, model: str | None = None, root: Path = Path("."), chunk_size: int = 20, on_chunk_done: Callable | None = None, token_budget: int | None = 60000, max_concurrency: int = 4, max_retry_depth: int = 3, deep_mode: bool = False)` — [`L1781`](../../../../../raw/code/graphify/graphify/llm.py#L1781) — Extract a corpus in chunks, merging results. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `extract_files_direct(files: list[Path], backend: str | None = None, api_key: str | None = None, model: str | None = None, root: Path = Path("."), *, deep_mode: bool = False)` — [`L1381`](../../../../../raw/code/graphify/graphify/llm.py#L1381) — Extract semantic nodes/edges from a list of files using the given backend. — documented in [graphify-file_slice](../../concepts/graphify-file_slice.md)
- `generate_community_labels(G, communities, *, backend: str | None = None, model: str | None = None, gods=None, quiet: bool = False, max_concurrency: int = 4, batch_size: int = _LABEL_BATCH_SIZE)` — [`L2423`](../../../../../raw/code/graphify/graphify/llm.py#L2423) — CLI entry point: resolve a backend, name communities, and degrade to
- `label_communities(G, communities, *, backend: str, model: str | None = None, gods=None, max_communities: int | None = None, top_k: int = _LABEL_TOP_K, batch_size: int = _LABEL_BATCH_SIZE, max_concurrency: int = 4)` — [`L2326`](../../../../../raw/code/graphify/graphify/llm.py#L2326) — Return a complete ``{cid: name}`` map using ``backend`` for naming.
- `provider_base_url_ok(base_url: str, name: str, *, warn: bool = True)` — [`L184`](../../../../../raw/code/graphify/graphify/llm.py#L184) — Structural safety check for a custom-provider base_url.

## Module values
- `BACKENDS` — [`L59`](../../../../../raw/code/graphify/graphify/llm.py#L59) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `_CHARS_PER_TOKEN` — [`L36`](../../../../../raw/code/graphify/graphify/llm.py#L36)
- `_CONTEXT_EXCEEDED_MARKERS` — [`L1578`](../../../../../raw/code/graphify/graphify/llm.py#L1578)
- `_DEEP_EXTRACTION_SUFFIX` — [`L422`](../../../../../raw/code/graphify/graphify/llm.py#L422)
- `_EXTRACTION_SYSTEM` — [`L391`](../../../../../raw/code/graphify/graphify/llm.py#L391)
- `_FILE_CHAR_CAP` — [`L29`](../../../../../raw/code/graphify/graphify/llm.py#L29) — documented in [graphify-llm](../../concepts/graphify-llm.md)
- `_FIXED_TEMPERATURE_MODEL_MARKERS` — [`L280`](../../../../../raw/code/graphify/graphify/llm.py#L280)
- `_IMAGE_MEDIA_TYPES` — [`L548`](../../../../../raw/code/graphify/graphify/llm.py#L548)
- `_IMAGE_TOKEN_ESTIMATE` — [`L562`](../../../../../raw/code/graphify/graphify/llm.py#L562)
- `_INJECTION_SENTINELS` — [`L469`](../../../../../raw/code/graphify/graphify/llm.py#L469)
- `_LABEL_BATCH_SIZE` — [`L2208`](../../../../../raw/code/graphify/graphify/llm.py#L2208)
- `_LABEL_FENCE_RE` — [`L2204`](../../../../../raw/code/graphify/graphify/llm.py#L2204)
- `_LABEL_MAXLEN` — [`L2207`](../../../../../raw/code/graphify/graphify/llm.py#L2207)
- `_LABEL_MAX_COMMUNITIES` — [`L2205`](../../../../../raw/code/graphify/graphify/llm.py#L2205)
- `_LABEL_TOP_K` — [`L2206`](../../../../../raw/code/graphify/graphify/llm.py#L2206)
- `_LLM_JSON_MAX_BYTES` — [`L759`](../../../../../raw/code/graphify/graphify/llm.py#L759)
- `_MAX_IMAGES_PER_CHUNK` — [`L568`](../../../../../raw/code/graphify/graphify/llm.py#L568)
- `_MAX_IMAGE_BYTES` — [`L558`](../../../../../raw/code/graphify/graphify/llm.py#L558)
- `_PATH_IMAGE_BACKENDS` — [`L572`](../../../../../raw/code/graphify/graphify/llm.py#L572)
- `_PER_FILE_OVERHEAD_CHARS` — [`L33`](../../../../../raw/code/graphify/graphify/llm.py#L33)
- `_TOKENIZER` — [`L57`](../../../../../raw/code/graphify/graphify/llm.py#L57)
- `_VISION_IMAGE_EXTENSIONS` — [`L547`](../../../../../raw/code/graphify/graphify/llm.py#L547)

