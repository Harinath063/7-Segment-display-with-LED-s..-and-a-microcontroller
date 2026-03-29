# 🔢 ESP32 LED-Based 7-Segment Display (Common Cathode)

## 📌 Overview

This project demonstrates how to build a **7-segment display using individual LEDs** and control it using an ESP32 microcontroller in Wokwi.
Instead of using a prebuilt display module, this design uses **discrete LEDs arranged in segment form (A–G)** to visually represent digits from **0 to 9**.

---

## ⚙️ Features

* Displays digits from **0 to 9 continuously**
* Uses **ESP32 GPIO pins** for control
* Built using **individual LEDs (custom 7-segment)**
* Designed and simulated in **Wokwi**
* Simple and beginner-friendly implementation

---

## 🧰 Components Required

* ESP32 Development Board
* 7 × LED segments (multiple LEDs per segment optional)
* 7 × Resistors (220Ω–330Ω)
* Breadboard (optional in real hardware)
* Connecting wires

---

## 🔌 Circuit Description

* The circuit follows a **Common Cathode configuration**
* All LED **cathodes (-)** are connected to **GND**
* Each segment (A–G) is connected to an ESP32 GPIO pin through a resistor

### 📍 Pin Mapping

| Segment | ESP32 GPIO |
| ------- | ---------- |
| A       | 23         |
| B       | 22         |
| C       | 21         |
| D       | 19         |
| E       | 18         |
| F       | 5          |
| G       | 17         |

---

## 💡 Working Principle

Each segment of the display is controlled by a GPIO pin:

* **HIGH (1)** → Segment ON
* **LOW (0)** → Segment OFF

By combining different segments, digits from **0 to 9** are formed.

Example:

* **0 → A, B, C, D, E, F ON**
* **1 → B, C ON**

---

## ▶️ Simulation

This project is designed using the Wokwi simulator.
You can run the simulation by uploading the code and wiring the circuit as described.

---

## 🚀 Applications / Use Cases

This project is very useful for:

* 📚 Learning **digital electronics basics**
* 🤖 Understanding **GPIO control in ESP32**
* 🔌 Practicing **hardware wiring and circuit design**
* 🧠 Building foundation for:

  * Digital clocks
  * Counters
  * Embedded systems projects
* 🏭 Understanding how real **7-segment displays work internally**

---

## ⚠️ Important Notes

* Always use **resistors** to protect LEDs
* Ensure all **cathodes are connected to GND**
* Verify correct **LED polarity**
* Avoid using input-only pins on ESP32

---

## 📄 Code

The Arduino code controls each segment to display numbers from 0–9 using GPIO pins.

---

V.Venkata Harinath 
ECE Diploma SVGP TIRUPATI.
