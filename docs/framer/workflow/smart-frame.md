# Smart Frame

## How Smart Frame Chooses Targets

Smart Frame starts from the current Blender context.

In Object Mode:

- If objects are selected, Framer frames selected eligible objects.
- If nothing is selected, Framer frames eligible scene objects.
- Eligibility comes from the Frameable Object Types mask, visibility, exclusion flags, and optionally selectability.

In Edit and component modes:

- Framer reads selected component bounds when supported.
- If supported edit geometry has no selected components, Framer falls back to the editable object's available bounds where possible.
- Multi-object Mesh Edit Mode is supported.

## Supported Modes

Framer includes dedicated bounds handling for:

- Object Mode
- Mesh Edit Mode
- Curve and Surface Edit Mode
- Lattice Edit Mode
- Armature Edit Mode
- Pose Mode
- Grease Pencil Edit Mode
- Hair Curves Edit/Sculpt workflows where supported by Blender context
- Particle mode object framing

Sculpt mode is intentionally not handled as a component-selection workflow. Use Blender's normal object framing tools there.

## Zero-Area and Tiny Selections

Blender selections such as empties, single vertices, bone endpoints, or very small component selections can have little or no spatial size. Framer uses zero-area minimum distance settings so the view does not collapse onto the target.

There are separate controls for:

- Object Mode zero-area distance
- Edit mode zero-area distance

Density-aware framing can further adjust tiny Mesh, Lattice, and Armature edit selections by using nearby edge, lattice, or bone lengths when that information is available.

## High-Poly Mesh Behavior

For dense Mesh Edit Mode targets, Framer can use a high-poly optimization path when the vertex count exceeds the configured threshold.

When recent selection history is available, Framer can use it to avoid scanning the whole mesh. If the mesh is above the threshold and no usable history is available, Framer can fall back to Blender's native `view3d.view_selected` operation instead of forcing an expensive scan.

## Margin Behavior

Framer stores separate margin multipliers for:

- Perspective View
- Orthographic View
- Camera View

The active view perspective decides which multiplier is used when Smart Frame runs.

## Camera View Note

When framing in Camera View, Framer avoids framing the active camera as part of the target set when other targets are available. This prevents a feedback loop where the camera frames itself.

