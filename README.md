# LDM1-LED Display Board
Adapter board to drive HDSP-C2x3 common cathode seven segment displays.  
## Overview
This board can be mounted underneath a HSDP-C2x3 display to allow easy driving via MCU.  
It uses a SN74HC594DR shift register and TBD62783AFWG driver IC to control the display.  
Resistor values are selected for a 10 - 13V LED supply.  
Depending on module color it might be necessary to increase R8 for even brightness on the decimal point.  
Modules are designed for use with a LDM8E controller. Find more info in this [repository](https://github.com/ndornseif/LDM8E-LEDDisplayController).  
## Pinout
- DRIVE: Input for 10 - 13V LED driving voltage.
- Digital VCC: Input for 2 - 5V logic supply voltage.
- Data IN: Serial data input to shift register.
- Data OUT: Serial data output from shift register.
- Register CLK: Clock for output register. Use to apply changes after data input.
- Serial CLK: Shift register clock for serial data input.
- AGND: LED ground connection. Allows for low side switching of LEDs.
- GND: Digital ground connection.
- Register CLR: Clear contents of shift register and output register (active low).
- NC: Not connected.
## Other
Published under CERN-OHL-S license.