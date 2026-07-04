---
title: 'Module: gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py'
type: catalog
provenance: extracted
module: gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `gitgalaxy.tools.cobol_to_cobol.cobol_etl_unpacker`/
symbols:
  main: main().
  unpack_comp3: unpack_comp3().
  unpack_ebcdic_file: unpack_ebcdic_file().
  calculate_byte_layout: calculate_byte_layout().
  calculate_byte_layout.count_nines: calculate_byte_layout().count_nines().
---
# Module: [`gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py)

## Functions
- `calculate_byte_layout(schema_json: dict)` — [`L26`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py#L26) — Parses the GitGalaxy JSON Schema to calculate the physical byte footprint
- `count_nines(s)` — [`L56`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py#L56)
- `main()` — [`L177`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py#L177)
- `unpack_comp3(raw_bytes: bytes, decimals: int)` — [`L87`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py#L87) — Decodes IBM Packed Decimal (COMP-3) hex values into standard Python floats.
- `unpack_ebcdic_file(binary_filepath: Path, schema_filepath: Path, output_filepath: Path)` — [`L110`](../../../../../../../raw/code/gitgalaxy/gitgalaxy/tools/cobol_to_cobol/cobol_etl_unpacker.py#L110) — Parses the mainframe binary file according to the calculated layout.

