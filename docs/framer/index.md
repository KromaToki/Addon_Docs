# Framer Manual

## Overview

Framer is a 3D View add-on for consistent viewport framing across object selections, edit-mode component selections, small or zero-area targets, and collection-filtered scenes.

The main operator is Smart Frame. It calculates target bounds from Blender scene data, object type filters, selection state, edit-mode geometry, and Framer exclusion flags, then frames the result in the active 3D View.

!!! warning "Important Source of Truth"
    Framer uses Blender scene state as the source of truth. Object and collection exclusion flags are stored on the objects and collections in the current file. The exclusion list in the sidebar is a session UI summary; use Refresh if it does not reflect the current file state after loading or external changes.

### Platform Support

Framer declares support for Blender 3.0 or newer.

## Core Features

- Smart Frame operator for object and component framing.
- Separate zero-area minimum distances for Object Mode and Edit modes.
- Density-aware framing for very small Mesh, Lattice, and Armature edit selections.
- High-poly edit mesh shortcut that avoids expensive full mesh scans when possible.
- Frameable object type mask for fallback framing when nothing is selected.
- Optional respect for Blender object selectability in Object Mode.
- Object and collection exclusion flags.
- Outliner and object context menu shortcuts for collection-focused framing.
- Optional viewport visualization for selection bounds, framing sphere, margin rectangle, and decoupled preview.
- Optional custom hotkey captured from add-on preferences.

## Quick Map

| Workflow | Management |
| :--- | :--- |
| - [Getting Started](./getting-started.md)<br>- [Smart Frame](./workflow/smart-frame.md) | - [Exclusions and Collections](./management/exclusions-and-collections.md)<br>- [Preferences](./management/preferences.md) |

