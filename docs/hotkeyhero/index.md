# HotkeyHero Manual

## Overview

HotkeyHero is a Blender keymap workspace for reviewing shortcuts, filtering large keymaps, identifying conflicts, and moving keymap changes between Blender setups through explicit JSON export and import.

HotkeyHero reads Blender's current keymap into a searchable table. From there you can inspect source, context, operator data, conflict state, and selection state before choosing whether to edit, disable, restore, import, or export keymap entries.

!!! warning "Important Source of Truth"
    Blender's keymap remains the active source of truth. HotkeyHero is not a live background monitor. After creating, deleting, installing, or changing hotkeys outside HotkeyHero, run Refresh so the list reflects the current Blender keymap.

### Platform Support

HotkeyHero targets Blender 4.5 or newer.

## HotkeyHero Versions

HotkeyHero has two release variants:

- HotkeyHero Full
- HotkeyHero Demo

| Feature | HotkeyHero Full | HotkeyHero Demo |
| :--- | :---: | :---: |
| Keymap scanning and refresh | yes | yes |
| Search and filters | yes | yes |
| Conflict drill-in views | yes | yes |
| Export reviewed profile data | yes | locked |
| Import and apply profile data | yes | locked |
| Edit, enable, disable, and restore hotkeys | yes | locked |
| Add-on prioritization tools | yes | locked |
| Legacy Vault backup restore | yes | limited onboarding only |

### Full Version

- Reviews Blender defaults, user-modified hotkeys, user-created hotkeys, and add-on hotkeys in one list.
- Filters by source, context, key, modifiers, event type, disabled state, deleted defaults, modal maps, tools, and brushes.
- Shows conflict drill-in views for overlapping shortcuts.
- Supports selected-row and bulk enable, disable, restore, prioritization, and hotkey editing.
- Exports and imports portable JSON profiles for backup, review, recovery, and transfer.
- Includes legacy Vault backup restore for older local snapshots.

### Demo Version

- Includes the scanner, search, filters, conflict views, and onboarding flow.
- Keeps Full controls visible so the workflow can be inspected before upgrading.
- Locks editing, restore, prioritization, export, and import application.

## Quick Map

| Workflow | Management |
| :--- | :--- |
| - [Getting Started](./getting-started.md)<br>- [Scanning and List](./workflow/scanning-and-list.md)<br>- [Search and Filters](./workflow/search-and-filters.md)<br>- [Conflicts](./workflow/conflicts.md) | - [Editing and Restore](./management/editing-and-restore.md)<br>- [Import and Export](./management/import-export.md)<br>- [Preferences and Diagnostics](./management/preferences-and-diagnostics.md) |

