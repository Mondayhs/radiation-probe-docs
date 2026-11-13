# Troubleshooting | 常見異常

This is a diagnosis index, **not** a list of confirmed root causes for every firmware revision.

| Observation | First checks | Evidence to retain |
|---|---|---|
| HK received but SCI seems stale | Mode, sampling interval, record timestamps, NAND readback | Raw HK and SCI plus parser version |
| RADFET values unchanged | ADC fields, voltage conversion, measurement cadence | Raw ADC values and decoded voltages |
| Reference voltage seems implausible | ADC resolution / Vref formula and byte order | Original packet and conversion code |
| Unexpected reset or health counter | Command-error logic and reset reason for active release | Power trace, HK, FSW revision |
| Fixed/repeated SEU count | Readback alignment, algorithm, data validity | Raw memory/error records |
| Readback packet mismatch | ICD byte offsets, length, CRC, numbering | Hex dump and full command/response pair |

## Triage order

1. Secure raw logs and stop making assumptions from GUI plots.
2. Note exact hardware, firmware, ICD and parser versions.
3. Separate sensor measurement, FSW processing, transport and parser issues.
4. Try a *documented, non-destructive* reproduction under supervision.
5. Create a private engineering issue with evidence and link a safe public summary only when approved.

**Important:** A suspected cause is not a verified cause. Track unresolved findings under [Open Items](maintenance/open-items.md).
