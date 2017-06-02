# steam_shortcuts_reader

This library reads and writes the shortcuts.vdf file and similarly formatted files.

## Types

* List: `0x00` `string name` `list_contents` `EndOfList`
* String: `0x01` `string name` `string value`
* Bytes4: `0x02` `string name` `4 bytes`
* EndOfList: `0x08`

All strings end with `0x00`.

shortcuts.vdf ends with one "extra" `0x08`, that is not attached to a list.
