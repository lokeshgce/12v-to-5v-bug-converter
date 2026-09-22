# 🔋 12V to 5V Buck Converter Using MOSFET

A compact **12V to 5V DC-DC Buck Converter** designed using a **NE555 timer and BSS84 P-channel MOSFET**.  
The project converts a 12V DC input into a regulated 5V DC output using PWM-based switching.

## 📌 Project Overview

This project demonstrates the design and implementation of a simple **step-down (Buck) converter** using discrete components.

The **NE555 timer** generates the PWM switching signal, which controls the **BSS84 P-channel MOSFET**. The switching waveform is then filtered using an **LC filter** consisting of an inductor and capacitor to obtain a lower DC output voltage.

### 🔄 Conversion

**Input:** 12V DC  
**Output:** 5V DC  
**Topology:** Buck Converter  
**Switching Controller:** NE555 Timer  
**Power Switch:** BSS84 P-Channel MOSFET

---

## 🎯 Objectives

- Design a DC-DC buck converter for stepping down 12V to 5V.
- Generate PWM using an NE555 timer.
- Control the switching operation using a MOSFET.
- Design and simulate the circuit using LTspice.
- Design a PCB using KiCad.
- Implement the circuit on a compact PCB.

---

## 🧩 Components Used

| Component | Value / Part |
|-----------|--------------|
| NE555 Timer | NE555 |
| MOSFET | BSS84 |
| Schottky Diode | 1N5817 |
| Inductor | 100 µH |
| Capacitor | 100 µF |
| Capacitors | 0.01 µF |
| Resistor | 3.5 kΩ |
| Resistor | 1.7 kΩ |
| Load | 30 Ω |
| Input Supply | 12V DC |

---

## 🛠️ Tools Used

- **LTspice** – Circuit simulation
- **KiCad** – Schematic and PCB design
- **PCB 3D Viewer** – PCB visualization

---

## 🔲 Block Diagram

       12V DC INPUT
            │
            ▼
      ┌─────────────┐
      │   NE555     │
      │ PWM Control │
      └──────┬──────┘
             │
             ▼
      ┌─────────────┐
      │    BSS84    │
      │   MOSFET    │
      └──────┬──────┘
             │
             ▼
      ┌─────────────┐
      │  Switching  │
      │    Stage    │
      └──────┬──────┘
             │
             ▼
      ┌─────────────┐
      │ 100 µH L    │
      │     +       │
      │ 100 µF C    │
      └──────┬──────┘
             │
             ▼
          5V DC
          OUTPUT

---

## 👨‍💻 Author

**Lokesh A.**  
B.E. Electronics and Communication Engineering (ECE)  
Government College of Engineering, Salem
