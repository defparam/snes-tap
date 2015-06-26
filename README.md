# snes-tap
This project includes Altium design files for an SNES tapping board.

Snes-tap V1.0
---------------------------------------------------------------------
This inital version of the board design files describes a simple adapter
board that converts the SNES bottom expansion port interface to a standard
100 mil IDC header for hardware interfacing. This interface gives you access
to the data bus and the peripheral address bus of the SNES. The interface also
gives you access to analog audio channels, the reset, the interrupt pin and a
couple of clocks.

Components (Connectors)
-----------
There are two connectors used in this board. The connector which plugs into the SNES
expansion port is a rare 2.0mm pitch micro edge connector. There aren't many vendors
which create this connector type. On this board we use the SAMTEC MEC2-30-01-L-DV.
The MEC2-30-01-L-DV is a 60-pin polarized connector, since the MEC2 doesn't have a 28-pin
variant we use the MEC2-30-01-L-DV and saw/dremel off pins 29-60. The footprint in the design
is modified to adapt to this new 28-pin footprint.

The second connector is a simple 30-pin 100 mil IDC header. In this design we used the
SAMTEC TSM-114-01-L-DV.


TODO:
--------
The next version of the snes-tap will include a 5v to 3.3v logic translator for
easy interfacing to modern hardware chips.

-Evan

