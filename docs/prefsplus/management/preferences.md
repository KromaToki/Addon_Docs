# Preferences

Open Edit > Preferences > Add-ons > PrefsPlus.

## Compact Filtered Add-on View

Compact Filtered Add-on View is optional.

When enabled, clicking a pinned add-on shows that add-on in a simplified PrefsPlus panel and temporarily hides Blender's native Add-ons list while the filter is active.

Use Clear Add-on Filter from the compact panel header, or click the active header pin again, to return to the normal Add-ons list.

Disable this option if Preferences layout or add-on display behavior becomes unexpected.

## PrefsPlus Configuration

PrefsPlus Configuration contains the main layout controls.

In Blender 5.0 or newer:

- Show Section Dropdown Menu displays Blender's Preferences section selector in the header when the sidebar is closed.
- Minimal Dropdown shows that section selector as an icon-only control.

In Blender 4.5, the section dropdown controls are not available.

## Header Button Controls

Persistent Header Buttons keeps pinned PrefsPlus buttons visible even when Preferences sections other than Add-ons are active.

Spacing controls the amount of separator space between header buttons. A value of `0.0` removes the extra spacing.

Save Profile and Load Profile manage PrefsPlus JSON profiles.

Add To Header opens the installed add-on search popup.

## Pin Row Controls

Each pinned add-on row includes:

- Display name from Blender add-on metadata.
- Label field for a custom short label.
- Text visibility toggle.
- Icon picker.
- Move left.
- Move right.
- Remove.

The final Preferences header button always links back to PrefsPlus itself.

## Operators

PrefsPlus registers these user-facing operators:

- `prefsplus.add_pin_search`
- `prefsplus.jump_to_addon`
- `prefsplus.clear_filter`
- `prefsplus.icon_viewer`
- `prefsplus.export_profile`
- `prefsplus.import_profile`
- `prefsplus.move_pin`
- `prefsplus.remove_pin`

