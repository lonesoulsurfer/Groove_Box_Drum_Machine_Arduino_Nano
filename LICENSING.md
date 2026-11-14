# Licensing

## This project: MIT

The firmware, the PCB files, the front panel files and the documents in this repository use the MIT License. See [LICENSE](LICENSE).

Groove Box is based on [DrumKid](https://github.com/mattybrad/drumkid) by Matt Bradshaw. DrumKid uses the MIT License. Thus [LICENSE](LICENSE) has two copyright lines: one for Matt Bradshaw and one for Marcus (lonesoulsurfer).

- The firmware is DrumKid firmware 1.2, with small changes.
- The PCB is based on the DrumKid PCB.
- The front panel design and the Eurorack version are by Marcus (lonesoulsurfer).

## Libraries in the sketch folder

The sketch folder has copies of two libraries in `Arduino Sketch/GrooveBox/src/`. They keep their own licences.

| Library | Licence | Notes |
|---------|---------|-------|
| `MozziDK` (a changed copy of [Mozzi](https://sensorium.github.io/Mozzi/), made for DrumKid) | Creative Commons Attribution-NonCommercial-ShareAlike 4.0 | **No commercial use.** See below. |
| [Bounce2](https://github.com/thomasfredericks/Bounce2) | MIT | Copyright (c) 2013 thomasfredericks |

## Important: no commercial use of the firmware

The copy of Mozzi in this project uses a non-commercial licence. The compiled firmware includes this copy. Thus you must not sell the firmware, or a device with this firmware, unless the Mozzi author gives you permission.

You can build Groove Box for yourself. You can share it and change it, under the same conditions.

Newer versions of Mozzi (version 2 and later) use the LGPL-2.1 licence, which permits commercial use. This project does not use them.
