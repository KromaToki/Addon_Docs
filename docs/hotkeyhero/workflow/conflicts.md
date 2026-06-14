# Conflicts

HotkeyHero marks conflicts when active keymap items share the same actionable key signature.

Conflicts are not always mistakes. Blender can intentionally reuse shortcuts across contexts, modes, tools, modal maps, or disabled alternatives. Use the conflict view to decide whether a shortcut overlap matters in your workflow.

## Show Conflicts

Use Show Conflicts to switch to the unresolved conflict view.

The Conflicts filter shows rows that share a key signature with another row. The benign/default conflict option controls whether default-only or accepted conflict groups are included.

## View Conflict

Use View Conflict on a row to show all items with the same key signature.

The conflict view helps compare:

- Display name.
- Hotkey.
- Operator id.
- Keymap context.
- Source.
- Active or disabled state.
- Add-on ownership.

Return to the main UI when you are finished reviewing the group.

## Prioritize Addon

Full includes two prioritization workflows:

- Prioritize Addon from a conflict view disables non-add-on bindings in that conflict and keeps an add-on binding active.
- Prioritize Addons performs a broader add-on prioritization pass by disabling conflicting non-add-on shortcuts.

Use these actions only after reviewing the conflict group. Export a profile first when changing many shortcuts at once.

## Accepted or Benign Conflicts

HotkeyHero distinguishes unresolved conflicts from default-only or accepted conflict groups. A default-only overlap may be intentional Blender behavior.

If a conflict is not harmful in your workflow, leave it alone. HotkeyHero is an inspection tool, not an automatic shortcut policy engine.

