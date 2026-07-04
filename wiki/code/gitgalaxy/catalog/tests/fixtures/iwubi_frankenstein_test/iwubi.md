---
title: 'Module: tests/fixtures/iwubi_frankenstein_test/iwubi.py'
type: catalog
provenance: extracted
module: tests/fixtures/iwubi_frankenstein_test/iwubi.py
status: fresh
symbol_base: scip-python python gitgalaxy 0.0.0 `tests.fixtures.iwubi_frankenstein_test.iwubi`/
symbols:
  IbusWubiEngine._process_key_event: IbusWubiEngine#_process_key_event().
  KeyEvent.__str__: KeyEvent#__str__().
  IbusWubiEngine.update_candidates: IbusWubiEngine#update_candidates().
  KeyEvent.state: KeyEvent#state.
  IbusWubiEngine.preedit_string: IbusWubiEngine#preedit_string.
  IbusWubiEngine.lookup_table: IbusWubiEngine#lookup_table.
  logger: logger.
  IbusWubiEngine.commit_candidate: IbusWubiEngine#commit_candidate().
  IbusWubiEngine.commit_string: IbusWubiEngine#commit_string().
  IMApp.run: IMApp#run().
  IbusWubiEngine.do_process_key_event: IbusWubiEngine#do_process_key_event().
  n: n.
  numpad_keys: numpad_keys.
  IMApp.bus: IMApp#bus.
  IMApp.factory: IMApp#factory.
  IMApp.bus_disconnected_cb: IMApp#bus_disconnected_cb().
  IbusWubiEngine._update_lookup_table: IbusWubiEngine#_update_lookup_table().
  c: c.
  IbusWubiEngine.invalidate: IbusWubiEngine#invalidate().
  IbusWubiEngine.page_up: IbusWubiEngine#page_up().
  IbusWubiEngine.page_down: IbusWubiEngine#page_down().
  IbusWubiEngine.cursor_up: IbusWubiEngine#cursor_up().
  IbusWubiEngine.cursor_down: IbusWubiEngine#cursor_down().
  IWubi.find_characters: IWubi#find_characters().
  IbusWubiEngine.set_input_mode: IbusWubiEngine#set_input_mode().
  IbusWubiEngine._is_shift_hotkey: IbusWubiEngine#_is_shift_hotkey().
  IbusWubiEngine.do_reset: IbusWubiEngine#do_reset().
  launch_engine: launch_engine().
  main: main().
  IbusWubiEngine.set_lookup_table_cursor_pos_in_current_page: IbusWubiEngine#set_lookup_table_cursor_pos_in_current_page().
  conn: conn.
  KeyEvent.val: KeyEvent#val.
  IbusWubiEngine._prev_key: IbusWubiEngine#_prev_key.
  IbusWubiEngine.do_candidate_clicked: IbusWubiEngine#do_candidate_clicked().
  IbusWubiEngine._match_hotkey: IbusWubiEngine#_match_hotkey().
  IbusWubiEngine.do_focus_in: IbusWubiEngine#do_focus_in().
  IbusWubiEngine.do_focus_out: IbusWubiEngine#do_focus_out().
  punctuation_map: punctuation_map.
  IbusWubiEngine._last_wubi_list_len: IbusWubiEngine#_last_wubi_list_len.
  num_keys: num_keys.
  IbusWubiEngine._input_mode: IbusWubiEngine#_input_mode.
  KeyEvent.name: KeyEvent#name.
  KeyEvent.unicode: KeyEvent#unicode.
  KeyEvent.shift: KeyEvent#shift.
  KeyEvent.control: KeyEvent#control.
  KeyEvent.mod1: KeyEvent#mod1.
  KeyEvent.mod5: KeyEvent#mod5.
  KeyEvent.release: KeyEvent#release.
  IbusWubiEngine.iwubi: IbusWubiEngine#iwubi.
  __base_dir__: __base_dir__.
  IbusWubiEngine.candidates: IbusWubiEngine#candidates.
  IbusWubiEngine.is_invalidate: IbusWubiEngine#is_invalidate.
  print_help: print_help().
  KeyEvent.lock: KeyEvent#lock.
  KeyEvent.mod2: KeyEvent#mod2.
  KeyEvent.mod3: KeyEvent#mod3.
  KeyEvent.mod4: KeyEvent#mod4.
  KeyEvent.button1: KeyEvent#button1.
  KeyEvent.button2: KeyEvent#button2.
  KeyEvent.button3: KeyEvent#button3.
  KeyEvent.button4: KeyEvent#button4.
  KeyEvent.button5: KeyEvent#button5.
  KeyEvent.hyper: KeyEvent#hyper.
  KeyEvent.meta: KeyEvent#meta.
  KeyEvent.modifier: KeyEvent#modifier.
  IbusWubiEngine.__init__: IbusWubiEngine#__init__().
  IbusWubiEngine.do_property_activate: IbusWubiEngine#do_property_activate().
  IbusWubiEngine.do_page_up: IbusWubiEngine#do_page_up().
  IbusWubiEngine.do_page_down: IbusWubiEngine#do_page_down().
  IbusWubiEngine.do_cursor_up: IbusWubiEngine#do_cursor_up().
  IbusWubiEngine.do_cursor_down: IbusWubiEngine#do_cursor_down().
  IMApp.mainloop: IMApp#mainloop.
  gen_punctuation_map: gen_punctuation_map().
  KeyEvent: KeyEvent#
  KeyEvent.code: KeyEvent#code.
  IWubi: IWubi#
  IbusWubiEngine: IbusWubiEngine#
  IbusWubiEngine.prop_list: IbusWubiEngine#prop_list.
  IMApp: IMApp#
  KeyEvent.__init__: KeyEvent#__init__().
  IbusWubiEngine.__gtype_name__: IbusWubiEngine#__gtype_name__.
  IMApp.__init__: IMApp#__init__().
---
# Module: [`tests/fixtures/iwubi_frankenstein_test/iwubi.py`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py)

## Classes
### `IMApp`
- def: [`tests/fixtures/iwubi_frankenstein_test/iwubi.py:548`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L548)
- signature: `class IMApp:`
- members:
  - `bus_disconnected_cb(self, bus)` — [`L580`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L580)
  - `run(self)` — [`L571`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L571)
  - `bus` — [`L554`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L554)
  - `factory` — [`L556`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L556)
  - `mainloop` — [`L553`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L553)
- protocol/private: `__init__`[`L549`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L549)
- uses (calls/refs, reference-scoped): (4 test-only callers)
- used by: (1 test-only callers)

### `IWubi`
- def: [`tests/fixtures/iwubi_frankenstein_test/iwubi.py:133`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L133)
- signature: `class IWubi:`
- members:
  - `find_characters(self, preedit_string)` — [`L134`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L134)
- uses (calls/refs, reference-scoped): (2 test-only callers)
- used by: (2 test-only callers)

### `IbusWubiEngine`
- def: [`tests/fixtures/iwubi_frankenstein_test/iwubi.py:213`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L213)
- signature: `class IbusWubiEngine(IBus.Engine):`
- members:
  - `_is_shift_hotkey(self, key)` — [`L259`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L259) — Check whether “key” matches the Shift hotkey.
  - `_match_hotkey(self, key, keyval, state)` — [`L404`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L404) — Check whether “key” matches a “hotkey” specified by “keyval” and
  - `commit_candidate(self)` — [`L468`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L468)
  - `commit_string(self, text)` — [`L463`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L463)
  - `cursor_down(self)` — [`L457`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L457)
  - `cursor_up(self)` — [`L451`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L451)
  - `do_candidate_clicked(self, index, dummy_button, dummy_state)` — [`L245`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L245)
  - `do_cursor_down(self)` — [`L543`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L543)
  - `do_cursor_up(self)` — [`L540`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L540)
  - `do_focus_in(self)` — [`L515`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L515)
  - `do_focus_out(self)` — [`L519`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L519)
  - `do_page_down(self)` — [`L537`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L537)
  - `do_page_up(self)` — [`L534`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L534)
  - `do_process_key_event(self, keyval, keycode, state)` — [`L383`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L383) — do_process_key_event = gi.VFuncInfo(process_key_event)
  - `do_property_activate(self, prop_name)` — [`L531`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L531)
  - `do_reset(self)` — [`L523`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L523)
  - `invalidate(self)` — [`L429`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L429)
  - `page_down(self)` — [`L445`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L445)
  - `page_up(self)` — [`L437`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L437)
  - `set_input_mode(self, mode=1)` — [`L249`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L249) — :param mode: Whether to use WuBi mode.
  - `set_lookup_table_cursor_pos_in_current_page(self, index)` — [`L230`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L230) — Sets the cursor in the lookup table to index in the current page
  - `update_candidates(self)` — [`L471`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L471)
  - `candidates` — [`L218`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L218)
  - `is_invalidate` — [`L220`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L220)
  - `iwubi` — [`L219`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L219)
  - `lookup_table` — [`L223`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L223)
  - `preedit_string` — [`L221`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L221)
  - `prop_list` — [`L224`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L224)
- protocol/private: `__gtype_name__`[`L214`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L214), `__init__`[`L216`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L216), `_input_mode`[`L225`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L225), `_last_wubi_list_len`[`L227`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L227), `_prev_key`[`L226`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L226), `_process_key_event`[`L275`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L275), `_update_lookup_table`[`L509`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L509)
- uses (calls/refs, reference-scoped): (8 test-only callers)

### `KeyEvent`
- def: [`tests/fixtures/iwubi_frankenstein_test/iwubi.py:85`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L85)
- doc: Key event class used to make the checking of details of the key
- signature: `class KeyEvent:`
- members:
  - `button1` — [`L104`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L104)
  - `button2` — [`L105`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L105)
  - `button3` — [`L106`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L106)
  - `button4` — [`L107`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L107)
  - `button5` — [`L108`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L108)
  - `code` — [`L92`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L92)
  - `control` — [`L98`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L98)
  - `hyper` — [`L110`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L110)
  - `lock` — [`L97`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L97)
  - `meta` — [`L111`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L111)
  - `mod1` — [`L99`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L99)
  - `mod2` — [`L100`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L100)
  - `mod3` — [`L101`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L101)
  - `mod4` — [`L102`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L102)
  - `mod5` — [`L103`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L103)
  - `modifier` — [`L114`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L114)
  - `name` — [`L94`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L94)
  - `release` — [`L112`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L112)
  - `shift` — [`L96`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L96)
  - `state` — [`L93`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L93)
  - `unicode` — [`L95`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L95)
  - `val` — [`L91`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L91)
- protocol/private: `__init__`[`L90`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L90), `__str__`[`L116`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L116)
- used by: (3 test-only callers)

## Functions
- `gen_punctuation_map()` — [`L41`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L41)
- `launch_engine(exec_by_ibus)` — [`L588`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L588)
- `main()` — [`L600`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L600)
- `print_help(out, v=0)` — [`L593`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L593)

## Module values
- `__base_dir__` — [`L21`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L21)
- `c` — [`L38`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L38)
- `conn` — [`L37`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L37)
- `logger` — [`L19`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L19)
- `n` — [`L25`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L25)
- `num_keys` — [`L24`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L24)
- `numpad_keys` — [`L30`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L30)
- `punctuation_map` — [`L82`](../../../../../../../raw/code/gitgalaxy/tests/fixtures/iwubi_frankenstein_test/iwubi.py#L82)

