# General Behavior
<img src="../../assets/GenBehavior.png" alt="Key Bindings" class="sticky-aside-img">

General Behavior defines how BrushHud interprets drag motion, how strength is scaled, and how the optional demo workflow is surfaced.

## Axis Controls

Axis Controls determine how drag movement is mapped to BrushHud actions.

### Axis Deadzone (px)

Axis Deadzone delays directional commitment until your drag has moved far enough to count as intentional input.

- Increase it if tiny hand movement causes accidental changes.
- Reduce it if the HUD feels slow to react.

### Follow Cursor Movement (Size Only)

Follow Cursor Movement lets the HUD reposition with your cursor while adjusting size.

- Enable it if you want the size display to track the brush more closely.
- Leave it off if you prefer a steadier HUD anchor while dragging.

### Swap Size/Strength Axes

Swap Size/Strength Axes reverses which drag direction controls size and which controls strength.

- Enable it if your muscle memory expects the opposite axis layout.
- This is one of the highest-impact controls for overall feel.

### Invert Strength Direction

Invert Strength Direction reverses the vertical drag direction used for strength changes.

- Enable it if strength feels backwards relative to your expectations.
- This only changes direction mapping, not the underlying strength system.

### Enable Axis Breakout

Enable Axis Breakout allows you to switch from one adjustment axis to the other by pulling far enough across the perpendicular direction.

- Enable it if you want more fluid movement between size and strength in one gesture.
- Leave it off if you want the first committed axis to remain locked.

### Breakout Threshold (px)

Breakout Threshold sets how far you must drag perpendicular to the active axis before the HUD switches axes.

- Increase it to prevent accidental switching.
- Reduce it if switching axes feels harder than it should.

## Strength Settings

Strength Settings combine falloff preset behavior and strength scaling behavior.

### Falloff Properties

#### Allow Preset X-Scroll

Allow Preset X-Scroll lets horizontal movement cycle falloff presets.

- Enable it if you want falloff changes integrated into the HUD gesture.
- Leave it off if you want to avoid accidental preset changes while adjusting strength.

#### Falloff Preset Drag Pixels

Falloff Preset Drag Pixels sets how much horizontal movement is needed before BrushHud switches to the next falloff preset.

- Increase it if presets change too easily.
- Reduce it if cycling presets feels sluggish.

### Strength Controls

#### Override Strength Limit

Override Strength Limit allows BrushHud to target values above Blender's normal strength limit.

- Enable it if your workflow depends on a higher effective ceiling.
- Leave it off if you want BrushHud to stay inside Blender's standard range.

#### Strength Ceiling

Strength Ceiling sets the maximum strength value BrushHud will target.

- Increase it only if Override Strength Limit is part of your workflow.
- Treat it as the top end of the strength range the HUD is allowed to reach.

#### Strength Sensitivity

Strength Sensitivity determines how much vertical drag is required to change strength.

- Higher values make strength changes slower and more controlled.
- Lower values make the HUD react more aggressively.

#### Speed Multiplier

Speed Multiplier controls how strongly the sensitivity modifier slows adjustments.

- Lower values make fine control slower and more precise.
- Higher values keep the slowed mode closer to normal speed.

## UI & HUD Previewer

This group exposes the optional live HUD previewer used to inspect the HUD without having to go from 3d view to preference a million times just to test the HUD.

### Enable HUD Previewer

Enable HUD Previewer reveals the HUD Previewer and Pause buttons in the preferences header (on the far right, next to Graphics button on the main button bar).

- Enable it when you want to preview the HUD in active 3D view.
- The previewer still starts in an off state after the controls are enabled.

### HUD Previewer

HUD Previewer starts the live preview overlay.

- Use it to inspect the HUD presentation from the preferences screen.
- This is a preview tool, not part of the normal sculpt workflow.

### Pause

Pause freezes the HUD preview animation on its current frame.

- Use it when you want to examine spacing, color, or visibility without motion.
- Pause only matters while HUD Previewer is running.

##Remember to save your adjustments here## -> [Profiles and Themes](../graphics/profiles-and-themes.md#save)
