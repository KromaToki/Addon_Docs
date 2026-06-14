# Getting Started

## Install and Open HotkeyHero

1. Install the HotkeyHero ZIP in Blender through Edit > Preferences > Add-ons.
2. Enable the add-on.
3. Open the add-on preferences.
4. Complete the first-run prompt.
5. Open a Properties editor, switch to the Scene tab, and use the HotkeyHero panel.

The preferences include Launch HotkeyHero, which switches a Properties editor to the Scene tab so the HotkeyHero panel is front and center.

## Full vs Demo

This manual describes the Full workflow.

- Demo includes scanning, searching, filtering, conflict review, and onboarding.
- Demo keeps Full controls visible, but editing, restore, prioritization, import application, and export are locked.
- Full unlocks the complete keymap management workflow.

## Recommended First Steps

If you are using HotkeyHero for the first time, do the following in order:

1. Run Refresh from the HotkeyHero panel.
2. Review the list columns and source icons in [Scanning and List](./workflow/scanning-and-list.md).
3. Use [Search and Filters](./workflow/search-and-filters.md) to narrow the list by context, source, key, or conflict state.
4. Open conflict details from [Conflicts](./workflow/conflicts.md) before changing any overlapping shortcut.
5. Export a full profile with [Import and Export](./management/import-export.md) before larger edits.
6. Use [Editing and Restore](./management/editing-and-restore.md) for targeted changes.

## Basic Workflow

1. Run Refresh so HotkeyHero reads the current Blender keymap.
2. Filter to the shortcut, source, context, or conflict group you want to review.
3. Open detail or conflict views when the list row alone is not enough.
4. Select rows for bulk actions.
5. Enable, disable, restore, prioritize, or edit selected rows as needed.
6. Export a profile before and after important changes.

## What HotkeyHero Does Not Do

HotkeyHero is built for reviewing, editing, restoring, filtering, exporting, and importing existing Blender keymap items. It does not replace every part of Blender's built-in keymap editor.

- HotkeyHero does not provide a general tool for creating brand-new hotkeys from scratch. Create new shortcuts through Blender's normal UI, then Refresh HotkeyHero to review or manage them. Import is the exception: when applying a HotkeyHero profile, Full can create a user keymap item from the imported profile if that binding does not already exist in the current Blender keymap.
- HotkeyHero does not perform Blender's direct keymap-delete action. It can disable hotkeys and restore selected rows back to Blender defaults.
- Restore Selected is a restore-to-default operation. If a selected row represents a user-created or user-modified keymap item, restoring it can make that custom entry disappear from a filtered HotkeyHero list because Blender no longer has that user override active.
- **HotkeyHero does not monitor keymaps live in the background. Refresh after changes made elsewhere.**
- HotkeyHero does not override add-ons that recreate their own shortcuts. If an add-on registers keymaps again later, it may recreate its shortcuts unless that add-on provides its own setting.
- HotkeyHero does not decide the correct shortcut layout. Conflict views show overlap and context so you can make the decision.
