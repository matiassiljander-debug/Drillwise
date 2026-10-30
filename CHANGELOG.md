# DrillWise Changelog

## Riser margin fixes

### Fixed

- Riser margin plot x-axis labels were offset by 0.05 SG. Gridlines started at 0.75 and stepped by 0.2, so the line labelled "1.5" was really at 1.55 (and so on across the axis). Gridlines are now placed on whole multiples of 0.1 SG with labels every 0.2 SG, in the shared plot function, so the same error cannot appear on other plots.
- Riser margin is now always checked at each RM section's top and TD (PP interpolated from the PPFG), as well as at every PPFG point in between. Previously only PPFG points inside the section were used, so the section TD - usually the tightest point - was skipped unless a PPFG point landed exactly on it.
- Missing inputs no longer show as a false "LOW": rows now say NO WD / AIR GAP, NO PP, NO MW or ABOVE SEABED. A blank water depth was previously treated as 0 m and could pass as "OK".

## v2.1

### Changed

- Updated the Time vs Depth module so drilling activities move in depth over time.
- Updated casing / running / cement / flat-time activities so they remain stationary at the current depth while time moves.
- Updated the `Build draft from section table` workflow to create separate drilling rows and casing/liner running rows where a casing or liner shoe matches the section end.

### Intended behaviour

- `Phase = Drilling` or any phase containing `drill` should plot as a depth-progressing activity.
- `Phase = Casing`, `Cement`, `Flat`, `BOP`, `Other`, or similar should plot as stationary depth while time increases.

### Non-changes

The following modules should remain unchanged from the working baseline unless explicitly edited later:

- PPFG upload/import
- Wellpath upload/import
- Well Schematic
- Riser Margin
- Gas Migration
- Kick Tolerance
- Capacity
- Wellpath 3D
- App name

## v2.0

### Added

- Added new `Time vs Depth` tab.
- Added manual time-depth activity table.
- Added `Build draft from section table`.
- Added add row / clear rows controls.
- Added apply table and update plot workflow.
- Added CSV/Excel import hook for time-depth rows.
- Added CSV export for time-depth rows.
- Added MD/TVD basis selector.
- Added casing shoe overlays.
- Added hover values for activity lines and casing shoes.
- Added summary cards for:
  - total planned days
  - drilling days
  - flat / other days
  - planned TD

## v1.x working baseline

### Retained baseline functionality

- Bigger plots
- Movable schematic labels
- 3D hover data box
- Gas migration curve clipping
- Riser Margin retained
- Gas Migration retained
- Kick Tolerance retained
- Capacity retained
- Normal app name retained

## Development notes

Future changes must be scoped narrowly. Do not rebuild the full app unless explicitly requested.
