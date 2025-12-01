# Zeva_BMS12v3_MEB
Zeva BMS12v3 firmware modified to support the VW MEB temperature sensors

This build of the firmware assumes a 10k NTC 3380K B sensor

_To build the firmware, CD to /Firmware and run:_

**$ make**

_This step is only required for new, unprogrammed modules:_

**$ avrdude -c usbtiny -p m16m1 -U lfuse:w:0xFF:m**

_To flash the BMS module with the new firmware_

**$ avrdude -c usbtiny -p m16m1 -U flash:w:Zeva_BMS12_v3.hex**
