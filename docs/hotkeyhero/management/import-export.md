# Import and Export

HotkeyHero's main save, recovery, and transfer path is explicit JSON export and import.

## Save and Transfer Protocol

1. Refresh the HotkeyHero list so it reflects the current Blender keymap.
2. Use Export Profile with a full snapshot before larger edits.
3. Use filters or selection when you intentionally want a visible-row or selected-row export.
4. Keep exported JSON files with the project, Blender version notes, or machine setup they belong to.
5. On another Blender install, use Import to preview the file before applying changes.
6. Apply only after reviewing the import preview and any conflict warnings.

## Export Profile

Export Profile writes a portable HotkeyHero JSON profile.

Use export for:

- Full keymap snapshots before edits.
- Visible filtered subsets for review.
- Selected rows for targeted transfer.
- Before and after snapshots around a cleanup pass.

## Import

Import reads a HotkeyHero JSON profile and builds an import preview before applying changes.

Preview classifications include:

- Ready: can be applied.
- Conflict: import row overlaps an existing shortcut.
- Duplicate: the binding already exists.
- Incompatible: the row cannot be applied in the current Blender setup.

Use Import Selected or Apply Import Preview only after reviewing the preview rows.

## Disabled Imported Rows

The import preview can include disabled imported items. When enabled, applying those rows can disable matching keys in the target setup.

Leave disabled-row import off unless you intentionally want the imported profile to carry disabled states into the current Blender keymap.

## Support Audit

Export KMI Audit writes parity-relevant raw Blender keymap-item data for selected or visible HotkeyHero items.

Use this for support and diagnostics, not as the normal backup format.

