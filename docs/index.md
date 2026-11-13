# Radiation Probe Knowledge Base

**Deep Space Radiation Probe (DSRP) · Compact Radiation Probe (CRP) · COSPAR-1**

Welcome to the public onboarding portal for NCU's radiation payload development. The aim is to help new team members understand **why the systems were designed**, **where to find approved engineering resources**, and **how to prepare for supervised testing**.

!!! warning "Public educational documentation — not a flight procedure"
    The pages here are a *handover draft*. Technical values and steps must be checked against the applicable hardware revision, firmware commit, ICD revision, and approved test SOP before use. This website must not contain private engineering files.

## Choose your starting point

<div class="grid cards" markdown>

- :material-school: **New to the project?**

    [Start Here — first week →](start/first-week.md)

- :material-satellite-variant: **Understand the missions**

    [DSRP & CRP overview →](mission/overview.md)

- :material-source-branch: **Why was CRP redesigned?**

    [DSRP → CRP design evolution →](mission/design-evolution.md)

- :material-flask-outline: **Prepare for a CRP test**

    [First test guide →](testing/first-test.md)

- :material-alert-circle-outline: **Something is wrong?**

    [Troubleshooting →](troubleshooting.md)

- :material-bookshelf: **Find the right file**

    [Engineering resources →](resources.md)

</div>

## Recommended learning path

**Understand the mission → Identify the board and firmware revision → Read the current ICD → Review the approved setup → Observe HK → Verify science data and archive logs.**

A healthy-looking HK stream alone is **not proof** of valid new scientific measurements. Use the relevant firmware version, decoded SCI records, timestamps, and raw logs to verify behavior.

## What stays private?

Detailed board design, source code, sensitive interfaces, calibration files, and unpublished logs are maintained in access-controlled repositories. Public pages contain only orientation, approved references, and conceptual procedures.

**Maintainers:** Please review [Release & Verification Status](maintenance/release-status.md) before treating a feature as validated.
