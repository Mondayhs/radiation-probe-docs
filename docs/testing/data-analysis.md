# Test Data & Analysis

A handover-quality test produces **replayable raw data** plus enough metadata to reproduce the parser output.

## Recommended records

| Artifact | Purpose |
|---|---|
| Raw UART / science logs | Ground truth for packet parsing |
| Parsed CSV | Human-readable derived output |
| Firmware commit / test GUI commit | Version-specific interpretation |
| ICD revision | Byte layout and commands |
| Test plan and operator notes | Conditions and expected behavior |
| Figures and analysis script | Reproducible conclusions |

## Common checks

- HK continuity and mode transition events
- SCI numbering and timestamps (watch for unchanged or stale entries)
- RADFET physical units and calibration assumptions
- NAND SEU classification and count validity
- Packet integrity and correctly applied byte-order rules

The source test tools are maintained in [DSRP-CRP-GUI (private)](https://github.com/Mondayhs/DSRP-CRP-GUI). Never publish unpublished radiation test logs without authorization.

## RADFET temperature note

RADFET measurements may require temperature compensation. The existing handover points to a **DSRP RADFET Data Correction** document (not included here) that should be linked after publication approval and version verification.
