# DrillWise Well Planner

DrillWise is a browser-based drilling engineering planning tool. The software is currently maintained as a single-file web app, with `index.html` as the main application file.

## How to run

Open the file below in a modern browser:

```text
index.html
```

Recommended browsers:

- Google Chrome
- Microsoft Edge

## Current version

```text
v2.1
```

## Main modules

- Inputs / Upload
- Well Schematic
- Wellpath / Trajectory
- Riser Margin
- Gas Migration
- Kick Tolerance
- Capacity
- Time vs Depth
- Export / Checks

## Key capabilities

### Inputs / Upload

- PPFG upload and column mapping
- Wellpath / survey upload and column mapping
- Excel / CSV / LAS-style input workflow, depending on the current working `index.html`
- Manual casing / liner / section input tables

### Well Schematic

- Subsea-style well schematic
- Casing and liner strings
- Cement shown outside casing
- Liner hanger / TOL marker
- Open-hole interval
- Movable labels where supported by current build

### Wellpath / Trajectory

- 3D wellpath view
- Plan view
- Selected-point / hover information
- MD/TVD lookup functionality

### Riser Margin

- PP, FG, Shmin and collapse curves
- Planned mud weight
- Required mud weight
- Casing shoe markers
- Hover values where supported by current build

### Gas Migration

- Gas migration screening plot
- PP / Shmin / FG comparison
- Casing shoe markers
- Gas migration pressure / EMW curve

### Kick Tolerance

- Section-based kick tolerance calculation
- PP and FG values from PPFG where supported
- Normal and swabbed kick scenario functionality

### Capacity

- Section capacity calculations
- Open-hole and annular capacity basis

### Time vs Depth

- Activity-based time vs depth table
- Build draft from section table
- Drilling rows move in depth over time
- Casing / running / cement / flat-time rows stay stationary at depth while time moves
- MD/TVD basis selector
- Casing shoe overlays

## Development rules

When making future changes:

1. Only change the requested module.
2. Do not rebuild the whole app unless explicitly requested.
3. Do not change upload/import logic unless the request is specifically about upload/import.
4. Do not change Riser Margin, Gas Migration, Kick Tolerance, Capacity, Well Schematic or Wellpath unless specifically requested.
5. Keep the visible application name as:

```text
DrillWise Well Planner
```

## Versioning rule

- Minor fixes: `v1.1`, `v1.2`, `v1.3`, etc.
- New tabs or major modules: `v2.0`, `v3.0`, etc.
- Current major version: `v2.1`

## GitHub note

Keep the repository private if the software contains internal well names, field data, PPFG data, wellpath data, formation tops, or other company-sensitive content.

Do not commit real operational well data unless this is explicitly approved.
