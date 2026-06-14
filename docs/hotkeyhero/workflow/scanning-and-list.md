# Scanning and List

HotkeyHero works from an explicit scan. The scan reads Blender keymaps, normalizes row data, computes source labels, detects conflicts, and populates the main hotkey list.

## Refresh

Use Refresh List or Refresh Scan whenever Blender's keymap may have changed.

Refresh is needed after:

- Installing or enabling an add-on that registers shortcuts.
- Editing hotkeys in Blender's built-in keymap editor.
- Creating a new shortcut from Blender's UI.
- Deleting or restoring keymap items outside HotkeyHero.
- Importing or restoring a HotkeyHero profile.

## List Rows

The main list is a unified view of Blender defaults, user overrides, user-created entries, add-on keymaps, tools, modal triggers, disabled rows, and deleted default placeholders.

Common row information includes:

- Name: the readable command or keymap item label.
- Hotkey: the key, modifiers, and event type.
- Operator: the Blender operator identifier.
- Context: the keymap or editor context.
- Source: whether the row is from Blender, User Mod, or Addon data.
- State icons: conflict, disabled, deleted, modal, tool, brush, import, or diagnostic state where available.

## Detail View

Use View Hotkey Detail to inspect a row in the multi-purpose detail window.

The detail view can show:

- Binding overview.
- Operator id.
- Source tag.
- Active state.
- Conflict state.
- Modal trigger state.
- Operator properties.
- Diagnostic metadata when support inspection is enabled.

Some add-on-owned rows are read-only by default. Full can unlock individual add-on hotkeys with the add-on override control, or globally through preferences.

## Deleted Defaults

HotkeyHero can show Blender-default hotkeys that were deleted from the current keymap. These rows represent a missing default binding, not a currently active shortcut.

Use Deleted filters and restore tools when you need to inspect or recover those defaults.

