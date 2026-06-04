# Size HUDs
<div style="position: sticky; top: 38px; background: var(--md-background-color); padding: 10px 0; z-index: 10;">
  <img src="../../assets/sizeHuds.png" alt="Size" style="width: 100%; max-height: 700px; object-fit: cover; border-radius: 4px;">
</div>

The Size page controls the brush size ring, the numeric readout, the baseline and active markers, radial guides, and the size-specific fade behavior.

## Style

These settings control the main ring appearance and optional texture preview.

- **Fill Mode**: Chooses the main visual style for the size ring.
	- `Line` uses a line-only presentation.
	- `Flat Fill` uses one filled color.
	- `Ring` uses directional increase and decrease coloring.
	- `Ring Gradient` fades or blends ring color(s).
- **Show Brush Texture**: Displays the active brush texture inside the size ring.
	- Enable it when texture context matters during size adjustments.
	- Leave it off for a cleaner, more minimal ring.
- **Force Line Mode With Texture**: Temporarily uses line mode when the texture overlay is visible.
	- Enable it if the filled ring and texture together feel too dense.
	- Leave it off if you prefer the chosen fill mode to remain visible even with texture preview.
- **Flat Fill Color***: Sets the single fill color used by Flat Fill mode.
- **Increase Color***: Sets the positive-direction ring color used in Ring and Ring Gradient modes.
- **Decrease Color***: Sets the negative-direction ring color used in Ring and Ring Gradient modes.
- **Blend Colors**: Softens the transition between directional colors in the gradient display.
	- Enable it for a smoother gradient read.
	- Disable it for a more separated directional look.
- **Keep Relative Positions**: Preserves the gradient relationship as the display changes.
	- Enable it if you want the gradient to feel stable while resizing.
	- Disable it if you want the gradient to respond more directly to changing positions.

## Numeric Values

These settings control the size number and the capsule behind it.

- **Show Numeric Values**: Displays the size number.
- **Font Size**: Changes the size of the numeric readout.
- **Font File**: Changes the typeface used for the size readout.
- **Color Mode**: Decides whether the number uses one color or separate colors above and below the baseline.
- **Color***: Sets the single text color when a single-color mode is active.
- **Above Baseline***: Sets the text color for values above the starting size.
- **Below Baseline***: Sets the text color for values below the starting size.

### Capsule Settings

- **Show Capsule**: Draws a background capsule behind the numeric value.
- **Background Color***: Sets the capsule fill color.
- **Capsule Fade**: Lets the capsule fade over distance rather than staying equally visible.
- **Fade Start (px)**: Sets the distance where capsule fading begins.
- **Fade End (px)**: Sets the distance where capsule fading finishes.
- **Outline**: Enables a border around the capsule.
- **Outline Width**: Sets the capsule border thickness.
- **Outline Color***: Sets the capsule border color.

## Active Line and Baseline

These settings control the live marker and the starting reference marker.

### Active Line

- **Active Line**: Draws the live ring marker for the current size value.
- **Width**: Sets the active line thickness.
- **Color Mode**: Determines whether the active line uses one color or separate directional colors.
- **Increase***: Sets the active line color used above the baseline.
- **Decrease***: Sets the active line color used below the baseline.
- **Color***: Sets the active line color when a single-color mode is active.

### Baseline

- **Baseline**: Draws the reference ring at the starting size.
- **Baseline Style**: Chooses whether the baseline is solid, dashed, or dotted.
- **Width**: Sets the baseline stroke thickness.
- **Length**: Changes the dash length used by the dashed baseline style.
- **Gap**: Controls the separation between dashed baseline segments.
- **Spacing**: Controls the separation between dotted baseline marks.
- **Color***: Sets the baseline color.

## Radial Guides

These settings control the guide lines around the size HUD.

- **Show**: Enables the radial guide lines.
- **Orientation**: Chooses how the guides are aligned.
	- `Cardinal` keeps them in fixed major directions.
	- `Diagonal` rotates them to diagonal reference lines.
	- `Follow Rotation` uses the rotation HUD orientation.
- **Line Width**: Sets the guide thickness.
- **Line Length**: Sets how far the guides extend.
- **Increase Color***: Sets the positive guide color when the guides use local directional colors.
- **Decrease Color***: Sets the negative guide color when the guides use local directional colors.

## Fade In

These settings control how the size HUD appears.

- **Enable**: Turns on the size HUD fade-in behavior.
- **Fade Time**: Sets how long the size HUD takes to fully appear.

## Footnotes

- `*` Full version only