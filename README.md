# Zeva_BMS12v3_MEB
Zeva BMS12v3 firmware modified to support the VW MEB temperature sensors

To build the firmware, CD to /Firmware and run:

$ make

This step is only required for new, unprogrammed modules:

$ avrdude -c usbtiny -p m16m1 -U lfuse:w:0xFF:m

To flash the BMS module with the new firmware

$ avrdude -c usbtiny -p m16m1 -U flash:w:Zeva_BMS12_v3.hex
