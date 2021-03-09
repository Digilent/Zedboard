# Zedboard Root Repository

IMPORTANT: No demos are currently present in this repository. Take a look at the Resource Center, link below, for earlier releases.

This repository contains all demos for the Zedboard.

For more information about the Zedboard, visit its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/zedboard/start) on Digilent Reference.

Each demo contained in this repository is documented on the Digilent Wiki, links in the table below.

| Wiki Link | Demo Master Branch | Submodules Used |
|-----------|--------------------|-----------------|
| [Zedboard <Demo Name>](https://reference.digilentinc.com/reference/programmable-logic/Zedboard/demos/<demo-name>) | <variant>/<demo>/master | HW,OS,SW, removing unused components |

## Repository Description

This repository is designed to offer a unified and comprehensive approach to all of the aspects of the demos that we provide for the Zedboard, across multiple tools. By cloning this repo recursively you will receive the repositories for Vivado projects (HW), and Vitis workspaces (SW). Each submodule may have its own submodule dependencies which will also be pulled when cloning. An important aspect of this structure is the fact that the SW heavily depends on hardware hand-off files from the HW repository.

This repository also provides releases containing project and image files used by the various tools involved. Releases provide files that are directly usable, without requiring the use git or any scripting systems. Documentation of each demo, as well as instructions for using their releases, can be found by visiting the corresponding pages on the Digilent Wiki, links below. All releases in this repository can be found in this repository's [releases page](https://github.com/Digilent/Zedboard/releases), however, use of the wiki pages to find specific well-tested releases is advised.

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked in the table of demos, above.

Demos were moved into this repository during 2020.1 updates. History of these demos prior to these updates can be found in their old repositories, linked below:
* https://github.com/Digilent/<Repo>

This repository took the place of a previous repository holding Zedboard demo projects, which can now be found at https://github.com/Digilent/Zedboard-old.