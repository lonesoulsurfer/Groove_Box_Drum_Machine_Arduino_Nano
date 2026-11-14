# Groove Box: Arduino Nano drum machine for Eurorack

Groove Box is a drum machine that uses an Arduino Nano. It is based on [DrumKid](https://github.com/mattybrad/drumkid) by Matt Bradshaw. Groove Box adds 3 trigger outputs to sync other synths, and it fits in a Eurorack case.

![Groove Box](https://github.com/user-attachments/assets/4eea0471-dde1-4ed7-b2dd-f4e1370c1a82)

## Build guide and video

- Step-by-step build guide on Instructables: [Groove Box - Arduino Nano Drum Machine](https://www.instructables.com/Groove-Box-Arduino-Nano-Drum-Machine/)
- Video on YouTube: [Groove Box](https://youtu.be/VaNvsRpYE2A)

## Features

- Arduino Nano drum machine with the DrumKid sound engine
- 3 trigger outputs, to sync with other synths
- Fits in a Eurorack case
- Power from a 16-pin Eurorack power connector, or from 9 V (or 12 V) through a JST connector
- Can operate from a 9 V battery

## What you need

### Hardware

- All parts are in the [list of parts](List%20of%20Parts.pdf).
- The schematic is [Schematic.png](Schematic.png).
- The Gerber files for the PCB and the front panel are in [Gerber Files](Gerber%20Files/). You can send them to a PCB maker.

### Software

- Arduino IDE
- An Arduino Nano

You do not need to install libraries. The sketch folder already has the two libraries that it uses, in `Arduino Sketch/GrooveBox/src/`.

> **Note:** Do not install Mozzi from the Library Manager for this project. The sketch uses its own changed copy of Mozzi. A newer Mozzi does not cause a problem, because the sketch does not use it.

## Upload the firmware

1. Download this repository. Click **Code → Download ZIP**, then extract the ZIP file.
2. Open `Arduino Sketch/GrooveBox/GrooveBox.ino` in the Arduino IDE.
3. Connect the Arduino Nano to your computer with a USB cable.
4. In the **Tools** menu, set these values:
   - **Board:** Arduino Nano
   - **Processor:** ATmega328P
   - **Port:** the COM port of your Nano
5. Click **Upload**.
6. Wait for the message **Done uploading**.

> **Note:** If the upload fails, set **Processor** to **ATmega328P (Old Bootloader)**, then try again. Many clone Nano boards need this setting.

## How to play

The instructions are in [How to Play - Instructions.pdf](How%20to%20Play%20-%20Instructions.pdf).

## Files in this repository

| Folder or file | Contents |
|----------------|----------|
| `Arduino Sketch/GrooveBox/` | Firmware, with the libraries that it uses |
| `Eagle Files/` | Eagle files for the PCB |
| `KiCad - Front Panel/` | KiCad and DXF files for the front panel |
| `Groove Box - Front Panel Design.svg` | Front panel artwork |
| `Gerber Files/` | Gerber files for the PCB and the front panel, ready to order |
| `List of Parts.pdf` | Parts list |
| `How to Play - Instructions.pdf` | How to play |
| `Schematic.png` | Schematic |

## Why I made it

I want to make my own modular synth that is simple to build. Each module has these aims:

- It operates from 9 V (and 12 V).
- It is easy to build, with a minimum of components.
- It uses an Arduino, to keep the parts count low and everything in tune.
- It fits in any Eurorack case, and it can use normal Eurorack power.
- It sounds good.
- It is portable, and it can operate from a 9 V battery.

![Groove Box module](https://github.com/user-attachments/assets/99cd2d2f-db10-4bef-a9e0-91c678bc92be)

## Credits

- Sound engine, firmware and original PCB: [DrumKid](https://github.com/mattybrad/drumkid) by Matt Bradshaw.
- Audio library: [Mozzi](https://sensorium.github.io/Mozzi/) by Tim Barrass (a changed copy, made for DrumKid).
- Button library: [Bounce2](https://github.com/thomasfredericks/Bounce2) by Thomas Fredericks.
- Eurorack version, trigger outputs and front panel: Marcus ([lonesoulsurfer](https://github.com/lonesoulsurfer)).

## Support

Do you like this project? You can support my work on [GitHub Sponsors](https://github.com/sponsors/lonesoulsurfer).

## Licence

- This project uses the [MIT License](LICENSE), the same as DrumKid.
- **Important:** The firmware includes a copy of Mozzi that has a non-commercial licence. Do not sell the firmware, or a device with this firmware, without permission from the Mozzi author.
- [LICENSING.md](LICENSING.md) gives the details.
