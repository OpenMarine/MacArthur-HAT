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
- changed CAN termination resistor from 1/4W to 1/10W.
- Added an extra resistor to the MOSFET controlling 12V_MAIANA to limit max voltage between gate and source. 

## v1.0 - 2023/03/21

- First version for testers
