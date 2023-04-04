# LDM1-LEDDisplayBoard
Adapter board to drive HDSP-C2x3 seven segment displays.  
Hardware version: 1.2.0  
## Overview
This board can be mounted underneath a HSDP-C2x3 display to allow easy driving via MCU.  
It uses a SN74HC594DR shift register and TBD62783AFWG driver IC to control the common cathode display module.  
Resistor values are selected for a 10-13V supply.
## Pinout
- DRIVE: Input for 12V LED driving voltage.
- +5V: Input for 2-6V logic supply voltage.
- DIN: Serial data input to shift register.
- DOUT: Serial data output from shift register.
- Serial CLK: Shift register clock for serial data input.
- Register CLK: Clock for shift register output register. Use to apply changes after data input.
- AGND: LED ground connection. Allows for low side switching of LEDs.
- GND: Digital ground connection.
## Other
Published under CERN-OHL-S license.