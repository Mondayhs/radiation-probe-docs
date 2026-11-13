# HK / SCI | Data Flow Concept

## Housekeeping (HK)

HK provides payload health and operational state information. It is useful for monitoring, but **should not be assumed to contain the entire science record**.

## Science (SCI)

SCI records are acquired and stored separately. Retrieval behavior depends on the firmware implementation and the appropriate ICD and user-data request commands.

**Conceptual flow:**

1. Payload acquires RADFET / NAND measurements.
2. Firmware assembles science records and updates the storage metadata.
3. HK provides selected status/summary fields.
4. Approved readback commands retrieve stored science records.
5. Parser checks the actual byte layout, CRC, counters, times and conversion formulas.

## Important diagnostic distinction

A new SCI record number is not by itself proof of a valid new physical measurement. A GUI graph that appears constant is not by itself proof that the payload stopped measuring.

To investigate, cross-check:

- raw communication logs vs. decoded data
- timestamp and record-number progression
- valid ADC conversion and units
- operating mode and science sampling interval
- firmware version and parser version

Avoid mixing byte orders or field offsets from different ICD revisions. Detailed packet layouts and operational command sequences stay in the private engineering documentation.
