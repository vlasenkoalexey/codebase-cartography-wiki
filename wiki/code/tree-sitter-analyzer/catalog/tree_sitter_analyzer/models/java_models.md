---
title: 'Module: tree_sitter_analyzer/models/java_models.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/models/java_models.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.models.java_models`/
symbols:
  JavaAnnotation.to_summary_item: JavaAnnotation#to_summary_item().
  JavaMethod.to_summary_item: JavaMethod#to_summary_item().
  JavaClass.to_summary_item: JavaClass#to_summary_item().
  JavaField.to_summary_item: JavaField#to_summary_item().
  JavaImport.to_summary_item: JavaImport#to_summary_item().
  JavaPackage.to_summary_item: JavaPackage#to_summary_item().
  JavaPackage: JavaPackage#
  JavaAnnotation: JavaAnnotation#
  JavaPackage.name: JavaPackage#name.
  JavaMethod.annotations: JavaMethod#annotations.
  JavaClass.annotations: JavaClass#annotations.
  JavaField.annotations: JavaField#annotations.
  JavaPackage.start_line: JavaPackage#start_line.
  JavaPackage.end_line: JavaPackage#end_line.
  JavaAnnotation.name: JavaAnnotation#name.
  JavaAnnotation.start_line: JavaAnnotation#start_line.
  JavaAnnotation.end_line: JavaAnnotation#end_line.
  JavaMethod: JavaMethod#
  JavaMethod.name: JavaMethod#name.
  JavaMethod.start_line: JavaMethod#start_line.
  JavaMethod.end_line: JavaMethod#end_line.
  JavaClass: JavaClass#
  JavaClass.name: JavaClass#name.
  JavaClass.start_line: JavaClass#start_line.
  JavaClass.end_line: JavaClass#end_line.
  JavaField: JavaField#
  JavaField.name: JavaField#name.
  JavaField.start_line: JavaField#start_line.
  JavaField.end_line: JavaField#end_line.
  JavaImport: JavaImport#
  JavaImport.name: JavaImport#name.
  JavaImport.start_line: JavaImport#start_line.
  JavaImport.end_line: JavaImport#end_line.
  JavaAnnotation.parameters: JavaAnnotation#parameters.
  JavaAnnotation.raw_text: JavaAnnotation#raw_text.
  JavaMethod.return_type: JavaMethod#return_type.
  JavaMethod.parameters: JavaMethod#parameters.
  JavaMethod.modifiers: JavaMethod#modifiers.
  JavaMethod.visibility: JavaMethod#visibility.
  JavaMethod.throws: JavaMethod#throws.
  JavaMethod.is_constructor: JavaMethod#is_constructor.
  JavaMethod.is_abstract: JavaMethod#is_abstract.
  JavaMethod.is_static: JavaMethod#is_static.
  JavaMethod.is_final: JavaMethod#is_final.
  JavaMethod.complexity_score: JavaMethod#complexity_score.
  JavaMethod.file_path: JavaMethod#file_path.
  JavaClass.full_qualified_name: JavaClass#full_qualified_name.
  JavaClass.package_name: JavaClass#package_name.
  JavaClass.class_type: JavaClass#class_type.
  JavaClass.modifiers: JavaClass#modifiers.
  JavaClass.visibility: JavaClass#visibility.
  JavaClass.extends_class: JavaClass#extends_class.
  JavaClass.implements_interfaces: JavaClass#implements_interfaces.
  JavaClass.is_nested: JavaClass#is_nested.
  JavaClass.parent_class: JavaClass#parent_class.
  JavaClass.file_path: JavaClass#file_path.
  JavaField.field_type: JavaField#field_type.
  JavaField.modifiers: JavaField#modifiers.
  JavaField.visibility: JavaField#visibility.
  JavaField.is_static: JavaField#is_static.
  JavaField.is_final: JavaField#is_final.
  JavaField.file_path: JavaField#file_path.
  JavaImport.module_name: JavaImport#module_name.
  JavaImport.imported_name: JavaImport#imported_name.
  JavaImport.import_statement: JavaImport#import_statement.
  JavaImport.line_number: JavaImport#line_number.
  JavaImport.is_static: JavaImport#is_static.
  JavaImport.is_wildcard: JavaImport#is_wildcard.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/models/java_models.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py)

## Classes
### `JavaAnnotation`
- def: [`tree_sitter_analyzer/models/java_models.py:14`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L14)
- doc: Java annotation representation
- signature: `class JavaAnnotation:`
- members:
  - `to_summary_item(self)` — [`L23`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L23) — Return dictionary for summary item
  - `end_line` — [`L20`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L20)
  - `name` — [`L17`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L17)
  - `parameters` — [`L18`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L18)
  - `raw_text` — [`L21`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L21)
  - `start_line` — [`L19`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L19)
- used by: [`annotations`](java_models.md#JavaClass.annotations), [`annotations`](java_models.md#JavaField.annotations), [`annotations`](java_models.md#JavaMethod.annotations)

### `JavaClass`
- def: [`tree_sitter_analyzer/models/java_models.py:62`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L62)
- doc: Java class representation with comprehensive details
- signature: `class JavaClass:`
- members:
  - `to_summary_item(self)` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L80) — Return dictionary for summary item
  - `annotations` — [`L75`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L75)
  - `class_type` — [`L68`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L68)
  - `end_line` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L74)
  - `extends_class` — [`L71`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L71)
  - `file_path` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L78)
  - `full_qualified_name` — [`L66`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L66)
  - `implements_interfaces` — [`L72`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L72)
  - `is_nested` — [`L76`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L76)
  - `modifiers` — [`L69`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L69)
  - `name` — [`L65`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L65)
  - `package_name` — [`L67`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L67)
  - `parent_class` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L77)
  - `start_line` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L73)
  - `visibility` — [`L70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L70)
- uses (calls/refs, reference-scoped): [`JavaAnnotation`](java_models.md#JavaAnnotation)

### `JavaField`
- def: [`tree_sitter_analyzer/models/java_models.py:90`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L90)
- doc: Java field representation
- signature: `class JavaField:`
- members:
  - `to_summary_item(self)` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L104) — Return dictionary for summary item
  - `annotations` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L97)
  - `end_line` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L99)
  - `field_type` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L94)
  - `file_path` — [`L102`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L102)
  - `is_final` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L101)
  - `is_static` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L100)
  - `modifiers` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L95)
  - `name` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L93)
  - `start_line` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L98)
  - `visibility` — [`L96`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L96)
- uses (calls/refs, reference-scoped): [`JavaAnnotation`](java_models.md#JavaAnnotation)

### `JavaImport`
- def: [`tree_sitter_analyzer/models/java_models.py:114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L114)
- doc: Java import statement representation
- signature: `class JavaImport:`
- members:
  - `to_summary_item(self)` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L127) — 要約アイテムとして辞書を返す
  - `end_line` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L125)
  - `import_statement` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L120)
  - `imported_name` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L119)
  - `is_static` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L122)
  - `is_wildcard` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L123)
  - `line_number` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L121)
  - `module_name` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L118)
  - `name` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L117)
  - `start_line` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L124)

### `JavaMethod`
- def: [`tree_sitter_analyzer/models/java_models.py:33`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L33)
- doc: Java method representation with comprehensive details
- signature: `class JavaMethod:`
- members:
  - `to_summary_item(self)` — [`L52`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L52) — Return dictionary for summary item
  - `annotations` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L41)
  - `complexity_score` — [`L49`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L49)
  - `end_line` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L44)
  - `file_path` — [`L50`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L50)
  - `is_abstract` — [`L46`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L46)
  - `is_constructor` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L45)
  - `is_final` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L48)
  - `is_static` — [`L47`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L47)
  - `modifiers` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L39)
  - `name` — [`L36`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L36)
  - `parameters` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L38)
  - `return_type` — [`L37`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L37)
  - `start_line` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L43)
  - `throws` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L42)
  - `visibility` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L40)
- uses (calls/refs, reference-scoped): [`JavaAnnotation`](java_models.md#JavaAnnotation)

### `JavaPackage`
- def: [`tree_sitter_analyzer/models/java_models.py:137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L137)
- doc: Java package declaration representation
- signature: `class JavaPackage:`
- members:
  - `to_summary_item(self)` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L144) — Return dictionary for summary item
  - `end_line` — [`L142`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L142)
  - `name` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L140)
  - `start_line` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L141)
- used by: [`format_analysis_result`](../formatters/toon_formatter.md#ToonFormatter.format_analysis_result), [`package`](result.md#AnalysisResult.package)  (1 test-only)

## Module values
- `__all__` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/java_models.py#L153)

