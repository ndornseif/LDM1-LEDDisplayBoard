# LDM1-LED Display Board
Adapter board to drive HDSP-C2x3 common cathode seven segment displays.  
## Overview
This board can be mounted underneath a HSDP-C2x3 display to allow easy driving via MCU.  
It uses a SN74HC594DR shift register and a TBD62783AFWG driver IC to control the display.  
Resistor values are selected for a 10–13 V LED supply.  
Depending on module color, it might be necessary to increase R8 for even brightness at the decimal point.  
Modules are designed for use with a LDM8E controller. Find more information in this [repository](https://github.com/ndornseif/LDM8E-LEDDisplayController).  
## Pinout
- DRIVE: Input for 10–13V LED driving voltage
- Digital VCC: Input for 2–5V logic supply voltage
- Data IN: Serial data input to the shift register
- Data OUT: Serial data output from the shift register
- Register CLK: Clock for the output register  
Use to apply changes after data input.  
- Serial CLK: Shift register clock for serial data input
- AGND: LED ground connection  
The separate LED ground allows for low-side switching of LEDs.  
- GND: Digital ground connection  
- Register CLR: Clear the contents of the shift register and output register (active low)   
- NC: Not connected
## Other
Published under CERN-OHL-S license.


