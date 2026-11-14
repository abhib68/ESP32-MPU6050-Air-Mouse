# 🖱️ ESP32 MPU6050 Wireless BLE Air Mouse

[![ESP32](https://img.shields.io/badge/ESP32-BLE_HID-blue.svg)](https://www.espressif.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Hardware](https://img.shields.io/badge/Hardware-DIY-green.svg)](#)

An open-source, gesture-controlled **3D Bluetooth HID Air Mouse** built using an **ESP32** microcontroller and an **MPU6050** 6-axis Gyroscope & Accelerometer sensor.

Move your mouse cursor seamlessly across Windows, macOS, Linux, and Android devices simply by moving your hand in the air.

---

## 📸 Demo & Circuit Diagram

> *Add a GIF of your air mouse in action and your wiring diagram image here.*
> `![Circuit Diagram](path/to/diagram.png)`

---

## 🛠️ Hardware Components

* **ESP32 Development Board** (ESP32-WROOM-32 or similar)
* **MPU6050** 6-Axis Accelerometer & Gyroscope Module
* **Push Buttons** (2x for Left & Right Click)
* **Breadboard & Jumper Wires**
* **Micro-USB / USB-C Cable** (or LiPo battery for portable use)

---

## 🔌 Wiring / Pinout

| MPU6050 / Button | ESP32 Pin | Notes |
| :--- | :--- | :--- |
| **VCC** | `3.3V` | Power supply |
| **GND** | `GND` | Common ground |
| **SCL** | `GPIO 22` | I2C Clock |
| **SDA** | `GPIO 21` | I2C Data |
| **Left Click** | `GPIO 18` | Connect to GND when pressed (`INPUT_PULLUP`) |
| **Right Click** | `GPIO 19` | Connect to GND when pressed (`INPUT_PULLUP`) |

*(Update the GPIO numbers above to match your firmware!)*

---

## 💻 Software & Libraries Required

1. **Arduino IDE** (or PlatformIO) with the **ESP32 Board Package** installed.
2. **ESP32-BLE-Mouse** library by T-vK.
3. **Adafruit MPU6050** & **Adafruit Unified Sensor** libraries (or `I2Cdev` / `MPU6050`).

---

## 🚀 Setup & Usage

1. **Clone this repository:**
   ```bash
   git clone [https://github.com/abhib68/ESP32-MPU6050-Air-Mouse.git](https://github.com/abhib68/ESP32-MPU6050-Air-Mouse.git)
