# snes-tap
This project includes Altium design files for an SNES expansion port tapping board to enable FPGA snooping of the SNES console.

Snes-tap V1.2 Rev B
---------------------------------------------------------------------
This is the second major release of this project. Drastic changes have
been made to allow for on board voltage translation support. The board
geometries have been modified to accommodate the active components and 
to interface to a 40-PIN 100mil header (instead of 30-pin in Rev A). 
The pinout of this header conforms with the GPIO 40-pin header of the 
Terasic DE0-Nano and DE0-Nano-SoC FPGA dev boards. Zipped up gerber/drill 
files have been submitted for easy fabrication direct to OSHPark 
without any DRC issues. Also included PDF schematic/layout and a 3D image
model of the board to be fabbed.

Snes-tap V1.0 Rev A
---------------------------------------------------------------------
This inital version of the board design files describes a simple adapter
board that converts the SNES bottom expansion port interface to a standard
100 mil IDC header for hardware interfacing. This interface gives you access
to the data bus and the peripheral address bus of the SNES. The interface also
gives you access to analog audio channels, the reset, the interrupt pin and a
couple of clocks.

Components (Connectors)
---------------------------------------------------------------------
There are two connectors used in this board. The connector which plugs into the SNES
expansion port is a rare 2.0mm pitch micro edge connector. There aren't many vendors
which create this connector type. On this board we use the SAMTEC MEC2-30-01-L-DV.
The MEC2-30-01-L-DV is a 60-pin polarized connector, since the MEC2 doesn't have a 28-pin
variant we use the MEC2-30-01-L-DV and saw/dremel off pins 29-60. The footprint in the design
is modified to adapt to this new 28-pin footprint.

The second connector is a simple 30-pin 100 mil IDC header. In this design we used the
SAMTEC TSM-114-01-L-DV. (REV A only)

On Rev B the pin header will be 40-pin 100 mil IDC. The part number is TBD.


TODO:
--------
Assemble the board, fix issues and incorporate fixed into v1.4 Rev C

-Evan

