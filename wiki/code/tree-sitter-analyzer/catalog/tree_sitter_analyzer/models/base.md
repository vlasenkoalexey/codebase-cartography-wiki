---
title: 'Module: tree_sitter_analyzer/models/base.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/models/base.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.models.base`/
symbols:
  CodeElement.name: CodeElement#name.
  CodeElement.start_line: CodeElement#start_line.
  CodeElement.end_line: CodeElement#end_line.
  CodeElement.language: CodeElement#language.
  Function: Function#
  CodeElement.raw_text: CodeElement#raw_text.
  Class: Class#
  Variable: Variable#
  Import: Import#
  CodeElement: CodeElement#
  Function.complexity_score: Function#complexity_score.
  CodeElement.element_type: CodeElement#element_type.
  Function.parameters: Function#parameters.
  Function.return_type: Function#return_type.
  Class.class_type: Class#class_type.
  Function.visibility: Function#visibility.
  Function.receiver_type: Function#receiver_type.
  Package: Package#
  CodeElement.docstring: CodeElement#docstring.
  Variable.variable_type: Variable#variable_type.
  Function.is_method: Function#is_method.
  Expression: Expression#
  Class.interfaces: Class#interfaces.
  Function.is_async: Function#is_async.
  Class.superclass: Class#superclass.
  Class.full_qualified_name: Class#full_qualified_name.
  Variable.visibility: Variable#visibility.
  Variable.is_constant: Variable#is_constant.
  Class.modifiers: Class#modifiers.
  Function.modifiers: Function#modifiers.
  Import.module_name: Import#module_name.
  CodeElement.to_summary_item: CodeElement#to_summary_item().
  Class.visibility: Class#visibility.
  Function.is_static: Function#is_static.
  Function.is_constructor: Function#is_constructor.
  Expression.expression_kind: Expression#expression_kind.
  Function.receiver: Function#receiver.
  Function.is_abstract: Function#is_abstract.
  Variable.modifiers: Variable#modifiers.
  Expression.preview: Expression#preview.
  Variable.is_static: Variable#is_static.
  Function.is_arrow: Function#is_arrow.
  Function.framework_type: Function#framework_type.
  Class.package_name: Class#package_name.
  Class.is_exported: Class#is_exported.
  Comprehension: Comprehension#
  Function.is_public: Function#is_public.
  Function.is_generator: Function#is_generator.
  Class.parent_class: Class#parent_class.
  Import.module_path: Import#module_path.
  Import.imported_names: Import#imported_names.
  Function.annotations: Function#annotations.
  Class.annotations: Class#annotations.
  Variable.receiver_type: Variable#receiver_type.
  Import.import_statement: Import#import_statement.
  Comprehension.comprehension_type: Comprehension#comprehension_type.
  Lambda: Lambda#
  Function.is_private: Function#is_private.
  Import.alias: Import#alias.
  Comprehension.target_variable: Comprehension#target_variable.
  Function.decorators: Function#decorators.
  Comprehension.has_condition: Comprehension#has_condition.
  Class.framework_type: Class#framework_type.
  Class.is_abstract: Class#is_abstract.
  Comprehension.iterable_preview: Comprehension#iterable_preview.
  Class.methods: Class#methods.
  CodeElement.line_count: CodeElement#line_count().
  Variable.is_final: Variable#is_final.
  Import.is_wildcard: Import#is_wildcard.
  Function.parent_class: Function#parent_class.
  Function.is_property: Function#is_property.
  Variable.initializer: Variable#initializer.
  Import.is_static: Import#is_static.
  Lambda.parameters: Lambda#parameters.
  Lambda.body_preview: Lambda#body_preview.
  Class.implements_interfaces: Class#implements_interfaces.
  Class.decorators: Class#decorators.
  Variable.annotations: Variable#annotations.
  Variable.field_type: Variable#field_type.
  Variable.element_type: Variable#element_type.
  Import.element_type: Import#element_type.
  Package.element_type: Package#element_type.
  Function.element_type: Function#element_type.
  Function.throws: Function#throws.
  Function.is_final: Function#is_final.
  Function.is_classmethod: Function#is_classmethod.
  Function.is_staticmethod: Function#is_staticmethod.
  Class.element_type: Class#element_type.
  Class.is_nested: Class#is_nested.
  Class.is_react_component: Class#is_react_component.
  Class.is_dataclass: Class#is_dataclass.
  Class.is_exception: Class#is_exception.
  Variable.is_val: Variable#is_val.
  Variable.is_var: Variable#is_var.
  Variable.is_readonly: Variable#is_readonly.
  Variable.decorators: Variable#decorators.
  Lambda.element_type: Lambda#element_type.
  Comprehension.element_type: Comprehension#element_type.
  Expression.element_type: Expression#element_type.
  dataclass_with_slots: dataclass_with_slots().
  CodeElement.node_type: CodeElement#node_type.
  Function.is_suspend: Function#is_suspend.
  Class.extends_class: Class#extends_class.
  CodeElement.get: CodeElement#get().
  Function.parameter_defaults: Function#parameter_defaults.
  Function.is_constant: Function#is_constant.
  Function.decorator_start_line: Function#decorator_start_line.
  Class.decorator_start_line: Class#decorator_start_line.
  Import.imported_name: Import#imported_name.
  Import.line_number: Import#line_number.
  __all__: __all__.
---
# Module: [`tree_sitter_analyzer/models/base.py`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py)

## Classes
### `Class`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:114`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L114) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- doc: Generic class representation
- signature: `class Class(CodeElement):`
- members:
  - `annotations` — [`L127`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L127)
  - `class_type` — [`L117`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L117) — documented in [tree_sitter_analyzer-languages-scala_plugin](../../../concepts/tree_sitter_analyzer-languages-scala_plugin.md)
  - `decorator_start_line` — [`L144`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L144)
  - `decorators` — [`L146`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L146)
  - `element_type` — [`L124`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L124)
  - `extends_class` — [`L130`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L130)
  - `framework_type` — [`L136`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L136)
  - `full_qualified_name` — [`L118`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L118)
  - `implements_interfaces` — [`L131`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L131)
  - `interfaces` — [`L121`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L121) — documented in [tree_sitter_analyzer-languages-scala_plugin](../../../concepts/tree_sitter_analyzer-languages-scala_plugin.md)
  - `is_abstract` — [`L140`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L140)
  - `is_dataclass` — [`L139`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L139)
  - `is_exception` — [`L141`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L141)
  - `is_exported` — [`L137`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L137)
  - `is_nested` — [`L128`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L128)
  - `is_react_component` — [`L135`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L135)
  - `methods` — [`L125`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L125)
  - `modifiers` — [`L122`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L122)
  - `package_name` — [`L119`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L119)
  - `parent_class` — [`L129`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L129)
  - `superclass` — [`L120`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L120) — documented in [tree_sitter_analyzer-languages-scala_plugin](../../../concepts/tree_sitter_analyzer-languages-scala_plugin.md)
  - `visibility` — [`L123`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L123)
- uses (calls/refs, reference-scoped): [`Function`](base.md#Function), [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`extract_classes`](../plugins/base.md#ElementExtractor.extract_classes), [`TREE_SITTER_AVAILABLE`](../languages/typescript_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`extract_classes`](../languages/csharp_plugin.md#CSharpElementExtractor.extract_classes), [`build_class_element`](../languages/python_plugin/_element_builders.md#build_class_element), [`extract_class`](../languages/typescript_plugin/_class_helpers.md#extract_class), [`extract_cpp_class`](../languages/_cpp_element_helpers.md#extract_cpp_class), [`TREE_SITTER_AVAILABLE`](../languages/csharp_plugin.md#TREE_SITTER_AVAILABLE), [`_extract_class_like`](../languages/scala_plugin.md#ScalaElementExtractor._extract_class_like), [`_extract_enum_with_cases`](../languages/scala_plugin.md#ScalaElementExtractor._extract_enum_with_cases), [`extract_class`](../languages/javascript_plugin/_class_helpers.md#extract_class), [`extract_class_declaration`](../languages/csharp_helpers.md#extract_class_declaration), [`extract_interface`](../languages/typescript_plugin/_class_helpers.md#extract_interface), [`_build_java_class`](../languages/_java_element_helpers.md#_build_java_class), [`TREE_SITTER_AVAILABLE`](../languages/php_plugin.md#TREE_SITTER_AVAILABLE), [`_extract_extension`](../languages/scala_plugin.md#ScalaElementExtractor._extract_extension), [`_extract_given`](../languages/scala_plugin.md#ScalaElementExtractor._extract_given), [`_extract_type_alias`](../languages/scala_plugin.md#ScalaElementExtractor._extract_type_alias), [`_extract_type_definition`](../languages/_c_type_definition_helpers.md#_extract_type_definition), [`_extract_class_optimized`](../languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin._extract_class_optimized), [`extract_namespace`](../languages/typescript_plugin/_class_helpers.md#extract_namespace), [`extract_classes`](../languages/cpp_plugin.md#CppElementExtractor.extract_classes), [`_extract_class_optimized`](../languages/cpp_plugin.md#CppElementExtractor._extract_class_optimized), [`extract_kotlin_class_or_object`](../languages/kotlin_helpers.md#extract_kotlin_class_or_object), [`extract_php_class_element`](../languages/php_helpers.md#extract_php_class_element), [`extract_type_alias`](../languages/typescript_plugin/_class_helpers.md#extract_type_alias), [`TREE_SITTER_AVAILABLE`](../languages/javascript_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`_extract_class_element`](../languages/ruby_plugin.md#RubyElementExtractor._extract_class_element), [`extract_enum`](../languages/typescript_plugin/_class_helpers.md#extract_enum), [`_build_go_class`](../languages/_go_type_helpers.md#_build_go_class), [`_extract_detailed_class_info`](../languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin._extract_detailed_class_info), [`_extract_type_def`](../languages/rust_plugin.md#RustElementExtractor._extract_type_def), [`extract_classes`](../languages/c_plugin.md#CElementExtractor.extract_classes), [`extract_classes`](../languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.extract_classes), [`TREE_SITTER_AVAILABLE`](../languages/python_plugin/plugin.md#TREE_SITTER_AVAILABLE), [`extract_classes`](../languages/rust_plugin.md#RustElementExtractor.extract_classes), [`extract_classes`](../languages/java_plugin.md#JavaElementExtractor.extract_classes), [`_extract_class_optimized`](../languages/java_plugin.md#JavaElementExtractor._extract_class_optimized), [`TREE_SITTER_AVAILABLE`](../languages/ruby_plugin.md#TREE_SITTER_AVAILABLE)  (+70 more; 161 test-only)

### `CodeElement`  ·  implements/extends ABC
- def: [`tree_sitter_analyzer/models/base.py:35`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L35) — documented in [tree_sitter_analyzer-models-markup_models](../../../concepts/tree_sitter_analyzer-models-markup_models.md)
- doc: Base class for all code elements
- signature: `class CodeElement(ABC):`
- members:
  - `get(self, key: str, default: Any = None)` — [`L56`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L56) — Dict-style attribute access so formatters can use e.get('element_type')
  - `line_count(self)` — [`L48`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L48) — Number of source lines spanned: end_line - start_line + 1.
  - `to_summary_item(self)` — [`L61`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L61)
  - `docstring` — [`L43`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L43)
  - `element_type` — [`L44`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L44)
  - `end_line` — [`L40`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L40) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `language` — [`L42`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L42) — documented in [tree_sitter_analyzer-models-base](../../../concepts/tree_sitter_analyzer-models-base.md)
  - `name` — [`L38`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L38) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
  - `node_type` — [`L45`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L45)
  - `raw_text` — [`L41`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L41) — documented in [tree_sitter_analyzer-plugins-base](../../../concepts/tree_sitter_analyzer-plugins-base.md)
  - `start_line` — [`L39`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L39) — documented in [tree_sitter_analyzer-mcp-tools-base_tool](../../../concepts/tree_sitter_analyzer-mcp-tools-base_tool.md)
- uses (calls/refs, reference-scoped): [`Function`](base.md#Function), [`Class`](base.md#Class), [`Variable`](base.md#Variable), [`Import`](base.md#Import), [`MarkupElement`](markup_models.md#MarkupElement), [`MarkdownElement`](../languages/markdown_plugin/elements.md#MarkdownElement), [`SQLElement`](sql_models.md#SQLElement), [`StyleElement`](markup_models.md#StyleElement), [`Package`](base.md#Package), [`Expression`](base.md#Expression), [`YAMLElement`](../languages/yaml_helpers.md#YAMLElement), [`to_summary_item`](markup_models.md#YAMLElement.to_summary_item), [`JSONElement`](../languages/json_plugin.md#JSONElement), [`to_summary_item`](sql_models.md#SQLElement.to_summary_item), [`to_summary_item`](markup_models.md#MarkupElement.to_summary_item), [`to_summary_item`](markup_models.md#StyleElement.to_summary_item), [`Comprehension`](base.md#Comprehension), [`Lambda`](base.md#Lambda), [`YAMLElement`](markup_models.md#YAMLElement)  (2 test-only)
- used by: [`Function`](base.md#Function), [`Class`](base.md#Class), [`Variable`](base.md#Variable), [`elements`](result.md#AnalysisResult.elements), [`Import`](base.md#Import), [`MarkupElement`](markup_models.md#MarkupElement), [`MarkdownElement`](../languages/markdown_plugin/elements.md#MarkdownElement), [`TREE_SITTER_AVAILABLE`](../languages/typescript_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`build_function_element`](../languages/python_plugin/_element_builders.md#build_function_element), [`SQLElement`](sql_models.md#SQLElement), [`extract_classes`](../languages/csharp_plugin.md#CSharpElementExtractor.extract_classes), [`StyleElement`](markup_models.md#StyleElement), [`extract_cpp_function`](../languages/_cpp_element_helpers.md#extract_cpp_function), [`build_class_element`](../languages/python_plugin/_element_builders.md#build_class_element), [`extract_function_from_field_declaration`](../languages/_cpp_field_function_helpers.md#extract_function_from_field_declaration), [`extract_class`](../languages/typescript_plugin/_class_helpers.md#extract_class), [`extract_method`](../languages/typescript_plugin/_function_helpers.md#extract_method), [`extract_cpp_class`](../languages/_cpp_element_helpers.md#extract_cpp_class), [`extract_arrow_function`](../languages/typescript_plugin/_function_helpers.md#extract_arrow_function), [`extract_arrow_function`](../languages/javascript_plugin/_function_helpers.md#extract_arrow_function), [`_extract_function`](../languages/rust_plugin.md#RustElementExtractor._extract_function), [`extract_abstract_method_signature`](../languages/typescript_plugin/_function_helpers.md#extract_abstract_method_signature), [`extract_functions`](../languages/csharp_plugin.md#CSharpElementExtractor.extract_functions), [`fill_missing_sql_tables_from_regex`](../languages/sql_plugin/table_extractor.md#fill_missing_sql_tables_from_regex), [`extract_java_method`](../languages/_java_element_helpers.md#extract_java_method), [`extract_generator_function`](../languages/typescript_plugin/_function_helpers.md#extract_generator_function), [`extract_function`](../languages/typescript_plugin/_function_helpers.md#extract_function), [`extract_kotlin_function`](../languages/kotlin_helpers.md#extract_kotlin_function), [`build_detailed_function_element`](../languages/python_plugin/_element_builders.md#build_detailed_function_element), [`_extract_function_common`](../languages/scala_plugin.md#ScalaElementExtractor._extract_function_common), [`extract_prototype_method`](../languages/javascript_plugin/_function_helpers.md#extract_prototype_method), [`Package`](base.md#Package), [`_extract_class_like`](../languages/scala_plugin.md#ScalaElementExtractor._extract_class_like), [`analyze_file`](../languages/typescript_plugin/plugin.md#TypeScriptPlugin.analyze_file), [`extract_method_signature`](../languages/typescript_plugin/_function_helpers.md#extract_method_signature), [`extract_property`](../languages/typescript_plugin/_variable_helpers.md#extract_property), [`extract_method`](../languages/javascript_plugin/_function_helpers.md#extract_method), [`parse_variable_declarator`](../languages/javascript_plugin/_variable_helpers.md#parse_variable_declarator), [`parse_variable_declarator`](../languages/typescript_plugin/_variable_helpers.md#parse_variable_declarator), [`_analyze_html_fallback`](../languages/html_plugin.md#_analyze_html_fallback)  (+228 more; 879 test-only)

### `Comprehension`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:215`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L215)
- doc: List/set/dict comprehension or generator expression
- signature: `class Comprehension(CodeElement):`
- members:
  - `comprehension_type` — [`L228`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L228)
  - `element_type` — [`L232`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L232)
  - `has_condition` — [`L231`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L231)
  - `iterable_preview` — [`L230`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L230)
  - `target_variable` — [`L229`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L229)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement)  (9 test-only)

### `Expression`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:236`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L236)
- doc: Generic expression (conditional, subscript, list literals)
- signature: `class Expression(CodeElement):`
- members:
  - `element_type` — [`L250`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L250)
  - `expression_kind` — [`L248`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L248)
  - `preview` — [`L249`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L249)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`extract_expressions`](../languages/bash_plugin.md#BashElementExtractor.extract_expressions), [`TREE_SITTER_AVAILABLE`](../languages/bash_plugin.md#TREE_SITTER_AVAILABLE), [`_extract_control_flow`](../languages/bash_plugin.md#BashElementExtractor._extract_control_flow), [`_extract_string_pattern`](../languages/bash_plugin.md#BashElementExtractor._extract_string_pattern), [`_extract_redirect`](../languages/bash_plugin.md#BashElementExtractor._extract_redirect), [`_extract_subscript`](../languages/bash_plugin.md#BashElementExtractor._extract_subscript), [`_extract_annotation`](../languages/scala_plugin.md#ScalaElementExtractor._extract_annotation), [`_extract_array`](../languages/bash_plugin.md#BashElementExtractor._extract_array), [`_extract_comment`](../languages/bash_plugin.md#BashElementExtractor._extract_comment), [`_extract_comment`](../languages/scala_plugin.md#ScalaElementExtractor._extract_comment), [`_extract_list`](../languages/bash_plugin.md#BashElementExtractor._extract_list), [`_extract_process_substitution`](../languages/bash_plugin.md#BashElementExtractor._extract_process_substitution), [`_extract_subshell`](../languages/bash_plugin.md#BashElementExtractor._extract_subshell), [`extract_annotations`](../languages/scala_plugin.md#ScalaElementExtractor.extract_annotations), [`extract_comments`](../languages/scala_plugin.md#ScalaElementExtractor.extract_comments)  (11 test-only)

### `Function`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:70`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L70) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- doc: Generic function/method representation
- signature: `class Function(CodeElement):`
- members:
  - `annotations` — [`L91`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L91)
  - `complexity_score` — [`L93`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L93) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
  - `decorator_start_line` — [`L108`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L108)
  - `decorators` — [`L110`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L110)
  - `element_type` — [`L89`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L89)
  - `framework_type` — [`L101`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L101)
  - `is_abstract` — [`L94`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L94)
  - `is_arrow` — [`L98`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L98)
  - `is_async` — [`L79`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L79)
  - `is_classmethod` — [`L104`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L104)
  - `is_constant` — [`L83`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L83)
  - `is_constructor` — [`L88`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L88) — documented in [tree_sitter_analyzer-languages-scala_plugin](../../../concepts/tree_sitter_analyzer-languages-scala_plugin.md)
  - `is_final` — [`L95`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L95)
  - `is_generator` — [`L97`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L97)
  - `is_method` — [`L99`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L99)
  - `is_private` — [`L81`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L81)
  - `is_property` — [`L103`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L103)
  - `is_public` — [`L82`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L82)
  - `is_static` — [`L80`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L80)
  - `is_staticmethod` — [`L105`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L105)
  - `is_suspend` — [`L85`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L85)
  - `modifiers` — [`L78`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L78)
  - `parameter_defaults` — [`L74`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L74)
  - `parameters` — [`L73`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L73) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
  - `parent_class` — [`L100`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L100)
  - `receiver` — [`L86`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L86)
  - `receiver_type` — [`L87`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L87)
  - `return_type` — [`L77`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L77) — documented in [tree_sitter_analyzer-languages-scala_plugin](../../../concepts/tree_sitter_analyzer-languages-scala_plugin.md)
  - `throws` — [`L92`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L92)
  - `visibility` — [`L84`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L84) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`extract_functions`](../plugins/base.md#ElementExtractor.extract_functions), [`TREE_SITTER_AVAILABLE`](../languages/typescript_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`build_function_element`](../languages/python_plugin/_element_builders.md#build_function_element), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`extract_cpp_function`](../languages/_cpp_element_helpers.md#extract_cpp_function), [`extract_function_from_field_declaration`](../languages/_cpp_field_function_helpers.md#extract_function_from_field_declaration), [`extract_method`](../languages/typescript_plugin/_function_helpers.md#extract_method), [`extract_arrow_function`](../languages/typescript_plugin/_function_helpers.md#extract_arrow_function), [`extract_arrow_function`](../languages/javascript_plugin/_function_helpers.md#extract_arrow_function), [`TREE_SITTER_AVAILABLE`](../languages/csharp_plugin.md#TREE_SITTER_AVAILABLE), [`_extract_function`](../languages/rust_plugin.md#RustElementExtractor._extract_function), [`_extract_function_optimized`](../languages/python_plugin/_function_extractor_mixin.md#PythonFunctionExtractionMixin._extract_function_optimized), [`extract_abstract_method_signature`](../languages/typescript_plugin/_function_helpers.md#extract_abstract_method_signature), [`extract_functions`](../languages/csharp_plugin.md#CSharpElementExtractor.extract_functions), [`extract_java_method`](../languages/_java_element_helpers.md#extract_java_method), [`extract_generator_function`](../languages/typescript_plugin/_function_helpers.md#extract_generator_function), [`extract_function`](../languages/typescript_plugin/_function_helpers.md#extract_function), [`extract_kotlin_function`](../languages/kotlin_helpers.md#extract_kotlin_function), [`build_detailed_function_element`](../languages/python_plugin/_element_builders.md#build_detailed_function_element), [`_extract_function_common`](../languages/scala_plugin.md#ScalaElementExtractor._extract_function_common), [`extract_prototype_method`](../languages/javascript_plugin/_function_helpers.md#extract_prototype_method), [`extract_method_signature`](../languages/typescript_plugin/_function_helpers.md#extract_method_signature), [`extract_method`](../languages/javascript_plugin/_function_helpers.md#extract_method), [`extract_function`](../languages/javascript_plugin/_function_helpers.md#extract_function), [`extract_generator_function`](../languages/javascript_plugin/_function_helpers.md#extract_generator_function), [`_extract_method_element`](../languages/ruby_plugin.md#RubyElementExtractor._extract_method_element), [`extract_php_method_element`](../languages/php_helpers.md#extract_php_method_element), [`_extract_singleton_method_element`](../languages/ruby_plugin.md#RubyElementExtractor._extract_singleton_method_element), [`extract_c_function`](../languages/_c_function_helpers.md#extract_c_function), [`TREE_SITTER_AVAILABLE`](../languages/php_plugin.md#TREE_SITTER_AVAILABLE), [`_build_go_function`](../languages/_go_function_helpers.md#_build_go_function), [`extract_method_declaration`](../languages/csharp_helpers.md#extract_method_declaration), [`extract_php_function_element`](../languages/php_helpers.md#extract_php_function_element), [`_extract_function_signature`](../languages/rust_plugin.md#RustElementExtractor._extract_function_signature), [`extract_kotlin_primary_constructor`](../languages/kotlin_helpers.md#extract_kotlin_primary_constructor), [`extract_property_declaration`](../languages/csharp_helpers.md#extract_property_declaration), [`_extract_function_optimized`](../languages/cpp_plugin.md#CppElementExtractor._extract_function_optimized), [`extract_macro_function`](../languages/_c_macro_helpers.md#extract_macro_function), [`extract_functions`](../languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.extract_functions)  (+90 more; 312 test-only)

### `Import`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:175`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L175) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- doc: Generic import statement representation
- signature: `class Import(CodeElement):`
- members:
  - `alias` — [`L184`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L184)
  - `element_type` — [`L183`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L183)
  - `import_statement` — [`L187`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L187)
  - `imported_name` — [`L186`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L186)
  - `imported_names` — [`L180`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L180)
  - `is_static` — [`L182`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L182)
  - `is_wildcard` — [`L181`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L181)
  - `line_number` — [`L188`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L188)
  - `module_name` — [`L178`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L178)
  - `module_path` — [`L179`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L179)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`TREE_SITTER_AVAILABLE`](../languages/typescript_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`extract_imports`](../plugins/base.md#ElementExtractor.extract_imports), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`TREE_SITTER_AVAILABLE`](../languages/csharp_plugin.md#TREE_SITTER_AVAILABLE), [`TREE_SITTER_AVAILABLE`](../languages/php_plugin.md#TREE_SITTER_AVAILABLE), [`parse_simple_import`](../languages/python_plugin/_import_helpers.md#parse_simple_import), [`parse_from_import`](../languages/python_plugin/_import_helpers.md#parse_from_import), [`extract_import_info_simple`](../languages/typescript_plugin/_import_info_helpers.md#extract_import_info_simple), [`extract_imports`](../languages/python_plugin/_import_package_mixin.md#PythonImportPackageMixin.extract_imports), [`extract_import`](../languages/kotlin_helpers.md#extract_import), [`extract_using_directive`](../languages/csharp_helpers.md#extract_using_directive), [`TREE_SITTER_AVAILABLE`](../languages/python_plugin/plugin.md#TREE_SITTER_AVAILABLE), [`_extract_import_info`](../languages/python_plugin/_import_package_mixin.md#PythonImportPackageMixin._extract_import_info), [`_build_import_info`](../languages/typescript_plugin/import_extractor.md#_build_import_info), [`_extract_dynamic_import`](../languages/typescript_plugin/import_extractor.md#_extract_dynamic_import), [`TREE_SITTER_AVAILABLE`](../languages/ruby_plugin.md#TREE_SITTER_AVAILABLE), [`_extract_import_info_enhanced`](../languages/javascript_plugin/_import_export_mixin.md#JavaScriptImportExportMixin._extract_import_info_enhanced), [`_extract_import_info_simple`](../languages/javascript_plugin/_import_export_mixin.md#JavaScriptImportExportMixin._extract_import_info_simple), [`_build_import`](../languages/_java_import_helpers.md#_build_import), [`_traverse_for_imports`](../plugins/__init__.md#DefaultExtractor._traverse_for_imports), [`_query_imports`](../languages/python_plugin/_import_helpers.md#_query_imports), [`_extract_dynamic_import`](../languages/javascript_plugin/_import_export_mixin.md#JavaScriptImportExportMixin._extract_dynamic_import), [`_build_commonjs_require_import`](../languages/typescript_plugin/import_extractor.md#_build_commonjs_require_import), [`_build_go_import`](../languages/_go_import_helpers.md#_build_go_import), [`_commonjs_import_from_match`](../languages/javascript_plugin/_import_helpers.md#_commonjs_import_from_match), [`_extract_import`](../languages/rust_plugin.md#RustElementExtractor._extract_import), [`_extract_import`](../languages/scala_plugin.md#ScalaElementExtractor._extract_import), [`extract_imports_from_tree`](../languages/python_plugin/_import_helpers.md#extract_imports_from_tree), [`_include_import`](../languages/_c_include_helpers.md#_include_import), [`_include_from_line`](../languages/_cpp_import_namespace_helpers.md#_include_from_line), [`_build_use_clause_import`](../languages/php_helpers.md#_build_use_clause_import), [`_declaration_import`](../languages/_cpp_import_namespace_helpers.md#_declaration_import), [`extract_imports`](../languages/csharp_plugin.md#CSharpElementExtractor.extract_imports), [`extract_imports`](../languages/go_plugin.md#GoElementExtractor.extract_imports), [`extract_require_statement`](../languages/ruby_helpers.md#extract_require_statement), [`extract_include_info`](../languages/_c_include_helpers.md#extract_include_info), [`_append_schema_reference`](../languages/sql_plugin/schema_reference_extractor.md#_append_schema_reference), [`extract_imports`](../languages/scala_plugin.md#ScalaElementExtractor.extract_imports), [`_traverse_for_imports`](../plugins/_base_traverse_mixin.md#DefaultTraverseMixin._traverse_for_imports)  (+70 more; 38 test-only)

### `Lambda`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:199`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L199)
- doc: Lambda expression representation
- signature: `class Lambda(CodeElement):`
- members:
  - `body_preview` — [`L210`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L210)
  - `element_type` — [`L211`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L211)
  - `parameters` — [`L209`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L209)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement)  (6 test-only)

### `Package`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:192`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L192) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- doc: Generic package declaration representation
- signature: `class Package(CodeElement):`
- members:
  - `element_type` — [`L195`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L195)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`TREE_SITTER_AVAILABLE`](../languages/csharp_plugin.md#TREE_SITTER_AVAILABLE), [`extract_packages`](../languages/csharp_plugin.md#CSharpElementExtractor.extract_packages), [`extract_packages`](../languages/scala_plugin.md#ScalaElementExtractor.extract_packages), [`extract_packages`](../languages/kotlin_plugin.md#KotlinElementExtractor.extract_packages), [`extract_go_package`](../languages/_go_package_helpers.md#extract_go_package), [`_extract_namespace_info`](../languages/_cpp_import_namespace_helpers.md#_extract_namespace_info), [`_extract_package_element`](../languages/_java_import_helpers.md#_extract_package_element), [`_extract_mod_package`](../languages/rust_plugin.md#RustElementExtractor._extract_mod_package), [`extract_packages`](../languages/go_plugin.md#GoElementExtractor.extract_packages), [`extract_packages`](../languages/rust_plugin.md#RustElementExtractor.extract_packages), [`extract_packages`](../languages/java_plugin.md#JavaElementExtractor.extract_packages), [`current_module`](../languages/python_plugin/_import_package_mixin.md#PythonImportPackageMixin.current_module), [`_convert_one_cpp_element`](../formatters/_cpp_formatter_convert_mixin.md#CppTableFormatterConvertMixin._convert_one_cpp_element), [`extract_java_packages`](../languages/_java_import_helpers.md#extract_java_packages), [`_extract_package`](../languages/go_plugin.md#GoElementExtractor._extract_package), [`_extract_package_element`](../languages/java_plugin.md#JavaElementExtractor._extract_package_element), [`_valid_namespace_name`](../formatters/_cpp_formatter_convert_mixin.md#_valid_namespace_name), [`_namespace_entry`](../formatters/_cpp_formatter_convert_mixin.md#_namespace_entry), [`extract_packages`](../languages/python_plugin/_import_package_mixin.md#PythonImportPackageMixin.extract_packages)  (8 test-only)

### `Variable`  ·  implements/extends CodeElement
- def: [`tree_sitter_analyzer/models/base.py:150`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L150) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
- doc: Generic variable representation
- signature: `class Variable(CodeElement):`
- members:
  - `annotations` — [`L163`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L163)
  - `decorators` — [`L171`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L171)
  - `element_type` — [`L158`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L158)
  - `field_type` — [`L166`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L166)
  - `initializer` — [`L161`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L161)
  - `is_constant` — [`L155`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L155)
  - `is_final` — [`L164`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L164)
  - `is_readonly` — [`L165`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L165)
  - `is_static` — [`L156`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L156)
  - `is_val` — [`L159`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L159)
  - `is_var` — [`L160`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L160)
  - `modifiers` — [`L154`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L154)
  - `receiver_type` — [`L169`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L169)
  - `variable_type` — [`L153`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L153) — documented in [tree_sitter_analyzer-languages-csharp_plugin](../../../concepts/tree_sitter_analyzer-languages-csharp_plugin.md)
  - `visibility` — [`L157`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L157)
- uses (calls/refs, reference-scoped): [`CodeElement`](base.md#CodeElement)
- used by: [`CodeElement`](base.md#CodeElement), [`TREE_SITTER_AVAILABLE`](../languages/typescript_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`extract_variables`](../plugins/base.md#ElementExtractor.extract_variables), [`TREE_SITTER_AVAILABLE`](../languages/sql_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`TREE_SITTER_AVAILABLE`](../languages/csharp_plugin.md#TREE_SITTER_AVAILABLE), [`extract_property`](../languages/typescript_plugin/_variable_helpers.md#extract_property), [`parse_variable_declarator`](../languages/javascript_plugin/_variable_helpers.md#parse_variable_declarator), [`parse_variable_declarator`](../languages/typescript_plugin/_variable_helpers.md#parse_variable_declarator), [`TREE_SITTER_AVAILABLE`](../languages/php_plugin.md#TREE_SITTER_AVAILABLE), [`extract_field_declaration`](../languages/csharp_helpers.md#extract_field_declaration), [`_extract_variable`](../languages/scala_plugin.md#ScalaElementExtractor._extract_variable), [`extract_event_declaration`](../languages/csharp_helpers.md#extract_event_declaration), [`extract_kotlin_property`](../languages/kotlin_helpers.md#extract_kotlin_property), [`_build_variables`](../languages/_cpp_variable_helpers.md#_build_variables), [`TREE_SITTER_AVAILABLE`](../languages/javascript_plugin/extractor.md#TREE_SITTER_AVAILABLE), [`_build_java_field`](../languages/_java_element_helpers.md#_build_java_field), [`_extract_scss_variables`](../languages/css_plugin.md#_extract_scss_variables), [`_extract_field_definition_optimized`](../languages/javascript_plugin/extractor.md#JavaScriptElementExtractor._extract_field_definition_optimized), [`extract_variables`](../languages/python_plugin/_class_extractor_mixin.md#PythonClassExtractionMixin.extract_variables), [`TREE_SITTER_AVAILABLE`](../languages/bash_plugin.md#TREE_SITTER_AVAILABLE), [`_extract_field`](../languages/rust_plugin.md#RustElementExtractor._extract_field), [`_extract_property_optimized`](../languages/javascript_plugin/extractor.md#JavaScriptElementExtractor._extract_property_optimized), [`TREE_SITTER_AVAILABLE`](../languages/python_plugin/plugin.md#TREE_SITTER_AVAILABLE), [`extract_variables`](../languages/typescript_plugin/extractor.md#TypeScriptElementExtractor.extract_variables), [`_build_module_constant`](../languages/python_plugin/_element_builders.md#_build_module_constant), [`_build_php_property_variable`](../languages/php_helpers.md#_build_php_property_variable), [`_extract_assignment_variable`](../languages/ruby_plugin.md#RubyElementExtractor._extract_assignment_variable), [`_extract_enum_variants`](../languages/rust_plugin.md#RustElementExtractor._extract_enum_variants), [`_extract_one_field`](../languages/_go_variable_helpers.md#_extract_one_field), [`_build_php_constant_variable`](../languages/php_helpers.md#_build_php_constant_variable), [`extract_variables`](../languages/go_plugin.md#GoElementExtractor.extract_variables), [`TREE_SITTER_AVAILABLE`](../languages/ruby_plugin.md#TREE_SITTER_AVAILABLE), [`extract_macro_definition`](../languages/c_helpers.md#extract_macro_definition), [`extract_property_signature`](../languages/typescript_plugin/_variable_helpers.md#extract_property_signature), [`extract_variables`](../languages/csharp_plugin.md#CSharpElementExtractor.extract_variables), [`_variable`](../languages/_c_declaration_helpers.md#_variable), [`extract_class_attribute_info`](../languages/python_plugin/_element_builders.md#extract_class_attribute_info), [`_traverse_for_variables`](../plugins/__init__.md#DefaultExtractor._traverse_for_variables), [`extract_variables`](../languages/rust_plugin.md#RustElementExtractor.extract_variables), [`_build_go_variable`](../languages/_go_variable_helpers.md#_build_go_variable)  (+77 more; 76 test-only)

## Functions
- `dataclass_with_slots(*args: Any, **kwargs: Any)` — [`L25`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L25)

## Module values
- `__all__` — [`L253`](../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/models/base.py#L253)

