# NucleOS — Arduino Port

**NucleOS** for Arduino-compatible boards is a lightweight pseudo-bare-metal operating system designed to give you more direct control over Arduino hardware beyond the standard Arduino runtime.

---

## 🚀 Overview

- 🧠 **Bare-Metal Inspired:** Runs with minimal runtime overhead, offering more flexibility than the standard Arduino core.
- 🛠 **Custom Startup:** Uses your own startup and kernel code to replace or augment the Arduino boot process.
- 🖥️ **Basic GUI Support:** Lightweight graphical UI layer compatible with common Arduino display shields.
- 📦 **Modular Apps:** Includes simple built-in apps like file explorers and system utilities.
- 🌐 **Expandable:** Easily add networking and other features with compatible Arduino libraries.
- ⚙️ **Development:** Fully compatible with the Arduino IDE and PlatformIO.

---

## 🛠 Features

| Feature                    | Description                                |
|---------------------------|--------------------------------------------|
| 🔧 Custom Startup         | Replace Arduino’s default boot sequence.  |
| 🖼️ GUI Layer             | Basic graphics for LCD/OLED displays.     |
| 📁 System Applications    | Explorer, shell interface, simple tools.  |
| 🌐 Arduino Library Compatible | Use existing Arduino libraries for Wi-Fi, sensors, etc. |
| 💡 Small Footprint       | Efficient code ideal for low-resource MCUs.|

---

## 🧰 Supported Boards

- Arduino Uno (ATmega328P)  
- Arduino Mega  
- Arduino Nano  
- Other AVR-based Arduino-compatible boards (support may vary)  

*Note: ARM-based Arduino boards (e.g. Arduino Due) support planned.*

---

## 🛠 Development Setup

- **IDE:** Arduino IDE or PlatformIO  
- **Programming Language:** C / C++  
- **Build:** Upload through standard Arduino tools  
- **Debug:** Serial monitor for logs and debug output

---

## 📂 Project Structure (Arduino Port)

nucleos/
├── ports/
│ └── arduino/
│ ├── start.S # Custom startup assembly (if applicable)
│ ├── main.cpp # Entry point with NucleOS kernel
│ ├── gui/ # GUI code compatible with Arduino displays
│ ├── apps/ # Built-in applications
│ └── libraries/ # Additional Arduino-compatible libs


---

## 🧑‍💻 About the Arduino Port

This port is maintained by **Kunsh Jain** and designed to give Arduino users a powerful, lightweight OS alternative that allows more control and modularity than the stock Arduino runtime — all while keeping the ease of use of the Arduino ecosystem.

---

## 📄 License

NucleOS Arduino port is licensed under the **MIT License**.  
Please attribute **Kunsh Jain** if you reuse or redistribute bare-metal or kernel-level code.

---

## 🚀 Getting Started

1. Clone or download the NucleOS repo.  
2. Open the Arduino port folder in your IDE.  
3. Build and upload to your Arduino board.  
4. Explore sample applications and GUI demos included.

---

> Ready to break out of Arduino's limitations?  
> Dive into **NucleOS Arduino** and build embedded projects your way!
