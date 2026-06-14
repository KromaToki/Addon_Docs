# Header Pins

## Add a Pin

Open Edit > Preferences > Add-ons > PrefsPlus, expand PrefsPlus Configuration, and click Add To Header.

The search popup lists installed add-ons using Blender's add-on metadata. Selecting an add-on adds it to the start of the header pin list.

If the add-on is already pinned, PrefsPlus leaves the existing pin in place.

## Use a Pin

Clicking a pin:

- Switches Preferences to the Add-ons section.
- Sets the add-on filter to All.
- Clears the enabled-only filter.
- Searches for the add-on display name.
- Expands the matching add-on entry when the compact filtered view is off.

Clicking the active pin again clears the add-on search filter.

## Rename a Pin

Each pinned row has a Label field. This value controls the text used when a pin is showing text.

If the pin has no icon, the label is shown automatically. If the pin has an icon, use the text visibility toggle to choose whether the label appears next to the icon.

## Choose an Icon

Click the icon button in a pinned row to open the icon picker.

The picker supports:

- Search
- All icons
- Modifiers
- Outliner
- Tools and Brushes
- UI and Views
- Others
- Page navigation when many icons match
- Copying the currently assigned icon name

Only valid Blender icon identifiers are stored. Invalid or empty icon names resolve to `NONE`.

## Reorder or Remove Pins

Use the left and right arrow buttons to move a pin in the header order.

Use the trash button to remove a pin.

PrefsPlus normalizes duplicate or invalid header order values during registration and pin edits.

