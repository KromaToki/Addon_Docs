# Profiles

## Save a Profile

Open Edit > Preferences > Add-ons > PrefsPlus, expand PrefsPlus Configuration, and click Save Profile.

PrefsPlus exports a JSON file containing:

- Profile schema version
- Add-on name
- Blender version
- Header spacing setting
- Section dropdown settings
- Persistent header button setting
- Pinned add-on module ids
- Pin labels
- Pin icons
- Pin text visibility
- Pin header order

## Load a Profile

Click Load Profile and choose a PrefsPlus JSON profile.

By default, loading a profile replaces existing pins. The file browser option Replace Existing Pins controls whether current pins are cleared first.

PrefsPlus validates that the file is a JSON object, that the schema is supported, and that the profile belongs to PrefsPlus.

## Missing Add-ons

Profiles store pinned add-ons by module id. If a profile references an add-on that is not installed in the current Blender setup, PrefsPlus skips that pin and reports the missing module names.

Install the missing add-ons, then load the profile again if those pins should be restored.

## Profile Compatibility

PrefsPlus currently uses profile schema version `1`.

Profiles are intended for moving a PrefsPlus header setup between Blender installations that have the same add-ons available.

