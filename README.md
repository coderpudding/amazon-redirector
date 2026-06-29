# My PMP

> A prototype portable media player built around the ESP32-S3.

This is my first hardware project. The goal of this prototype is to validate the hardware architecture before moving to a custom PCB and a smaller clip-on design.

---

## The Idea

I wanted a dedicated music player for running without the distractions of a smartphone.

The original concept was a compact clip-on player with a touchscreen, onboard speaker, and wireless song transfer. This prototype focuses on proving the core hardware before building that final version.

---

## Features

- Shake to wake
- Touchscreen interface
- Onboard speaker
- Wi-Fi song transfer
- Deep sleep support
- SD card music storage

---

## Transferring Songs

The ESP32 creates its own Wi-Fi access point.

Simply connect from your phone or laptop, open a browser, and upload songs directly to the SD card—no dedicated app required.

---

## Circuit Diagram

![Circuit Diagram](circuitdiagram.png)

The entire system is centered around the ESP32-S3. Audio is handled through an I2S amplifier, storage comes from a MicroSD card, while the touchscreen, RTC, and motion sensor communicate over SPI and I2C.

---

## Enclosure Design

![Enclosure Render](enclosure.png)

The enclosure was designed around the hardware instead of forcing the hardware to fit inside an existing case.

The shell was built first, followed by the screen opening, speaker grille, USB-C cutout, SD card slot, and magnet mounts. Every module was then positioned inside as a dummy model to verify clearances before printing.

---

## Bill of Materials

The complete parts list, prices, and purchase links are available in **bom.csv**.

---

## Future Plans

This prototype is the foundation for future revisions.

- Custom PCB
- Smaller enclosure
- Original clip-on form factor
- Better battery integration
- Reduced wiring# amazon-redirector
