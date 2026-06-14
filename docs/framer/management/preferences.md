# Preferences

Open Edit > Preferences > Add-ons > Framer.

## Frameable Object Types

Frameable Object Types controls the object type mask used by Object Mode fallback framing when nothing is selected.

The default mask includes:

- Mesh
- Armature
- Empty

Framer also integrates this mask into the 3D View object type visibility panel by adding a framing toggle next to each supported object type.

## Frame Settings

Respect Selectability skips objects with Blender selectability disabled during Object Mode framing.

Zero Area Min Distance controls minimum framing distance for targets that have no meaningful size:

- Object: used in Object Mode.
- Edit: used in Edit and component modes.

Density controls tiny component framing:

- Use Density enables density-aware framing.
- Respect Zero Area Min Distance prevents density framing from moving closer than the zero-area minimum.
- Mesh, Lattice scale affects mesh and lattice component density distance.
- Armature scale affects armature edit density distance.
- Min Distance sets the minimum distance while density framing is active.

High-Poly Optimization controls dense Mesh Edit Mode handling:

- Enable turns on the optimized path.
- Threshold sets the vertex count above which a mesh is treated as high-poly.

Margin Multiplier controls view breathing room:

- Persp for Perspective View.
- Ortho for Orthographic View.
- Camera for Camera View.

## HUD Settings

HUD Settings controls the notification overlay used for exclusion and reset feedback.

- Font Size
- Duration
- Horizontal and Vertical position
- Warning Text Color
- Success Text Color
- Optional background color and opacity

Positions are stored as pixel offsets.

## Frame Visualizations

Frame Visualizations draws optional guides in the viewport when Smart Frame runs.

Core controls:

- Enable Visualization
- Decouple Visualizations
- Face Camera

Decouple Visualizations previews the framing guides without moving the view. When decoupling is turned off again, Framer attempts to run Smart Frame so the view matches the preview.

Bounds controls:

- Framing sphere outline
- Bounds rectangle outline
- Outline colors
- Outline widths

Margin controls:

- Margin rectangle outline
- Fill when bounds are smaller than margin
- Fill when bounds are larger than margin
- Fill and outline colors
- Outline width

Display controls:

- Show Margin Multiplier
- Show Decouple State
- Pixel positions for both display labels

## Custom Hotkey

Custom Hotkey captures and registers a keymap item for `view3d.framer`.

Controls:

- Enable Hotkey
- Set Hotkey
- Clear Hotkey
- Ctrl, Shift, Alt, and OS modifier toggles

If no key is stored, Enable Hotkey is inactive. Press Esc while capture is waiting to cancel without changing the stored hotkey.

