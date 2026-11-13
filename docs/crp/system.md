# CRP System Tour

CRP combines two types of radiation measurements:

- **RADFET:** assesses total ionizing dose through threshold-voltage behavior, with temperature and calibration considerations.
- **NAND Flash:** observes radiation-related bit errors, with careful interpretation of erased/programmed data states and read-verification results.

## Major functional blocks

1. Radiation sensors and associated analog measurement circuitry
2. SmartFusion2-based digital processing and firmware
3. Nonvolatile memory for measurement records and selected configuration data
4. Payload-to-platform communication
5. Housekeeping (HK) and science (SCI) storage / readback

## How to study the hardware

Begin with the approved block diagram, power-tree description and hardware revision; do not derive safe connector pinouts or power limits from this public overview. The hardware design files are in the [private CRP repository](https://github.com/Mondayhs/compact-radiation-probe).

## Next

[Programming and firmware](programming.md) · [HK/SCI data flow](data-flow.md) · [First test](../testing/first-test.md)
