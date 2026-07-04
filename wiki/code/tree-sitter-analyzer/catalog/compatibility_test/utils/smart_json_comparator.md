---
title: 'Module: compatibility_test/utils/smart_json_comparator.py'
type: catalog
provenance: extracted
module: compatibility_test/utils/smart_json_comparator.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `compatibility_test.utils.smart_json_comparator`/SmartJsonComparator#
symbols:
  SmartJsonComparator._sort_arrays: _sort_arrays().
  SmartJsonComparator.normalize_json: normalize_json().
  SmartJsonComparator.recursive_normalize: recursive_normalize().
  SmartJsonComparator.config: config.
  SmartJsonComparator.compare_with_report: compare_with_report().
  SmartJsonComparator.generate_normalized_files: generate_normalized_files().
  SmartJsonComparator: ''
  SmartJsonComparator.__init__: __init__().
---
# Module: [`compatibility_test/utils/smart_json_comparator.py`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py)

## Classes
### `SmartJsonComparator`
- def: [`compatibility_test/utils/smart_json_comparator.py:8`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L8)
- signature: `class SmartJsonComparator:`
- members:
  - `__init__(self, config_path)` — [`L9`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L9) — 設定ファイルを読み込んで初期化
  - `_sort_arrays(self, data)` — [`L14`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L14) — 設定に基づいて配列をソートする再帰的な関数
  - `compare_with_report(self, file1_path, file2_path)` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L77) — 詳細な比較レポートを生成
  - `generate_normalized_files(self, input_dir, output_dir)` — [`L107`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L107) — 正規化されたファイルを出力ディレクトリに生成
  - `normalize_json(self, data)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L48) — JSONを正規化（無視フィールド除去、ソート等）
  - `recursive_normalize(d)` — [`L57`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L57)
  - `config` — [`L12`](../../../../../../raw/code/tree-sitter-analyzer/compatibility_test/utils/smart_json_comparator.py#L12)
- used by: [`configure_smart_comparison`](../scripts/_analyze_differences_setup.md#configure_smart_comparison)

