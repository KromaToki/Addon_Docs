# Getting Started

## Install and Open Framer

1. Install the Framer ZIP or source folder through Blender's add-on workflow.
2. Enable the add-on in Edit > Preferences > Add-ons.
3. Open a 3D View.
4. Press `N` to open the sidebar.
5. Go to View > Framer.
6. Click Smart Frame.

Framer also adds a Framer item to the 3D View View menu.

## Basic Workflow

1. Select an object or edit-mode component you want to frame.
2. Run Smart Frame from View > Framer or from your assigned hotkey.
3. If nothing is selected in Object Mode, Framer frames all eligible scene objects based on the Frameable Object Types preference.
4. Use exclusions when specific objects or collections should be ignored by fallback framing.
5. Adjust margin, zero-area distance, density, and visualization settings from the Framer add-on preferences.

## Assign a Hotkey

Framer does not require a hotkey, but it can register one from its preferences.

1. Open Edit > Preferences > Add-ons > Framer.
2. Expand Custom Hotkey.
3. Click Set Hotkey.
4. Press the desired key combination.
5. Keep Enable Hotkey on.

The operator id is `view3d.framer`. You can also configure this operator from Blender's normal keymap editor.

## First Settings to Review

- Frameable Object Types: controls which object types are included when no object is selected.
- Respect Selectability: skips objects with selectability disabled during Object Mode framing.
- Zero Area Min Distance: controls how close Framer can move for point-sized targets.
- Margin Multiplier: sets breathing room separately for Perspective, Orthographic, and Camera View.
- Frame Visualizations: optional viewport guides for checking bounds and margin behavior.

## What Framer Does Not Do

Framer is a viewport framing tool. It does not replace Blender selection, visibility, or collection systems.

- Framer does not make hidden objects visible.
- Framer does not override object or collection exclusion flags unless you use reset/include commands.
- Framer does not provide special component framing for Sculpt mode.
- Framer does not animate view transitions; framing changes are immediate.

