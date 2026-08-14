# DrillWise Test Report

## Current version

```text
v2.1
```

## Overall result

```text
PASS - Documentation baseline prepared
```

This test report is a repository documentation file. It records the expected retained functionality for the working `index.html` baseline.

## Required retained modules

| Check | Expected status |
|---|---|
| Inputs / Upload present | PASS |
| PPFG upload/import retained | PASS |
| Wellpath upload/import retained | PASS |
| Well Schematic retained | PASS |
| Wellpath / Trajectory retained | PASS |
| Riser Margin retained | PASS |
| Gas Migration retained | PASS |
| Kick Tolerance retained | PASS |
| Capacity retained | PASS |
| Time vs Depth retained | PASS |
| App name remains `DrillWise Well Planner` | PASS |

## v2.1 expected Time vs Depth behaviour

| Behaviour | Expected status |
|---|---|
| Time vs Depth tab available | PASS |
| Activity table available | PASS |
| Build draft from section table available | PASS |
| Drilling rows move in depth over time | PASS |
| Casing / running rows stay stationary at depth while time moves | PASS |
| Cement / flat-time rows stay stationary at depth while time moves | PASS |
| MD/TVD basis selector available | PASS |
| Casing shoe overlays available | PASS |

## Regression guard

For future changes, check that the following still work before accepting a new version:

1. Open the app in Chrome or Edge.
2. Confirm the app opens without JavaScript error.
3. Confirm PPFG upload still works with the known working PPFG file.
4. Confirm wellpath upload still works with the known working survey file.
5. Confirm Well Schematic opens.
6. Confirm Riser Margin plot opens.
7. Confirm Gas Migration plot opens.
8. Confirm Kick Tolerance opens and calculates.
9. Confirm Capacity opens and calculates.
10. Confirm Time vs Depth opens and plots.

## Development instruction for Claude or other coding tools

When updating this project, only modify the requested module. Preserve the existing working implementation of all unrelated modules.

If a requested change is small, prefer a small patch rather than a full rewrite.
