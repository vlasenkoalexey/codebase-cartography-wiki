---
title: 'Module: graphify/detect.py'
type: catalog
provenance: extracted
module: graphify/detect.py
status: fresh
symbol_base: scip-python python graphify 0.0.0 `graphify.detect`/
symbols:
  detect: detect().
  classify_file: classify_file().
  FileType: FileType#
  _shebang_interpreter: _shebang_interpreter().
  _is_ignored: _is_ignored().
  save_manifest: save_manifest().
  _load_graphifyignore: _load_graphifyignore().
  FileType.CODE: FileType#CODE.
  _is_sensitive: _is_sensitive().
  CODE_EXTENSIONS: CODE_EXTENSIONS.
  detect_incremental: detect_incremental().
  load_manifest: load_manifest().
  _zip_within_caps: _zip_within_caps().
  count_words: count_words().
  _env_command_args: _env_command_args().
  _is_noise_dir: _is_noise_dir().
  _shebang_file_type: _shebang_file_type().
  FileType.DOCUMENT: FileType#DOCUMENT.
  convert_office_file: convert_office_file().
  FileType.VIDEO: FileType#VIDEO.
  _file_within_size_cap: _file_within_size_cap().
  xlsx_extract_structure: xlsx_extract_structure().
  _looks_like_paper: _looks_like_paper().
  _resolves_under_root: _resolves_under_root().
  extract_pdf_text: extract_pdf_text().
  xlsx_to_markdown: xlsx_to_markdown().
  FileType.PAPER: FileType#PAPER.
  _generic_keyword_hit: _generic_keyword_hit().
  _split_env_s: _split_env_s().
  _load_graphifyinclude: _load_graphifyinclude().
  _MANIFEST_PATH: _MANIFEST_PATH.
  docx_to_markdown: docx_to_markdown().
  _is_ignored._eval: _is_ignored()._eval().
  FileType.IMAGE: FileType#IMAGE.
  PAPER_EXTENSIONS: PAPER_EXTENSIONS.
  IMAGE_EXTENSIONS: IMAGE_EXTENSIONS.
  xlsx_extract_structure._nid: xlsx_extract_structure()._nid().
  _find_vcs_root: _find_vcs_root().
  DOC_EXTENSIONS: DOC_EXTENSIONS.
  xlsx_extract_structure._add: xlsx_extract_structure()._add().
  xlsx_extract_structure._edge: xlsx_extract_structure()._edge().
  _SKIP_DIRS: _SKIP_DIRS.
  _stat_and_hash: _stat_and_hash().
  _parse_gitignore_line: _parse_gitignore_line().
  _is_ignored._eval._matches: _is_ignored()._eval()._matches().
  _is_included._matches: _is_included()._matches().
  _is_included: _is_included().
  OFFICE_EXTENSIONS: OFFICE_EXTENSIONS.
  _OFFICE_MAX_DECOMPRESSED_BYTES: _OFFICE_MAX_DECOMPRESSED_BYTES.
  _md5_file: _md5_file().
  save_manifest._normalise_entry: save_manifest()._normalise_entry().
  VIDEO_EXTENSIONS: VIDEO_EXTENSIONS.
  CORPUS_WARN_THRESHOLD: CORPUS_WARN_THRESHOLD.
  CORPUS_UPPER_THRESHOLD: CORPUS_UPPER_THRESHOLD.
  FILE_COUNT_UPPER: FILE_COUNT_UPPER.
  _OFFICE_MAX_RAW_BYTES: _OFFICE_MAX_RAW_BYTES.
  _OFFICE_MAX_COMPRESSION_RATIO: _OFFICE_MAX_COMPRESSION_RATIO.
  _SENSITIVE_DIRS: _SENSITIVE_DIRS.
  _SENSITIVE_PATTERNS: _SENSITIVE_PATTERNS.
  _GENERIC_KEYWORD_PATTERNS: _GENERIC_KEYWORD_PATTERNS.
  _WORD_SPLIT: _WORD_SPLIT.
  _PAPER_SIGNALS: _PAPER_SIGNALS.
  _PAPER_SIGNAL_THRESHOLD: _PAPER_SIGNAL_THRESHOLD.
  _ASSET_DIR_MARKERS: _ASSET_DIR_MARKERS.
  _SHEBANG_CODE_INTERPRETERS: _SHEBANG_CODE_INTERPRETERS.
  _SKIP_FILES: _SKIP_FILES.
  _VCS_MARKERS: _VCS_MARKERS.
  _to_relative_for_storage: _to_relative_for_storage().
  _to_absolute_from_storage: _to_absolute_from_storage().
  _could_contain_included_path: _could_contain_included_path().
  _auto_follow_symlinks: _auto_follow_symlinks().
---
# Module: [`graphify/detect.py`](../../../../../raw/code/graphify/graphify/detect.py)

## Classes
### `FileType`  ·  implements/extends Enum, str
- def: [`graphify/detect.py:20`](../../../../../raw/code/graphify/graphify/detect.py#L20) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- signature: `class FileType(str, Enum):`
- members:
  - `CODE` — [`L21`](../../../../../raw/code/graphify/graphify/detect.py#L21) — documented in [graphify-detect](../../concepts/graphify-detect.md)
  - `DOCUMENT` — [`L22`](../../../../../raw/code/graphify/graphify/detect.py#L22) — documented in [graphify-detect](../../concepts/graphify-detect.md)
  - `IMAGE` — [`L24`](../../../../../raw/code/graphify/graphify/detect.py#L24)
  - `PAPER` — [`L23`](../../../../../raw/code/graphify/graphify/detect.py#L23)
  - `VIDEO` — [`L25`](../../../../../raw/code/graphify/graphify/detect.py#L25) — documented in [graphify-detect](../../concepts/graphify-detect.md)
- used by: [`detect`](detect.md#detect), [`classify_file`](detect.md#classify_file), [`_shebang_file_type`](detect.md#_shebang_file_type)  (34 test-only)

## Functions
- `_add(nid: str, label: str)` — [`L546`](../../../../../raw/code/graphify/graphify/detect.py#L546)
- `_auto_follow_symlinks(root: Path)` — [`L993`](../../../../../raw/code/graphify/graphify/detect.py#L993) — Return whether ``root`` has any direct symlinked child.
- `_could_contain_included_path(path: Path, root: Path, patterns: list[tuple[Path, str]])` — [`L961`](../../../../../raw/code/graphify/graphify/detect.py#L961) — Return True if a directory may contain files matched by .graphifyinclude.
- `_edge(src: str, tgt: str, relation: str)` — [`L552`](../../../../../raw/code/graphify/graphify/detect.py#L552)
- `_env_command_args(args: list[str], *, allow_split: bool = True)` — [`L220`](../../../../../raw/code/graphify/graphify/detect.py#L220) — Strip leading env(1) options and var assignments, return the trailing — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_eval(target: Path)` — [`L811`](../../../../../raw/code/graphify/graphify/detect.py#L811) — Apply last-match-wins to a single target path.
- `_file_within_size_cap(path: Path, cap: int = _OFFICE_MAX_RAW_BYTES)` — [`L51`](../../../../../raw/code/graphify/graphify/detect.py#L51) — True if *path* exists and its on-disk size is within *cap*.
- `_find_vcs_root(start: Path)` — [`L730`](../../../../../raw/code/graphify/graphify/detect.py#L730) — Walk upward from start; return the first directory containing a VCS marker.
- `_generic_keyword_hit(name: str)` — [`L134`](../../../../../raw/code/graphify/graphify/detect.py#L134) — True if a generic secret keyword appears load-bearing in the filename.
- `_is_ignored(path: Path, root: Path, patterns: list[tuple[Path, str]], *, _cache: dict[Path, bool] | None = None)` — [`L788`](../../../../../raw/code/graphify/graphify/detect.py#L788) — Return True if the path should be ignored per .graphifyignore patterns. — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `_is_included(path: Path, root: Path, patterns: list[tuple[Path, str]])` — [`L912`](../../../../../raw/code/graphify/graphify/detect.py#L912) — Return True if path matches any .graphifyinclude allowlist pattern.
- `_is_noise_dir(part: str, parent: Path | None = None)` — [`L688`](../../../../../raw/code/graphify/graphify/detect.py#L688) — Return True if this directory name looks like a venv, cache, or dep dir. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_is_sensitive(path: Path)` — [`L176`](../../../../../raw/code/graphify/graphify/detect.py#L176) — Return True if this file likely contains secrets and should be skipped. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_load_graphifyignore(root: Path)` — [`L743`](../../../../../raw/code/graphify/graphify/detect.py#L743) — Read .graphifyignore files and return (anchor_dir, pattern) pairs. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_load_graphifyinclude(root: Path)` — [`L882`](../../../../../raw/code/graphify/graphify/detect.py#L882) — Read .graphifyinclude allowlist patterns from root and ancestors.
- `_looks_like_paper(path: Path)` — [`L191`](../../../../../raw/code/graphify/graphify/detect.py#L191) — Heuristic: does this text file read like an academic paper? — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_matches(rel: str, p: str, anchored: bool)` — [`L815`](../../../../../raw/code/graphify/graphify/detect.py#L815)
- `_matches(rel: str, p: str, anchored: bool)` — [`L917`](../../../../../raw/code/graphify/graphify/detect.py#L917)
- `_md5_file(path: Path)` — [`L1188`](../../../../../raw/code/graphify/graphify/detect.py#L1188) — MD5 of file contents streamed in 64KB chunks — for change detection only.
- `_nid(*parts: str)` — [`L520`](../../../../../raw/code/graphify/graphify/detect.py#L520)
- `_normalise_entry(entry)` — [`L1301`](../../../../../raw/code/graphify/graphify/detect.py#L1301)
- `_parse_gitignore_line(raw: str)` — [`L706`](../../../../../raw/code/graphify/graphify/detect.py#L706) — Parse one raw line from a .graphifyignore file per gitignore spec.
- `_resolves_under_root(path: Path, root: Path)` — [`L1009`](../../../../../raw/code/graphify/graphify/detect.py#L1009) — True when ``path`` resolves to a target inside ``root``. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_shebang_file_type(path: Path)` — [`L378`](../../../../../raw/code/graphify/graphify/detect.py#L378) — Peek at the first line of an extensionless file for a shebang. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_shebang_interpreter(path: Path)` — [`L343`](../../../../../raw/code/graphify/graphify/detect.py#L343) — Return the interpreter name from a shebang line. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `_split_env_s(value: str, rest: list[str])` — [`L213`](../../../../../raw/code/graphify/graphify/detect.py#L213) — Re-tokenize an `env -S`/`--split-string` packed command, prepending the
- `_stat_and_hash(path_str: str)` — [`L1201`](../../../../../raw/code/graphify/graphify/detect.py#L1201) — Stat + MD5 a single file; returns None on OSError (e.g. deleted mid-run).
- `_to_absolute_from_storage(key: str, root: Path)` — [`L1240`](../../../../../raw/code/graphify/graphify/detect.py#L1240) — Inverse of :func:`_to_relative_for_storage`.
- `_to_relative_for_storage(key: str, root: Path)` — [`L1210`](../../../../../raw/code/graphify/graphify/detect.py#L1210) — Return ``key`` as a forward-slash relative path from ``root``.
- `_zip_within_caps(path: Path)` — [`L59`](../../../../../raw/code/graphify/graphify/detect.py#L59) — Reject a zip-based office file that is a likely zip/XML bomb. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `classify_file(path: Path)` — [`L386`](../../../../../raw/code/graphify/graphify/detect.py#L386) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `convert_office_file(path: Path, out_dir: Path)` — [`L604`](../../../../../raw/code/graphify/graphify/detect.py#L604) — Convert a .docx or .xlsx to a markdown sidecar in out_dir. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `count_words(path: Path)` — [`L645`](../../../../../raw/code/graphify/graphify/detect.py#L645) — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `detect(root: Path, *, follow_symlinks: bool | None = None, google_workspace: bool | None = None, extra_excludes: list[str] | None = None)` — [`L1018`](../../../../../raw/code/graphify/graphify/detect.py#L1018) — documented in [graphify-__main__](../../concepts/graphify-__main__.md)
- `detect_incremental(root: Path, manifest_path: str = _MANIFEST_PATH, *, follow_symlinks: bool | None = None, google_workspace: bool | None = None, kind: str = "semantic", extra_excludes: list[str] | None = None)` — [`L1358`](../../../../../raw/code/graphify/graphify/detect.py#L1358) — Like detect(), but returns only new or modified files since the last run. — documented in [graphify-detect](../../concepts/graphify-detect.md)
- `docx_to_markdown(path: Path)` — [`L440`](../../../../../raw/code/graphify/graphify/detect.py#L440) — Convert a .docx file to markdown text using python-docx.
- `extract_pdf_text(path: Path)` — [`L423`](../../../../../raw/code/graphify/graphify/detect.py#L423) — Extract plain text from a PDF file using pypdf.
- `load_manifest(manifest_path: str = _MANIFEST_PATH, *, root: Path | None = None)` — [`L1255`](../../../../../raw/code/graphify/graphify/detect.py#L1255) — Load the manifest from a previous run. Returns {} on any error.
- `save_manifest(files: dict[str, list[str]], manifest_path: str = _MANIFEST_PATH, *, kind: str = "both", root: Path | None = None)` — [`L1277`](../../../../../raw/code/graphify/graphify/detect.py#L1277) — Save current file mtimes + content hashes for change detection. — documented in [graphify-watch](../../concepts/graphify-watch.md)
- `xlsx_extract_structure(path: Path)` — [`L514`](../../../../../raw/code/graphify/graphify/detect.py#L514) — Extract structural nodes (sheets, named tables, column headers) from an .xlsx file.
- `xlsx_to_markdown(path: Path)` — [`L482`](../../../../../raw/code/graphify/graphify/detect.py#L482) — Convert an .xlsx file to markdown text using openpyxl.

## Module values
- `CODE_EXTENSIONS` — [`L30`](../../../../../raw/code/graphify/graphify/detect.py#L30) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `CORPUS_UPPER_THRESHOLD` — [`L38`](../../../../../raw/code/graphify/graphify/detect.py#L38)
- `CORPUS_WARN_THRESHOLD` — [`L37`](../../../../../raw/code/graphify/graphify/detect.py#L37)
- `DOC_EXTENSIONS` — [`L31`](../../../../../raw/code/graphify/graphify/detect.py#L31)
- `FILE_COUNT_UPPER` — [`L39`](../../../../../raw/code/graphify/graphify/detect.py#L39)
- `IMAGE_EXTENSIONS` — [`L33`](../../../../../raw/code/graphify/graphify/detect.py#L33) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `OFFICE_EXTENSIONS` — [`L34`](../../../../../raw/code/graphify/graphify/detect.py#L34)
- `PAPER_EXTENSIONS` — [`L32`](../../../../../raw/code/graphify/graphify/detect.py#L32) — documented in [graphify-analyze](../../concepts/graphify-analyze.md)
- `VIDEO_EXTENSIONS` — [`L35`](../../../../../raw/code/graphify/graphify/detect.py#L35)
- `_ASSET_DIR_MARKERS` — [`L202`](../../../../../raw/code/graphify/graphify/detect.py#L202)
- `_GENERIC_KEYWORD_PATTERNS` — [`L123`](../../../../../raw/code/graphify/graphify/detect.py#L123)
- `_MANIFEST_PATH` — [`L28`](../../../../../raw/code/graphify/graphify/detect.py#L28)
- `_OFFICE_MAX_COMPRESSION_RATIO` — [`L48`](../../../../../raw/code/graphify/graphify/detect.py#L48)
- `_OFFICE_MAX_DECOMPRESSED_BYTES` — [`L47`](../../../../../raw/code/graphify/graphify/detect.py#L47)
- `_OFFICE_MAX_RAW_BYTES` — [`L46`](../../../../../raw/code/graphify/graphify/detect.py#L46)
- `_PAPER_SIGNALS` — [`L158`](../../../../../raw/code/graphify/graphify/detect.py#L158)
- `_PAPER_SIGNAL_THRESHOLD` — [`L173`](../../../../../raw/code/graphify/graphify/detect.py#L173)
- `_SENSITIVE_DIRS` — [`L99`](../../../../../raw/code/graphify/graphify/detect.py#L99)
- `_SENSITIVE_PATTERNS` — [`L105`](../../../../../raw/code/graphify/graphify/detect.py#L105)
- `_SHEBANG_CODE_INTERPRETERS` — [`L205`](../../../../../raw/code/graphify/graphify/detect.py#L205)
- `_SKIP_DIRS` — [`L660`](../../../../../raw/code/graphify/graphify/detect.py#L660)
- `_SKIP_FILES` — [`L682`](../../../../../raw/code/graphify/graphify/detect.py#L682)
- `_VCS_MARKERS` — [`L703`](../../../../../raw/code/graphify/graphify/detect.py#L703)
- `_WORD_SPLIT` — [`L131`](../../../../../raw/code/graphify/graphify/detect.py#L131)

