# Profiles and Themes
<div style="position: sticky; top: 38px; background: var(--md-background-color); padding: 10px 0; z-index: 10;">
  <img src="../../assets/graphics_themes.png" alt="Key Bindings" style="width: 100%; max-height: 700px; object-fit: cover; border-radius: 4px;">
</div>

The Graphics category's first section is the profile editor. It's the control center for selecting, linking, saving, importing, and exporting appearance presets. 

## Workflow

For most users, the cleanest appearance workflow is:

1. choose or create a graphics profile,
2. tune the HUD properties,
3. save the result,
4. link it to the current Blender theme if you want auto-load behavior.

## Blender Theme Section

This is on the left side and contains:

### Theme Picker

The theme picker chooses the Blender theme BrushHud should evaluate for theme-linked profile matching.

- Use it to inspect or resolve the active theme-profile relationship.
- This does not directly change HUD styling on its own; it changes the theme context BrushHud uses.

### Refresh Theme Link

<img src="../../assets/refresh_theme_link.png" alt="refresh_theme_link" style="position: sticky; top: 0px; float: left; max-width: 50px; margin: 0 0 0px 0px; border-radius: 1px; box-shadow: 0 4px 10px rgba(0,0,0,0.15);">

Refresh reevaluates the relationship between the current Blender theme and the linked BrushHud profile.

- Returns the profile to the assigned theme.

### Not Linked Warning
<img src="../../assets/not_linked.png" alt="refresh_theme_link" style="position: sticky; top: 0px; float: left; max-width: 50px; margin: 0 0 0px 0px; border-radius: 1px; box-shadow: 0 4px 10px rgba(0,0,0,0.15);">

The warning appears when the current theme does not have a clear BrushHud profile assigned.

- This just means no profile isn't linked yet
- Use the Link profile button or create one from the theme to remove the warning.

## BrushHud Profile

The BrushHud Profile box manages the graphics preset itself.
!!! WARNING "Save Manually"
    Currently you must save your changes manually before exiting Blender. Otherwise they won't be loaded next session
    Just  click the file save (icon) when finished (or have settings you like)


### Profile Picker

The profile picker chooses which saved graphics profile is active.

- Use it to swap the entire appearance setup quickly.
- If a theme is already linked, the chosen profile may also act as that theme's resolved default.

### Link or Unlink Theme Association

The link button attaches the selected graphics profile to the current Blender theme.

- Link when you want BrushHud to auto-load a specific appearance for that theme.
- Unlink when you no longer want that theme to resolve to the profile automatically.

### Create Graphics Profile (+)

Create Graphics Profile (+) builds a new BrushHud profile with current graphics setting, and names the profile after the current Blender theme.

- Use it to quickly start a new profile from scratch.

### Save

Save updates the currently active graphics profile.

- Use it when you have refined a profile and want to keep the same name.
- It is best for incremental edits.

### Delete

Delete removes the active graphics profile.

- Use it when a preset is obsolete, redundant, or superseded.
- Delete only affects the saved profile, not the current Blender theme itself.

### Save As
 
- Use it to branch from a profile without overwriting the original.
- This is the safest save option when experimenting heavily.

### Import

Import loads a graphics profile from disk.

BrushHud supports import modes for graphics profiles:

- Graphics + HUD Style: import Graphics properties and color styling.
- HUD Style Only: import the structural HUD styling while keeping current theme-compatible colors.
- Graphics Colors Only: import only the color layer and keep current HUD structure.

### Export

Export writes the current or selected graphics profile to a file.

- Use it for backup, distribution, or migration.
- Export is also the easiest way to preserve a stable release look.

### Folder (icon)

Open Folder opens the graphics profile directory in windows.

- Use it for manual file management or backup.
- This is also useful when reviewing imported profile files directly.
