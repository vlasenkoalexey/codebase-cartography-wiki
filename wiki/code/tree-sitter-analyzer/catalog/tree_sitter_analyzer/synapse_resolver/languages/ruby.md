---
title: 'Module: tree_sitter_analyzer/synapse_resolver/languages/ruby.py'
type: catalog
provenance: extracted
module: tree_sitter_analyzer/synapse_resolver/languages/ruby.py
status: fresh
symbol_base: scip-python python tree-sitter-analyzer 0.0.0 `tree_sitter_analyzer.synapse_resolver.languages.ruby`/
symbols:
  resolve_ruby_callee: resolve_ruby_callee().
  RubyResolverContext: RubyResolverContext#
  build_ruby_context: build_ruby_context().
  _ruby_project_owns: _ruby_project_owns().
  _lookup_in_file: _lookup_in_file().
  _RUBY_LANG: _RUBY_LANG.
  _owner_kind: _owner_kind().
  RubyResolverContext.__init__: RubyResolverContext#__init__().
  _BARE_CALLABLE_KINDS._BARE_CALLABLE_KINDS: _BARE_CALLABLE_KINDS._BARE_CALLABLE_KINDS.
  _split_receiver: _split_receiver().
  RubyResolverContext.__slots__: RubyResolverContext#__slots__.
---
# Module: [`tree_sitter_analyzer/synapse_resolver/languages/ruby.py`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py)

## Classes
### `RubyResolverContext`
- def: [`tree_sitter_analyzer/synapse_resolver/languages/ruby.py:65`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L65)
- doc: Per-index Ruby resolution maps (built once per pass).
- signature: `class RubyResolverContext:`
- protocol/private: `__init__`[`L79`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L79), `__slots__`[`L72`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L72)
- used by: [`resolve_ruby_callee`](ruby.md#resolve_ruby_callee), [`build_ruby_context`](ruby.md#build_ruby_context), [`_ruby_project_owns`](ruby.md#_ruby_project_owns), [`_lookup_in_file`](ruby.md#_lookup_in_file), [`_owner_kind`](ruby.md#_owner_kind)

## Functions
- `_lookup_in_file(ctx: RubyResolverContext, file_path: str, simple: str)` — [`L128`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L128) — Symbol id of a same-file BARE-CALLABLE named ``simple`` in ``file_path``.
- `_owner_kind(ctx: RubyResolverContext, owner_file: str, sym_id: int)` — [`L147`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L147) — Kind (``function``/``method``/``class``) of ``sym_id`` in ``owner_file``.
- `_ruby_project_owns(ctx: RubyResolverContext, simple: str)` — [`L160`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L160) — True when a RUBY project symbol is named ``simple``.
- `_split_receiver(full_name: str, bare_name: str)` — [`L119`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L119) — Return ``(receiver, simple_name)`` from a Ruby call's full name.
- `build_ruby_context(*, imports_by_file: dict[str, Any], file_languages: dict[str, str], file_symbols: dict[str, Any], global_name_table: dict[str, Any], file_class_methods: Any, **_ignored: Any)` — [`L93`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L93) — Build the Ruby context, or ``None`` when no ``.rb`` file is indexed.
- `resolve_ruby_callee(bare_name: str, full_name: str, caller_file: str, lang_ctx: RubyResolverContext)` — [`L175`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L175) — Resolve one Ruby call edge.

## Module values
- `_BARE_CALLABLE_KINDS` — [`L62`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L62)
- `_RUBY_LANG` — [`L52`](../../../../../../../raw/code/tree-sitter-analyzer/tree_sitter_analyzer/synapse_resolver/languages/ruby.py#L52)

