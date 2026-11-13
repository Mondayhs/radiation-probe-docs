# Your First CRP Test | 第一次測試

**Goal:** With qualified supervision, confirm payload identity, communications, HK readout, SCI generation/readback, and reproducible logs.

!!! danger "Do not energize or flash hardware from this web page alone"
    The public draft lacks the approved pinout, supply/current limits, precise equipment configuration, applicable PCB revision and signed-off test SOP. Obtain them from the responsible engineer before testing.

## A. Preparation checklist

- [ ] Record operator, test date and board/serial revision.
- [ ] Verify FSW commit/tag, ICD revision, GUI/parser version.
- [ ] Obtain approved wiring, grounding, power setup and instrument list.
- [ ] Establish an unambiguous raw-log storage location.
- [ ] Assign an experienced tester to supervise the setup.

## B. Workflow overview

1. **Visual inspection:** verify board and connectors against the approved drawing.
2. **Approved power-up:** have an authorized operator apply the approved procedure.
3. **Communication check:** confirm connection using a sanctioned non-destructive command.
4. **HK check:** capture raw packets and inspect decoded status and time.
5. **SCI check:** confirm that science processing produces new data and that stored records can be retrieved.
6. **Archive:** retain original packets, decoder settings, observations and exception notes.

## C. Acceptance questions

- Are records actually new, or is the parser showing repeated/stale values?
- Are reference-voltage and RADFET calculations physically plausible?
- Can SCI readback be tied to the expected source record and timestamp?
- Did a reset or mode change occur during the test?
- Can another engineer reproduce the findings using the documented versions?

## D. Minimal test log template

~~~text
Test ID:
Date / operator:
Hardware revision / serial:
FSW commit/tag:
ICD revision:
GUI/parser commit:
Approved setup reference:
Expected result:
Actual HK behavior:
Actual SCI behavior:
Raw log location:
Anomalies and issues:
Reviewer:
~~~

For interpretation and troubleshooting see [Data Analysis](data-analysis.md) and [Troubleshooting](../troubleshooting.md).
