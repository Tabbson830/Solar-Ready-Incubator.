# Solar-Ready-Incubator.
A hybrid power digital poultry incubator for rural applications.
# 🐣 A Solar-Ready Digital Poultry Egg Incubator

**An engineering response to rural power instability, providing continuous hybrid power for agricultural resilience.**

---

## 📌 The Problem
In Zambia, a national power deficit of over 1,111 megawatts has led to extensive load-shedding schedules (up to 20 hours a day). For rural poultry farmers relying on commercial digital incubators, this is catastrophic. Standard incubators are grid-dependent (220V AC); when the power fails, the internal temperature drops, leading to immediate embryo mortality and significant economic loss. 

## 💡 The Proposed Solution
This project introduces a **"Solar-Ready" Hybrid Digital Incubator**. It acts as a bridge between high-tech incubation and rural infrastructure challenges. 

By prioritizing **Active Power Resilience**, the system accepts Grid Power (AC) when available to conserve battery life, but utilizes an engineered Automatic Transfer Switch (ATS) to seamlessly transition to a Solar Battery (DC) backup during load shedding. 



---

## ⚙️ Key Technical Features
1. **Autonomous Power-Path Circuitry:** Detects grid failure and switches to solar battery backup in under **50 milliseconds**, preventing the microcontroller from resetting during the transition.
2. **Precision Environmental Sensing:** Utilizes the DHT22 sensor for real-time monitoring of internal conditions.
3. **PID Temperature Controller:** A microcontroller-based Proportional-Integral-Derivative (PID) algorithm maintains a strictly stable $37.5^\circ C$ environment with a minimal $\pm0.5^\circ C$ variance.
4. **Automated Actuation:** Integrates an automated mechanical egg-turning mechanism to ensure uniform heat distribution, alongside DC-DC Buck Converters operating at >90% efficiency to maximize battery life.

---

## 🛠️ Methodology: Agile & Incremental
The development of this embedded system follows an Agile and Incremental approach, moving away from high-risk waterfall design.

* **Increment 1 (Power & ATS):** Designing and unit-testing the relay-based Automatic Transfer Switch and diode OR-ing logic.
* **Increment 2 (Sensing):** Interfacing the DHT22 and calibrating environmental data streams.
* **Increment 3 (Control):** Implementing the PID heating algorithm and mechanical turning logic.

---

## 📂 Repository Structure

* `/src` - Contains the C++ source code for the microcontroller (Arduino/ESP32).
* `/hardware` - Contains circuit schematics (Proteus/Fritzing) and the Bill of Materials (BOM).
* `/docs` - Project proposals, presentation slides, and technical reports.

---

## 🚀 Getting Started (Prototype Phase)
*Currently in the active build phase. Code and schematics will be pushed to their respective directories incrementally.*

### Planned Hardware Stack:
* **Controller:** Arduino Uno / ESP32
* **Sensors:** DHT22 (Temperature & Humidity)
* **Power Electronics:** 5V Relay Modules, DC-DC Buck Converters (LM2596)
* **Energy Source:** 12V 18Ah SLA Battery, 50W Solar Panel, 220V-to-12V AC Adapter

---

## 👨‍💻 Author
**Tabbson Simukonda** Computer Engineering  
The Copperbelt University
