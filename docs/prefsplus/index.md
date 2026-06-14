# PrefsPlus Manual

## Overview

PrefsPlus adds quick-access buttons to Blender's Preferences header so frequently used add-on preferences can be filtered and opened without repeatedly searching the Add-ons list.

Pinned buttons target installed add-ons by module id. Each pin can have a custom label, optional text display, a Blender icon, and a header order.

!!! warning "Preferences UI Patch"
    PrefsPlus modifies Blender Preferences header drawing while the add-on is enabled. The compact filtered add-on view also temporarily hides Blender's native Add-ons panel when a pinned add-on is active. Disable the compact view if Blender's Preferences UI behaves unexpectedly.

### Platform Support

PrefsPlus targets Blender 4.5 or newer.

Blender 5.0 or newer supports the optional Preferences section dropdown in the header. Blender 4.5 uses pinned add-on header buttons only.

## Core Features

- Pin installed add-ons to the Preferences header.
- Click a pin to switch to Preferences > Add-ons and filter to that add-on.
- Click the active pin again to clear the filter.
- Rename pin labels.
- Use icon-only pins or show text labels.
- Choose a Blender UI icon for each pin.
- Move pins left or right.
- Remove pins.
- Save and load PrefsPlus JSON profiles.
- Optionally keep pins visible outside the Add-ons section.
- Optionally use a compact filtered add-on view.

## Quick Map

| Workflow | Management |
| :--- | :--- |
| - [Getting Started](./getting-started.md)<br>- [Header Pins](./workflow/header-pins.md) | - [Profiles](./management/profiles.md)<br>- [Preferences](./management/preferences.md) |

