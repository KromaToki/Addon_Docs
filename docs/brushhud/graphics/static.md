# Static HUD
<div style="position: sticky; top: 38px; background: var(--md-background-color); padding: 10px 0; z-index: 10;">
  <img src="../../assets/StaticHud.png" alt="Key Bindings" style="width: 100%; max-height: 700px; object-fit: cover; border-radius: 4px;">
</div>



The Static page controls how BrushHud looks when it is visible outside the main active adjustment moment.

## Static Ring

- **Show Outline**: Enables the idle ring outline.
- **Width**: Sets the thickness of that static outline.
- **Color***: Sets the static outline color.

## Static Fill

- **Enable Fill**: Keeps the static HUD filled instead of outline-only.
	- This only works when the broader size HUD uses Flat Fill mode.
	- If Flat Fill mode is not active, BrushHud treats static fill as unavailable.

## Display Options

- **Show Numeric Values**: Keeps the numeric display visible in static mode.
- **Hide Strength**: Removes the strength readout from the static display.
	- Enable it if you want a cleaner idle HUD.
	- Leave it off if the strength value is important even when you are not actively dragging.

## Fade In

- **Enable**: Turns on fade-in behavior for the static HUD.
- **Static Hud Fade-In Time**: Controls how long the static HUD takes to appear.
- **Fade In After Quick Gesture**: Delays the static reveal until the quick-gesture window has passed.
	- Enable it if you want to avoid flashing the static HUD during fast, transient motion.
	- Leave it off if you want the idle state to appear more immediately.
- **Quick Gesture Window (ms)**: Sets the time window BrushHud uses to decide whether a gesture was only a quick action.
	- Increase it if static reveal still happens too soon.
	- Reduce it if the idle HUD takes too long to return.

## Footnotes

- `*` Full version only