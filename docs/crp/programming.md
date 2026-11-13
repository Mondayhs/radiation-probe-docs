# SmartFusion2 | Firmware and Programming

This page is an **orientation guide**, not a complete programming SOP.

## Existing instructional materials

- [CRP firmware repository (private)](https://github.com/Mondayhs/compact-radiation-probe)
- [SmartFusion2 CRP programming video](https://youtu.be/LCdHjrpG3Nc)
- [COSPAR-1 hardware programming precautions (video)](https://youtube.com/shorts/jd6NB5zPXXo)

These links were included in the handover notes. Confirm that videos and their content are approved for public linking.

## Revision-control rules

- Always record **board revision**, **FSW branch/commit**, **ICD revision**, and **test-script revision**.
- Make experimental changes on a dedicated Git branch. Never overwrite the release baseline.
- Build and flash only with the team's verified toolchain and approved board-level programming procedure.
- Verify the active firmware by an agreed method after programming, and preserve console/HK logs.

## UART baud-rate changes

Modifying the code alone is not sufficient: the host interface and receiving software must use compatible settings. Consult the specific FSW release and ICD before changing any communications parameter.

## Missing materials for a complete SOP

- [ ] Approved power and cable connection diagrams
- [ ] Exact SmartFusion2 toolchain versions and programming file selection
- [ ] Approved build steps, image naming and checksum procedure
- [ ] Recovery and troubleshooting procedure after a failed flash
