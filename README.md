# 📖 ePUB Reader with E-Ink Display - AM-EPUBR-R1

A **compact handheld device** designed for reading books in **ePUB format**, powered by an **ESP32** and featuring an **e-ink display** for a paper-like reading experience.  
It includes **native USB file transfer**, an **SD card slot**, **Li-Po battery power**, and a **rotary encoder** for smooth navigation.  

---

## ✨ Features
- ✅ Supports **ePUB format**
- ✅ **Native USB** file transfer for loading books
- ✅ **SD card storage** for your library
- ✅ Powered by a **Li-Po battery** for portability
- ✅ **Compact PCB** with custom design
- ✅ **Rotary encoder** for intuitive UI control
- ✅ Designed with **KiCAD**, **Fusion 360**, and **VS Code**

---

## 🔧 Feature Description

This device combines multiple subsystems to create a compact, battery-powered **ePUB reader** with USB file transfer and SD storage.  
Below is an overview of the main components and their roles:

- **ESP32-S3-WROOM-1** → The core microcontroller, handling ePUB processing, display control, and USB/SD communication.  
- **AP61100Z6-7** → High-efficiency step-down DC/DC regulator, providing stable 3.3V power to the system.  
- **BQ24040DSQR** → Li-Po battery charger and power-path management IC.  
- **JST PH 2.0 Connector** → Battery input for the Li-Po cell.  
- **USB_C_Receptacle_USB2.0_16P** → Main USB interface for file transfer, charging, and firmware upload.  
- **USB to TTL header (6-pin)** → Debug/programming interface for ESP32.  
- **AP22804AW5** → Power distribution switch, protecting USB and system power paths.  
- **USBLC6-2SC6** → ESD protection for USB data lines.  
- **SI1308EDL** → P-channel MOSFET for load switching/power management.  
- **74LVC125APW** → Quad buffer/line driver for logic level shifting and signal integrity.  
- **24-pin Display Connector** → E-Ink display interface (data, control, power).  
- **SIQ-02FVS3 Rotary Encoder** → User input for page turning and navigation.  
- **BMA400** → Low-power 3-axis accelerometer (e.g., auto screen rotation, device orientation).  
- **Micro SD Card slot (Det1)** → External storage for ePUB files.  

Each component contributes to a **modular and power-efficient design** that balances portability, usability, and robustness.


---

## 📂 Repository Contents
- `/docs` → PDF schematic, PCB outline, and component placement  
- `/firmware` → ESP32 firmware code  
- `/3d` → Fusion 360 and KiCAD exports  
- `/images` → Project renders, schematics, and board previews  

---

## 🖼️ Project Gallery

### 📱 Device Concept Render
![ePUB reader 3D](images/ePUB%20reader%203D%20render.PNG)

### 📐 Schematic
![Schematic](images/Schematic.png)

### 🖤 PCB Layout
**Top view**  
![PCB TOP](images/PCB%20TOP.png)  

**Bottom view**  
![PCB BOT](images/PCB%20BOT.png)

### 🛠️ 3D PCB Render
![PCB 3D](images/PCB%203D.png)

---

## 🧱 Hardware block diagram
![ePUB reader with e-ink display block diagram](docs/ePUB%20reader%20with%20e-ink%20display%20block%20diagram.png)

---

## 🚀 How to Use
1. Open `/docs` to view the circuit schematic, PCB outline, and component placement.  
2. Replicate the PCB design using the provided documentation.  
3. Build and flash the firmware in **VS Code (ESP-IDF)** or **Arduino IDE** for the ESP32.  
4. Upload your favorite books via USB or SD card.  
5. Enjoy reading on your **custom-built ePUB reader** 📚✨  

---

## 🎯 Purpose
This is a **personal build project** intended as a DIY hardware showcase.  
The schematic and PCB layout are provided **for reference and inspiration only**.  

---
