# Rotation HUD
<div style="position: sticky; top: 38px; background: var(--md-background-color); padding: 10px 0; z-index: 10;">
  <img src="../../assets/rotation.png" alt="Key Bindings" style="width: 100%; max-height: 700px; object-fit: cover; border-radius: 4px;">
</div>

The Rotation page controls the compass display, the numeric angle readout, the compass shell, and the small cursor marker used during rotation.

## Limitation

BrushHud cannot display procedural textures such as Cloud or Perlin. Regular image files such as JPG and PNG are supported.

## Compass

- **Diameter**: Changes the overall size of the rotation compass.

### North Indicator

- **Offset from Center**: Moves the north indicator away from the middle of the compass.
- **Line Width**: Sets the north indicator thickness.
- **Color at Center***: Sets the inner north indicator color.
- **Color at Edge***: Sets the outer north indicator color.

### Tick Marks

- **Degree Step**: Controls the angular spacing between minor tick marks.
- **Tick Line Width**: Sets the thickness used for the compass tick marks.
- **South/East/West**: Enables the main non-north cardinal marks.
- **Line Length**: Controls how far those main tick marks extend.
- **Color***: Sets the shared color for the main cardinal marks.
- **Minor**: Enables the smaller intermediate tick marks.
- **Line Length**: Controls how far the minor ticks extend.
- **Color***: Sets the minor tick color.

## Numeric Values

- **Font**: Enables the numeric rotation readout.
- **Display at Cursor**: Places the numeric degrees near the cursor instead of leaving them in the compass area.
	- Enable it when you want the angle readout to stay close to the active gesture.
	- When this is enabled, some cursor-circle styling becomes less relevant.
- **Size**: Changes the numeric rotation text size.
- **Font File**: Changes the typeface used by the rotation number.
- **Color***: Sets the numeric text color.
- **Background Color***: Sets the capsule background behind the numeric readout.
- **Outline**: Enables a border around the rotation value capsule.
- **Width**: Sets the capsule outline thickness.
- **Color***: Sets the capsule outline color.

## Background and Outline

- **Background**: Enables the compass backdrop.
- **Color***: Sets the compass backdrop color.
- **Outline**: Enables the main compass ring.
- **Width**: Sets the compass ring thickness.
- **Color***: Sets the compass ring color.

## Rotation Cursor

- **Size**: Changes the size of the cursor circle marker.
- **Stylus Offset**: Changes how far the cursor marker is positioned from the stylus or cursor reference.
- **Fill**: Enables color fill inside the cursor circle.
- **Color***: Sets the cursor circle fill color.

## Footnotes

- `*` Full version only