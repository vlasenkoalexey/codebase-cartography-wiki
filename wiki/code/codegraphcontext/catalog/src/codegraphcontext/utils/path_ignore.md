---
title: 'Module: src/codegraphcontext/utils/path_ignore.py'
type: catalog
provenance: extracted
module: src/codegraphcontext/utils/path_ignore.py
status: fresh
symbol_base: scip-python python codegraphcontext 0.0.0 `src.codegraphcontext.utils.path_ignore`/
symbols:
  file_path_has_ignore_dir_segment: file_path_has_ignore_dir_segment().
  cypher_path_not_under_ignore_dirs: cypher_path_not_under_ignore_dirs().
  parse_ignore_dir_names: parse_ignore_dir_names().
---
# Module: [`src/codegraphcontext/utils/path_ignore.py`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_ignore.py)

## Functions
- `cypher_path_not_under_ignore_dirs(path_var: str, ignore_dir_names: Optional[List[str]] = None)` — [`L24`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_ignore.py#L24) — Returns a Cypher fragment that keeps only paths not under any IGNORE_DIRS segment — documented in [codegraphcontext-tools-code_finder](../../../../concepts/codegraphcontext-tools-code_finder.md)
- `file_path_has_ignore_dir_segment(file_path: Path, index_root: Path)` — [`L40`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_ignore.py#L40) — True if any directory segment of file_path relative to index_root matches — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)
- `parse_ignore_dir_names()` — [`L16`](../../../../../../../raw/code/codegraphcontext/src/codegraphcontext/utils/path_ignore.py#L16) — Directory names from IGNORE_DIRS, falling back to defaults when unset or empty. — documented in [codegraphcontext-cli-config_manager](../../../../concepts/codegraphcontext-cli-config_manager.md)

