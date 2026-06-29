```md
# My PMP

> A prototype portable media player built around the ESP32-S3.

This is my first hardware project. Instead of designing a custom PCB immediately, I built this prototype using off-the-shelf modules to learn the complete hardware design process. The long-term goal is to integrate everything onto a single PCB and turn it into the compact clip-on media player I originally envisioned.

---

## The Idea

I wanted a dedicated music player for running without the distractions of a smartphone.

The original concept was a clip-on device that simply plays music and gets out of the way. This prototype focuses on validating the hardware architecture before moving to a custom PCB and a much smaller enclosure.

---

## Features

- Shake to wake
- Touchscreen interface
- Built-in speaker
- Wi-Fi music transfer
- MicroSD storage
- Deep sleep support

---

## Transferring Songs

The ESP32 hosts its own Wi-Fi access point.

Connect to the device from your phone or laptop, open a browser, and drag and drop songs directly onto the SD card. No dedicated app or cable is required.

---

## Circuit Diagram

![Circuit Diagram](circuitdiagram.png)

The entire system is centered around the ESP32-S3. The display, touch controller, RTC, motion sensor, audio amplifier, charging module, and SD card are connected through SPI, I2C, I2S, and GPIO interfaces while keeping every pin conflict-free.

---

## Enclosure Design

### Overall Design

![Overall CAD](overall-cad.png)

The enclosure was designed around the hardware instead of forcing the hardware to fit into an existing case. Every cutout, mounting point, and opening was added only after the internal layout was finalized.

### Internal Layout

![Internal Layout](internal-layout.png)

After creating the shell, each component was positioned as a dummy model inside the enclosure to verify spacing, port alignment, cable routing, and overall fit before printing.

---

## Bill of Materials

The complete parts list, purchase links, and pricing can be found in [bom.csv](bom.csv).

---

## Future Plans

This prototype validates the overall hardware architecture.

Future revisions will focus on:

- Designing a custom PCB
- Reducing the enclosure size
- Returning to the original clip-on form factor
- Improving battery integration
- Reducing internal wiring

---

Built for **Macondo** 🚀
```

