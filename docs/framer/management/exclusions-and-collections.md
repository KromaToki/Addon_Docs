# Exclusions and Collections

## Exclusion Types

Framer supports two exclusion levels:

- Object exclusion: excludes one object from Framer framing calculations.
- Collection exclusion: excludes objects in that collection from Framer framing calculations.

Exclusion flags are stored on Blender objects and collections in the current file.

## Sidebar Exclusion List

Open 3D View > Sidebar (`N`) > View > Framer.

The Framer panel includes:

- Smart Frame
- Excluded object list
- Excluded collection list
- Refresh Exclusions
- Reset All Exclusions
- Per-entry clear buttons

Use Refresh Exclusions when the displayed list does not match the current object or collection flags.

## Object Exclusions

Object exclusions are available from:

- Object Properties > Visibility > Framer > Exclude from Framing
- Object context menu in the 3D View
- The Framer sidebar exclusion list, when clearing an existing exclusion

Some object types show a standalone Framer panel in Object Properties when Blender's normal Visibility parent panel is not available.

## Collection Exclusions

Collection exclusions are available from:

- Collection Properties > Framer > Exclude from Framing
- Outliner collection context menu
- The Framer sidebar exclusion list, when clearing an existing exclusion

Excluding a collection excludes that collection's contents from Framer target gathering. Clear the collection exclusion when objects inside it should be available for Smart Frame again.

## Sole Framable Collection

The Outliner collection context menu includes Make Sole Framable. This keeps the chosen collection frameable and excludes sibling collections at the same hierarchy level. For nested collections, Framer also keeps the parent chain included and excludes competing branches.

When multiple sibling collections are selected in the Outliner, Framer can make the selected collections the only frameable siblings together.

The 3D View object context menu includes Make Parent Collection Sole Framable. If an object belongs to more than one collection, Framer offers collection-specific entries so the intended source collection can be chosen explicitly.

## Reset and Include Commands

Reset All Exclusions clears object and collection Framer exclusion flags and clears the sole-frameable collection marker.

Additional operators exist for collection-wide management:

- `framer.exclude_all_collections`
- `framer.include_all_collections`
- `framer.select_frameable_objects`
- `framer.reset_all_exclusions`
- `framer.exclusion_refresh`

