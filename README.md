# Mixed-Signal PCB Board (2-Layer)
A 2-layer mixed-signal printed circuit board (PCB) designed to integrate analog and digital systems on a single board. This project was developed as part of a guided learning experience to understand signal integrity, layout partitioning, and design for manufacturing.

---

## 🧠 Objective

To develop a compact, Arduino-compatible mixed-signal PCB using ATmega328P and USB interface, focusing on layout challenges of combining analog and digital domains on a 2-layer board.

---

## 🔧 Core Components

- **Microcontroller:** ATmega328P (with bootloader)
- **USB Interface:** ATmega16U2 for USB-to-Serial
- **Power Supply:** 5V and 3.3V power rails with onboard regulation
- **Clock:** 16 MHz crystal oscillator
- **Programming Interface:** ICSP header

---

## 📡 Interfaces & IO

- USB (via ATmega16U2)
- SPI (on ICSP)
- I2C (shared with analog pins A4/A5)
- UART Serial (pins 0/1)
- 14 Digital IOs
- 6 Analog Inputs
- PWM outputs

---

## 🧩 Design Considerations

- Clear analog/digital domain separation in layout
- Differential pair routing for USB signals
- Decoupling capacitors for power stability
- USB protection circuitry
- Grounding and return path strategies
- DFM and DFx (DFA, DFT, DFC) checks
- Constraint management for trace width and clearance
- Gerber, ODB++, and IPC-2581 output for fabrication
- Fabrication drawings and assembly files

---

## 📎 Files

- [`/gerbers`](./gerbers): Gerber files for board fabrication
- [`/docs`](./docs): Schematic, layout image, optional stackup
- [`/bom`](./bom): Bill of Materials

> ⚠️ This board is not yet fabricated. Designed using OrCAD as part of training under Hasofu Academy.

---

## 👨‍🏫 Acknowledgments

Project developed with mentorship from **Kirsch Mackey**, founder of **Hasofu Academy**.

---

## 🚫 Disclaimer

This project is based on open-source Arduino schematics and adapted for educational purposes only. No proprietary or personal libraries are included.

