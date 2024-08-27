# Doro56
***
![Image](/pics/build.jpg)

A 56-key split keyboard with a reversible PCB that uses normal mods, an exploded number row, a semi-columnar staggered layout, plus support for rotary encoders.

[ZMK config](https://github.com/gehennaXXIV/zmk-config-Doro56)

It has a supporting JSON file for https://nickcoutsos.github.io/keymap-editor/

QMK config - None yet - RP2040 Pro Micro support soon

***
## Changelog

#### v1.1 - Minor Edit
- **Caps and Enter Footprints**: Changed to a single reversible footprint (previously used two single key footprints rotated).
- **JST PH Footprint**: Adjusted and relocated for increased flexibility.
- **PCB Cutout**: Modified to remove blank space between Control and Alt keys, allowing space for a 402030 battery without increasing the case height clearance.
- **Plate**: Slightly increased the cutout size for the rotary encoder.


***
## Build Guide
None yet, but for a quick overview:
* [Solder the MCU](https://raw.githubusercontent.com/gehennaXXIV/Doro56/main/pics/mcu.jpg) with the components facing down, and the TRRS jack on top of the half you are building. For MCU socketing, the footprint was modified to allow [sockets with thick pins to work](https://down-ph.img.susercontent.com/file/sg-11134201-7qvco-ley7fi4ef44v33). You can use milmax pins, or, what I use, harvested gold pins from a 5-pin RGB header (also cheaper). [Sample 2](https://raw.githubusercontent.com/gehennaXXIV/Doro56/main/pics/sockets.jpg)
* Bridge the [jumpers](https://raw.githubusercontent.com/gehennaXXIV/Doro56/main/pics/bridge.jpg) on the MCU from underneath, and add other components such as diodes, MX sockets, and the power switch.

![Image](/pics/pcb.jpg)

***
## PARTS
| **COMPONENTS**             |  Qty  |  Remarks |
| :------------------------- | :---: | :------  |
| Diodes 1N4148W (SMD)        |  56   | SOD-123  |
| MX Switch Sockets           |  56   |          |
| 2U PCB-Mount Stabilizers    |  04   |          |
| Power Switch                |  02   | MSK12C02 |
| Reset Switch                |  02   | MJTP1250 |
| JST 2 PH Right Angle Jack   |  02   |          |
| TRRS Jack                   |  02   |  MJ-4PP-9 or PJ320A |
| Rotary Encoder              |  02   | EC11 - acrylic case has enough clearance for 22mm knobs |

***
| **MCU**                        |  Qty  |  Remarks |
| :----------------------------- | :---: | :------  |
| Low Profile MCU sockets        |  04   |  Does not need to be expensive milmax sockets. The MCU socket footprint was modified to allow [sockets with thick pins to work](https://down-ph.img.susercontent.com/file/sg-11134201-7qvco-ley7fi4ef44v33) |
| Mill Max Pins                  |  48   |  Mouser 3320-0-00-15-00-00-03-0, or a cheaper option: harvested gold pins from a 5-pin RGB header (just snip off the plastic parts) |
| Nice Nanos                     |  02   |  or NRF52840 clones |
| Li-Po Battery                  |  02   |  **Take note of the polarity before plugging it in.** [Here's a tutorial on how to change the polarity.](https://www.youtube.com/watch?v=za-azgbZor8) |

***
| **CASE**                                |  Qty  |  Remarks |
| :--------------------------------------- | :---: | :------  |
| [Acrylic Case](/Case/acrylic)            |  01   | Maybe a 3DP one soon, but I'm very content with the acrylic case. Let me know if you create one! |
| M2 6mm Wafer Head Screws                 |  20   | Plate screws |
| M2 10mm Round Standoff Spacer            |  10   | Plate standoffs, add +2mm if you need bottom clearance (see case readme) |
| M2 8mm Wafer Head Screws                 |  32   | Case screws |
| M2 13mm Round Standoff Spacer            |  16   | Case standoffs, add +2mm if you need bottom clearance (see case readme) |
| Rubber Feet                              |  08   | Currently, the keyboard lays flat. I’ve yet to design a base layer for angled feet |

***
## FOOTPRINTS USED
* https://github.com/ebastler/marbastlib
* https://github.com/joe-scotto/scottokeebs
* https://github.com/GEIGEIGEIST/KLOR
* https://github.com/50an6xy06r6n/keyboard_reversible.pretty

***
## DISCLAIMER
Please note that while this keyboard is provided as open-source, I am not liable for any issues, malfunctions, or other problems that may arise from its use. The keyboard is provided "as-is," and I make no warranties or guarantees regarding its performance or functionality. Use at your own risk.
