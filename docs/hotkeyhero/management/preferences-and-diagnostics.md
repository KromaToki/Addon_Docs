# Preferences and Diagnostics

HotkeyHero preferences hold launch, onboarding, editing, visual, backup, and diagnostic controls.

## Launch

Launch HotkeyHero switches a Properties editor to the Scene tab so the HotkeyHero panel is visible.

If the editor state is unavailable, open the HotkeyHero panel from the Scene tab or use the preferences launch button again after a Properties editor exists.

## First-Run Prompt

On first run, HotkeyHero can prompt for setup before opening the main workspace.

Full prompts for an initial export so a portable snapshot exists before editing. Demo uses onboarding to confirm the panel layout while keeping Full-only actions locked.

## Editing Add-on Hotkeys

Allow Editing Addon Hotkeys controls whether add-on-owned hotkeys can be edited directly.

Keep this off unless you understand how the owning add-on manages its shortcuts. Some add-ons recreate keymaps when they load, update, or re-register.

## UI Options

Flat Hotkey Buttons changes the list button styling by rendering list buttons without embossed styling.

Other panel controls can show or hide stats, tools, utilities, and diagnostic information depending on build and preferences.

## Scanning and Diagnostics

Scanning and diagnostic preferences control how much HotkeyHero surfaces about source resolution, conflict state, modal resolution, and support metadata.

Use diagnostics when:

- A shortcut source looks wrong.
- A modal or tool relationship needs inspection.
- A conflict group does not match expectations.
- Support asks for audit data or resolver metadata.

## Performance Notes

HotkeyHero uses Blender's native UIList for the main hotkey table. Large keymaps can contain thousands of rows, so the add-on uses cache layers for display strings, filters, conflict state, and diagnostics.

If the list looks stale after external keymap edits, run Refresh rather than assuming the UI is live.

