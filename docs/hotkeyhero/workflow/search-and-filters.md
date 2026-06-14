# Search and Filters

Search and filters narrow the current HotkeyHero list without changing Blender's keymap.

## Text Search

The text search field searches by operator id, readable name, and hotkey string.

Use the search method toggle to switch between:

- Contains search.
- Exact match search.

Clear Text Filter removes the text search.

## Context Filters

Use the keymap and context drop-downs to focus the list on a specific Blender keymap or editor context.

Modal keymap filtering is available when reviewing modal-trigger rows or modal keymap data.

## Source Filters

The source chips filter by row origin:

- Blender: default Blender keymap entries.
- User Mod: user overrides or user-created keymap changes.
- Addon: add-on-owned keymap entries.

Source labels are derived from scanner data and keymap metadata, not from display-name guessing.

## Type and State Filters

Use these chips when reviewing specialized keymap entries:

- Modals: modal trigger or modal map related rows.
- Tools: tool activation rows.
- Brushes: brush-related rows from scanner-populated keymap type data.
- Conflicts: rows with shortcut overlap.
- Disabled: inactive keymap entries.
- Deleted: default entries missing from the live keymap.

The conflict chip can include or exclude benign/default conflict groups depending on the conflict options shown in the chip.

## Key Filters

Use Capture Filter Key to filter by a pressed key combination.

Key filtering includes:

- Base key.
- Shift.
- Ctrl.
- Alt.
- OS key.
- Keyboard-as-modifier key.
- Event type: press, click, double-click, drag, or release.

The key search method can switch between exact and contains matching. Clear Key Filter removes the key-specific filter state.

## Import Preview Filters

When viewing an import preview, the filter chips change to import classifications:

- Ready.
- Conflict.
- Duplicate.
- Incompatible.

The import preview can also show or hide context and optionally include disabled imported rows.

