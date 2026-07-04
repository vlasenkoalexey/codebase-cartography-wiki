---
title: 'Module: graphify/transcribe.py'
type: catalog
provenance: extracted
module: graphify/transcribe.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.transcribe`/
symbols:
  transcribe: transcribe().
  download_audio: download_audio().
  build_whisper_prompt: build_whisper_prompt().
  transcribe_all: transcribe_all().
  VIDEO_EXTENSIONS: VIDEO_EXTENSIONS.
  _TRANSCRIPTS_DIR: _TRANSCRIPTS_DIR.
  _model_name: _model_name().
  is_url: is_url().
  _FALLBACK_PROMPT: _FALLBACK_PROMPT.
  URL_PREFIXES: URL_PREFIXES.
  _DEFAULT_MODEL: _DEFAULT_MODEL.
  _get_whisper: _get_whisper().
  _get_yt_dlp: _get_yt_dlp().
---
# Module: [`graphify/transcribe.py`](../../../../../raw/code/graphify/graphify/transcribe.py)

## Functions
- `_get_whisper()` — [`L23`](../../../../../raw/code/graphify/graphify/transcribe.py#L23)
- `_get_yt_dlp()` — [`L34`](../../../../../raw/code/graphify/graphify/transcribe.py#L34)
- `_model_name()` — [`L19`](../../../../../raw/code/graphify/graphify/transcribe.py#L19)
- `build_whisper_prompt(god_nodes: list[dict])` — [`L95`](../../../../../raw/code/graphify/graphify/transcribe.py#L95) — Build a domain hint for Whisper from god nodes extracted from the corpus.
- `download_audio(url: str, output_dir: Path)` — [`L50`](../../../../../raw/code/graphify/graphify/transcribe.py#L50) — Download audio-only stream from a URL using yt-dlp.
- `is_url(path: str)` — [`L45`](../../../../../raw/code/graphify/graphify/transcribe.py#L45) — Return True if the string looks like a URL rather than a file path.
- `transcribe(video_path: Path | str, output_dir: Path | None = None, initial_prompt: str | None = None, force: bool = False)` — [`L118`](../../../../../raw/code/graphify/graphify/transcribe.py#L118) — Transcribe a video/audio file or URL to a .txt transcript.
- `transcribe_all(video_files: list[str], output_dir: Path | None = None, initial_prompt: str | None = None)` — [`L166`](../../../../../raw/code/graphify/graphify/transcribe.py#L166) — Transcribe a list of video/audio files or URLs, return paths to transcript .txt files.

## Module values
- `URL_PREFIXES` — [`L12`](../../../../../raw/code/graphify/graphify/transcribe.py#L12)
- `VIDEO_EXTENSIONS` — [`L11`](../../../../../raw/code/graphify/graphify/transcribe.py#L11)
- `_DEFAULT_MODEL` — [`L14`](../../../../../raw/code/graphify/graphify/transcribe.py#L14)
- `_FALLBACK_PROMPT` — [`L16`](../../../../../raw/code/graphify/graphify/transcribe.py#L16)
- `_TRANSCRIPTS_DIR` — [`L15`](../../../../../raw/code/graphify/graphify/transcribe.py#L15)

