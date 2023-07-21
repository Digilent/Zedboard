# Zedboard Root Repository

## Zedboard OLED Demo

### Description

| Button     | Function                                                           |
| ---------- | ------------------------------------------------------------------ |
| BTNC       | With the display on, each pixel on the display can                 | 
|            | be lit up at once by pressing the center D-Pad button (BTNC).      |
|            | Press the BTNC to return the display to its original state         |
| BTNU       | With the display on, you can load pre-defined text onto the        |
|            | display by pressing the up D-Pad button (BTNU)                     |                          
| BTNR       | The OLED display can be turned on and off by pressing the CPU_RESET|
|  	     | button above the PROG button                                       |
| BTND       | To clear the display, press the down D-Pad button (BTND)           |

!!! Before shutting down/reprogramming the board please make sure you properly turn off the OLED display by pressing the BTNR button. When the display is off, LD0 should also be off.
This is necessary to prevent damaging the OLED display.

After shutting down the OLED display from the BTNR button, it is possible to open it again from the BTNR button only after 3.5 seconds passed.

This branch contains sources for the Zedboard OLED Demo.

This project is a Vivado demo using the Zedboard's LEDs, pushbuttons and OLED Display written in Verilog. When programmed onto the board, the display will automatically be initialized. When you are done operating the demo, and want to turn your board off, press the BTNR to turn the display off. LED0 is tied to the status of the OLED display. If the LED0 is on so is the OLED display. The display can be turned on from an off state by pressing the CPU Reset Button again. The OLED Display is controlled by the BTNR, BTNU, BTNC and BTND of the D-Pad Buttons.

For more information on the Zedboard OLED, including setup instructions, visit its [Demo Page](https://digilent.com/reference/programmable-logic/zedboard/demos/oled) on the Digilent Wiki.

For more information on the Zedboard, including other demos that may be available, see its [Resource Center](https://digilent.com/reference/programmable-logic/zedboard/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Zedboard).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes      |
| OS        | No       |
| SW        | No       |

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* ZedBoard with an external 12V Power Supply
* 1 Micro-USB cable, for programming
