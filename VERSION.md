# DrillWise Version

## Current version

```text
v2.1
```

## Current baseline

The current source of truth should be the working `index.html` file that opens correctly and contains the latest working DrillWise software.

## Versioning convention

### Minor fixes

Use minor versions for bug fixes and small UI adjustments:

```text
v1.1
v1.2
v1.3
v2.1
v2.2
```

Examples:

- small schematic adjustment
- colour/layout tweak
- bug fix in an existing module
- hover label correction
- upload mapping correction

### Major versions

Use a new major version for new tabs or major modules:

```text
v2.0
v3.0
```

Examples:

- new Time vs Depth tab
- new cementing module
- new hydraulics module
- campaign overview module

## Current module status

| Module | Status |
|---|---|
| Inputs / Upload | Retain as working baseline |
| Well Schematic | Retain as working baseline |
| Wellpath / Trajectory | Retain as working baseline |
| Riser Margin | Retain as working baseline |
| Gas Migration | Retain as working baseline |
| Kick Tolerance | Retain as working baseline |
| Capacity | Retain as working baseline |
| Time vs Depth | Added in v2.0, refined in v2.1 |

## Critical development instruction

When changing DrillWise, only modify the requested area. Do not alter unrelated modules.

For example, if the request is:

```text
Move the Riser Margin colour controls
```

then do not change:

- PPFG upload
- wellpath upload
- gas migration
- kick tolerance
- capacity
- schematic
- time vs depth

## Current app name

The visible name inside the application should remain:

```text
DrillWise Well Planner
```
