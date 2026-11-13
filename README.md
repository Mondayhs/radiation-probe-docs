# NCU Radiation Probe Knowledge Base

Public onboarding and engineering handover for **DSRP → CRP / COSPAR-1**.

> **Documentation status:** Working draft. This repository contains public orientation material, not flight-approved operating instructions. Keep firmware, hardware design files, detailed ICDs, credentials, and unapproved test logs in private repositories.

## Browse the website

Website (after GitHub Pages deployment): https://mondayhs.github.io/radiation-probe-docs/

## Local preview

```bash
python -m pip install -r requirements.txt
mkdocs serve
```

The documentation source lives in `docs/`. Edit Markdown files, submit updates, and verify technical claims against the released firmware revision, ICD, and test evidence.

## Public / private boundary

- **Public:** This documentation, mission background, onboarding, high-level design evolution, and approved learning materials.
- **Private:** CRP source, PCB design files, detailed interface documentation, raw test logs, calibration data, and unpublished engineering records.

Private repository references may be visible as names or links; they are not made public by linking to them. Do not embed private file contents in GitHub Pages builds.
