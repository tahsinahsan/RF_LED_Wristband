# Aurabrace
I am the designer of Aurabrace.
Aurabrace is a low-power wireless LED wristband system designed for synchronized lighting effects, inspired by large-scale audience interaction devices. The system uses an RF receiver, a Padauk microcontroller, and onboard memory to deliver dynamic LED patterns efficiently.

---

## 🔧 Hardware Overview

Aurabrace is built using a minimal and cost-efficient hardware stack:

* **MCU:** Padauk PFS154
* **RF Receiver:** CMT2210LH
* **Clock Source:** External crystal oscillator
* **Memory:** External EEPROM (for storing lighting effects)
* **Output:** 2 × LEDs (onboard)

---

## ⚙️ System Architecture

The system operates as follows:

1. **RF Signal Reception**
   The RF receiver (CMT2210LH) captures wireless broadcast signals containing effect data.

2. **Data Processing (MCU)**
   The PFS154 microcontroller decodes incoming data and determines which lighting effect to execute.

3. **Effect Storage (EEPROM)**
   Predefined lighting patterns are stored in EEPROM. The MCU reads effect sequences from memory.

4. **LED Driving (PWM Control)**
   The MCU uses hardware PWM to drive LEDs with smooth fades, brightness control, and timing accuracy.

---

## 💡 Features

* Ultra low-cost design
* Hardware PWM-based LED control
* RF-controlled synchronized lighting
* EEPROM-based effect storage
* Battery-efficient operation
* Compact wearable form factor

---

## 🔋 Power Efficiency

Aurabrace is optimized for low power consumption:

* Uses hardware PWM (minimal CPU load)
* Low system clock configuration
* Efficient RF polling strategy
* Suitable for battery-powered wearable devices

---

## 🎯 Use Cases

* Concert audience wristbands
* Event synchronization lighting
* Interactive installations
* Wearable LED systems

---

## 🚀 Project Goals

* Achieve smooth LED fading with minimal hardware
* Maintain reliable RF communication
* Optimize battery life for long-duration events
* Keep firmware simple and efficient

---

## 📌 Notes

* Hardware PWM is used for LED fading to reduce CPU usage.
* Timing and fade effects are controlled via software counters.
* RF protocol implementation depends on transmitter configuration.

---

## 📂 Status

🛠️ In development

---

## 🤝 Contributions

This project is currently experimental. Contributions, optimizations, and ideas are welcome.

---

## 📜 License

TBD
