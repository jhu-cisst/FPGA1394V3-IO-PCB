# FPGA1394V3-IO-PCB

PCB design for I/O board used with [FPGA1394V3](https://github.com/jhu-cisst/FPGA1394V3), in KiCad format.

This board connects to the DF11 connector (J9) on FPGA1394V3, which provides +3.3V, GND and 4 I/O signals (MIO34-37) from the Zynq SoC PS, and makes protected versions of these signals available on a DB9F connector. Specifically, the +3.3V output has a 100 mA current limit and the I/O signals have 50 Ohm current-limiting resistors and a transorb (TVS diode) for protection.

This board is used in the [dVRK Si Controller](https://github.com/jhu-dvrk/dVRK-Si-Controller), starting with Rev 4 of the enclosure.

## Files

* `dvrk-ios.kicad_pro`: KiCad project file
* `dvrk-ios.kicad_sch`: Schematics (KiCad format)
* `dvrk-ios.kicad_pcb`: PCB layout (KiCad format)
* `dvrk-ios-bom.xlsx`: Bill of Materials (Excel format)
