# Editing and Restore

Full can edit, enable, disable, and restore existing Blender keymap items. Demo shows these controls but keeps them locked.

## Selection

Use row selection for bulk operations.

Selection commands include:

- All: select all visible hotkeys.
- None: deselect all hotkeys.
- Invert: invert the current visible selection.

Filters affect which rows are visible, so confirm the current filter state before using bulk actions.

## Enable and Disable

Use Enable or Disable to change the active state of selected hotkeys.

Use the row Toggle Hotkey control when you want to enable or disable a single item without changing other selections.

Disabling a hotkey keeps the keymap item available for review and possible re-enabling. It is not the same as deleting a keymap item from Blender's keymap editor.

When a keymap edit, restore, prioritization, or similar mutation succeeds, HotkeyHero saves Blender user preferences so the keymap change persists. Blender exposes this as a full user-preferences save, not a keymap-only save, so review unrelated preference changes before applying large keymap operations.

## Edit Hotkey

Use Edit Hotkey or Set Hotkey controls to capture a new key for existing rows.

Set Hotkey supports:

- Base key capture.
- Shift, Ctrl, Alt, and OS modifiers.
- Keyboard-as-modifier capture.
- Press, click, double-click, drag, and release event types.
- Apply to selected rows.

Some add-on hotkeys are locked by default because add-ons may recreate their own keymaps. Full can allow editing add-on hotkeys globally in preferences or per row with Toggle Addon Hotkey Override.

## Restore Selected

Restore Selected restores selected deleted hotkeys and user overrides to Blender defaults.

This is a restore-to-default operation. If a row represents a user-created or user-modified keymap item, restoring it can remove the active user override from Blender, which can make the row disappear from HotkeyHero after refresh.

## Undelete Defaults

Use Undelete Selected, Undelete Hotkey, or Undelete All to restore Blender-default hotkeys that were deleted from the keymap.

These actions apply only to deleted default rows.

## Deleted-Default Normalization

HotkeyHero treats Blender-default keys as addressable keymap items. When Refresh finds a new set of deleted defaults, it presents an explicit normalization choice instead of modifying the keymap during the scan.

The default **Safe Active** policy:

- Restores non-conflicting defaults active.
- Restores defaults that would conflict as disabled items.

The prompt also supports **All Disabled**, **All Active**, individual review, or leaving the current deleted set unchanged. Choosing Leave Unchanged acknowledges only that exact set; newly deleted defaults cause the prompt to appear again.

## Restore Blender Defaults

Restore Blender Defaults restores Blender keymaps to factory defaults while preserving add-on-created keymaps.

This is a broad operation. Export a profile first, then refresh after the restore completes.

