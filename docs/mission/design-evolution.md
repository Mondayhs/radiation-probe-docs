# DSRP → CRP | Design Evolution & Lessons Learned

This page preserves the chain **Observed issue → Root cause or requirement → CRP implementation → Verification evidence**.

!!! warning "Draft, not a flight-release change log"
    The table summarizes development discussions. **Implemented does not mean verified.** Add the precise firmware commit, ICD revision, test setup, raw log and reviewer before declaring each item released.

| Topic | DSRP observation / limitation | CRP improvement | Verification evidence |
|---|---|---|---|
| RADFET long-run operation | Interruption of continuous measurements was observed | Review reset/error counters and recovery behavior | Attach approved long-run report |
| NAND SEU anomaly | Repeated fixed error count (3456) was observed | Correct counting and verification paths | Attach before/after records |
| SEU characterization | Limited separation of error mechanisms | Erased / programmed patterns; static / dynamic classification | Link radiation test and firmware revision |
| SEU readback confidence | Single read can be ambiguous | Triple-read verification | Verify classification on approved test data |
| Boot configuration | Reset recovery and stored configuration require care | Protected persistent parameters, CRC, mirrored storage | Cite FSW and boot tests |
| CubeSat integration | Different platform interfaces | COSPAR-1 connectors, UART / RS-422 and interface handling | Confirm hardware and ICD revision |
| Firmware robustness | Counter and health-reporting anomalies | State handling, watchdog and command management corrections | Link tested commit and log |

## Design change record template

~~~yaml
id: CRP-CHANGE-XXX
symptom_or_requirement: TBD
root_cause_status: suspected / confirmed / not applicable
implementation:
  repository: TBD
  commit: TBD
  firmware_version: TBD
interface_impact: TBD
verification:
  method: TBD
  raw_log: TBD
  report: TBD
  outcome: pending
reviewer: TBD
release_status: not approved
~~~

## Evidence still needed

- [ ] DSRP radiation flight dataset and anomaly investigation report
- [ ] Root cause and source-code evidence for the repeated SEU count
- [ ] COSPAR-1 CRP firmware change-to-commit mapping
- [ ] Long-run continuity and proton SEE test reports
- [ ] Version-specific ICD and release approval

Do not use this public high-level summary as a substitute for the private engineering change log.
