# 🌙 Smart Streetlight Dimming System

> 🚧 This project is a **conceptual prototype** submitted for the **BYTE Program** by **Texas Instruments**.  
> 🛠 We have developed the idea and simulation but not implemented it in hardware yet.

---

## 📌 Overview

This project proposes an **energy-efficient streetlight system** that dynamically adjusts brightness based on real-time traffic detection. Using motion sensors and wireless communication, the system aims to reduce power wastage, minimize light pollution, and improve public safety.

---

## 🎯 Problem Statement

Urban streetlights stay fully powered even in low or no traffic zones post-midnight, leading to:

- ❌ Unnecessary power consumption
- 💸 High electricity bills
- 🌃 Light pollution
- 🌍 Increased environmental impact

---

## 🎯 Objective

Design and propose a **smart dimming system** for streetlights that:

- ✅ Detects motion (vehicles or pedestrians)
- ✅ Brightens or dims accordingly
- ✅ Works in all weather conditions
- ✅ Maintains privacy (no cameras)
- ✅ Uses low-power wireless communication

---

## 🧩 System Architecture

### 🧠 Components Used

| Component        | Function                              | Power (Wh/day) | Cost (₹)     |
|------------------|---------------------------------------|----------------|--------------|
| **TI CC1312R**   | Sub-1 GHz Wireless MCU                | 0.23           | ₹3000–₹4000  |
| **AWR6843 Radar**| Object detection up to 200m           | 13.64          | ₹2500–₹2850  |
| **LDR Sensor**   | Detects ambient light                 | 3.6            | ₹5–₹10       |
| **INMP441 Mic**  | Optional sound sensing                | 0.04           | ₹250–₹600    |
| **Other**        | Battery, solar panel, wiring, etc.    | —              | ₹220–₹1000   |
| **Total**        | Per unit estimate                     | —              | ₹6070        |

---

## 🔋 Power Consumption

| System               | Consumption (Wh/day) |
|----------------------|----------------------|
| Conventional LED     | 3016                 |
| Smart Streetlight    | 1456                 |
| **Saved Per Unit**   | **1560 Wh/day**      |

---

## 📡 Communication & Detection

- **AWR6843 Radar**: mmWave FMCW radar to detect object motion up to 200m, weather-resistant.
- **TI CC1312R**: Sub-1 GHz wireless MCU for communication between streetlight clusters.
- One radar controls 5 streetlights spaced ~35m apart.

---

## 🧪 Simulation Demo

A conceptual simulation is built using Arduino on TinkerCad.

🔗 [View TinkerCad Simulation](https://www.tinkercad.com/things/b3ShjQMp1lT-smart-street-light-?sharecode=pYmFXSowwQA3zFg-XhGliW5zqv3pkTI-yd5uiAeoYkk)

### 🔧 Instructions

1. Click "Start Simulation"
2. Adjust photoresistor light levels
3. In darkness, lights turn ON
4. Motion sensor detects proximity of object
5. If object is near, brightness increases
6. When no object is present, lights dim

---
