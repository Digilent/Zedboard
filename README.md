# Zedboard Root Repository

## Zedboard FMC-Pcam-Adapter Demo

### Description

This branch contains sources for the Zedboard FMC-Pcam-Adapter Demo.

This project demonstrates the usage of the FMC Pcam Adapter as an interface from one to four different Pcam cameras and the ZedBoard platform. The Video Stream from each different camera is getting in through the MIPI/FMC connectors and out through the carrier VGA port. For errors and feed-back messages, an UART interface is present.	

For more information on the Zedboard FMC-Pcam-Adapter Demo, including setup instructions, visit its [Demo Page](https://digilent.com/reference/programmable-logic/zedboard/demos/fmc-pcam) on the Digilent Wiki.

For more information on the Zedboard, including other demos that may be available, see its [Resource Center](https://digilent.com/reference/programmable-logic/zedboard/start) on the Digilent Wiki.

#### Implementation details

During the 2022.1 upgrade, significant changes were made to the VDMA synchronization mechanism, which is needed to make sure the write operations (camera frames being stored to DDR) and read operations (VGA output reading frames from DDR) don't overlap, resulting in unwanted frame tearing. More details can be found on the demo's wiki page and in both Vivado and Vitis projects' comments.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Zedboard).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes      |
| OS        | No       |
| SW        | Yes      |

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* ZedBoard with an external 12V Power Supply
* 2 Micro-USB cables. One for programming and the other one for the uart interface
* 1 VGA cable
* FMC-Pcam-Adapter board
* From 1 to 4 Pcam-5C cameras
* VGA monitor
