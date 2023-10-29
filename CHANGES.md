## v1.2 - 2023/10/29

- upgrade to KiCad 7.
- changed 1-Wire pull-up from 3.3k to 1.6k.
- changed Seatalk R22 from 3.3k to 1.6k.
- changed the RJ45 connector from through-hole to surface mount.

## v1.1 - 2023/06/17

- Rebuilt Seatalk1 circuit replacing opto with a transistor to make it work in all cases.
- Removed Seatalk1 jumper.
- New screw terminal configuration to make wiring clearer and more consistent.
- Removed option to power from NMEA 2000 or Seatalk1 networks to meet standards.
- Relocation of the I2C connector on the front side for easy access.
- Added 3.3V ESD diodes to Seatalk RX and Shutdown-detection to protect Pi GPIOs.
- Changed 1-Wire ESD diodes from 5V to 3.3V.
- Changed from 3.3K to 1K resistor to make amber LEDs brighter.
- Tweaked a few resistor values to minimize number of different parts.
- The CAN termination resistor changed from 1/10W to 1/4W.
- Rebuilt 12V switch circuit to use MOSFET for controlling power from main 12V input to MAIANA.

## v1.0 - 2023/03/21

- First version for testers
