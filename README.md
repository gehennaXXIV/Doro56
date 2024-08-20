# Doro56
***
![Image](/pics/build.jpg)

A 56 key split keyboard with reversible PCB that uses normal mods, with an exploded number row and a semi-columnar staggered layout, plus support for rotary encoders.

[ZMK config](https://github.com/gehennaXXIV/zmk-config-Doro56)

It has a supporting json file for https://nickcoutsos.github.io/keymap-editor/ 


QMK config - none yet

Build Guide - none yet, but for tldr; 
* solder mcu, trrs on top of the halve you are building. the mcu socket footprint was modified to allow [sockets with thick pins to work](https://down-ph.img.susercontent.com/file/sg-11134201-7qvco-ley7fi4ef44v33). you can either use milmax pins, or what i use, harvested gold pins from a 5 pin rgb header (also cheaper). [sample](<img src="https://raw.githubusercontent.com/gehennaXXIV/Doro56/main/pics/sockets.jpg" width="200" />
)
* bridge the [jumpers](https://raw.githubusercontent.com/gehennaXXIV/Doro56/main/pics/bridge.jpg) on the mcu from under, and other components such as diodes mx sockets, also power switch.

![Image](/pics/pcb.jpg)


***
## PARTS
| **COMPONENTS**             |  Qty  |  Remarks |
| :--------------------- 	 | :---: | :------  |
| Diodes 1N4148W (SMD)	 	 |  56   | SOD-123  |
| MX Switch Sockets		     |  56   |          |
| 2U PCB-Mount Stabilizers   |  04   |          |
| Power Switch				 |  02   | MSK12C02 |
| Reset Switch 		 		 |  02   | MJTP1250 |
| JST 2 PH Right Angle Jack	 |  02   |          |
| Rotary Encoder             |  02   | EC11 - acrylic case has enough clearance for 22mm knobs |

***
| **MCU**                        |  Qty  |  Remarks |
| :--------------------- 		 | :---: | :------  |
| Low Profile MCU sockets        |  04   |  Does not need to be expensive millmax sockets, the mcu socket footprint was modified to allow [sockets with thick pins to work](https://down-ph.img.susercontent.com/file/sg-11134201-7qvco-ley7fi4ef44v33)
| Mill Max Pins					 |  48   |  Mouser 3320-0-00-15-00-00-03-0, or a cheaper one, harvested gold pins 5pin RGB header (just snip off the plastic parts)
| Nice Nanos                     |  02   |  or NRF52840 clones
| Li-Po Battery                  |  02   |  TAKE NOTE OF THE POLARITY BEFORE PLUGGING IT IN [Here's a tutorial on how to change the polarity.](https://www.youtube.com/watch?v=za-azgbZor8)

***
| **CASE**                                |  Qty  |  Remarks |
| :--------------------- 		          | :---: | :------  |
| [Acrylic Case](/Case/acrylic)           |  01   | maybe a 3DP one soon, but I'm very content with the acrylic case. LMK if you create one! |
| M2 6mm Wafer Head Screws		          |  20   | Plate screws
| M2 10mm Round Standoff Spacer           |  10   | Plate standoffs, add +2mm if you need bottom clearance (see case readme) |
| M2 8mm Wafer Head Screws		          |  32   | Case screws |
| M2 13mm Round Standoff Spacer           |  16   | Case standoffs, add +2mm if you need bottom clearance (see case readme) |
| Rubber Feet					          |  08   | Currently the keyboard lays flat, I've yet to design a base layer for angled feet |

***
## FOOTPRINTS USED
* https://github.com/ebastler/marbastlib
* https://github.com/joe-scotto/scottokeebs
* https://github.com/GEIGEIGEIST/KLOR
* https://github.com/50an6xy06r6n/keyboard_reversible.pretty

***
## DISCLAIMER
Please note that while this keyboard is provided as open-source, I am not liable for any issues, malfunctions, or other problems that may arise from its use. The keyboard is provided "as-is," and I make no warranties or guarantees regarding its performance or functionality. Use at your own risk.
