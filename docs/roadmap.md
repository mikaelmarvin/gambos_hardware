# Roadmap

Open hardware work on **v1.0** and planned changes for **later hardware iterations**. Move items to done as they complete; add v1.1+ entries only when they target a new PCB spin, not v1.0 bring-up.

Firmware work is tracked in the [firmware roadmap](https://github.com/mikaelmarvin/Gambos-Flight-Controller/blob/main/docs/software/roadmap.md).

## Current iteration (v1.0)

### Hardware

- Document assembly and bench test procedure (or link from bring-up notes)
- Testing of bulk capacitors on servo motors and their response -> osciloscope measuring

### Documentation

- Hardware pages: fill placeholders (e.g. power measurements, LDO notes)
- BOM with manufacturer part numbers in repo or linked spreadsheet

## Next hardware iteration (v1.1+)

Changes intended for a **future PCB revision** after v1.0 bring-up and flight tests — not general repo todos.

### Fixes from v1.0 bring-up

- S2 pin, which is dedicated to the SERVO2 motor cannot be mapped to a hardware generated PWM signal in stm32cubemx, thus making this hardware version not be able to control 5 servos, but 4 (S1, S3, S4, S5).

### Design improvements under consideration

- Copper pour and stitching can be done in a more elegant way
- Add a GNSS module with a ready made antenna, 
- BLE would be interesting
- Humidity sensor
- Ditch the MUTAG ESD component; it is a nightmare to solder -> general component selection optimized for easier soldering

---

[Documentation index](../README.md)
