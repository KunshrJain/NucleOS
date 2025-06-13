# NucleOS

**NucleOS** is a lightweight, pseudo-bare-metal operating system built specifically for a range of embedded platforms including **ESP32**, **STM32**, **Arduino-compatible boards**, and **Raspberry Pi**. Designed with minimalism and embedded development in mind, it strips away traditional RTOS overhead and gives you direct control over hardware — while still providing a usable kernel, simple GUI, and built-in application support.

---

## 🚀 Overview

- 🧠 **Pseudo-Bare-Metal Core:** No FreeRTOS or bloated frameworks. NucleOS boots with custom startup code and your own kernel logic.
- 🌐 **Wi-Fi Kernel Support:** Built-in low-weight networking support for ESP32 modules.
- 🖥️ **GUI Stack:** Basic kernel GUI and optional user-facing GUI for simple embedded displays.
- 🧩 **Modular Applications:** Includes base apps like a file explorer, system viewer, and support for integrating custom apps like an embedded ChatGPT UI.
- 💡 **Fully Hackable:** Designed for total code control and deep customization.

---

## 🛠 Features

| Feature                      | Description |
|-----------------------------|-------------|
| 🔧 Custom Bootloader        | Your code runs first — no hidden RTOS layers. |
| 🌐 Wi-Fi Kernel Support     | Lightweight integration of ESP32’s wireless stack. |
| 🖼️ GUI Support              | Basic graphical layers for embedded displays. |
| 📁 System Applications      | Explorer, shell interface, and basic tools. |
| 🤖 Chatbot Embedding        | Add your own LLM UI or chatbot client. |
| 💻 Dev Environment          | Compatible with Linux and Windows. |
| 📦 Cross-Platform Support   | Works on ESP32, STM32, Arduino-compatible boards, and Raspberry Pi. |
| 🔌 Embedded Friendly        | Small memory footprint, efficient runtime. |
| 🧪 Extendable Base          | Build your own apps, drivers, or kernel modules. |

---

## 🧰 Platform & Tools

- **Supported Chips & Boards:**  
  - ESP32 (WROOM, WROVER, S2, S3, C3)  
  - STM32 series  
  - Arduino-compatible microcontrollers  
  - Raspberry Pi (various models)

- **Toolchains:**  
  - `xtensa-esp32-elf-gcc` and ESP-IDF 5.x for ESP32  
  - ARM GCC toolchains for STM32 and Raspberry Pi  
  - Arduino IDE / PlatformIO support for Arduino boards

- **Flashing Tools:**  
  - `esptool.py` for ESP32  
  - STM32CubeProgrammer or OpenOCD for STM32  
  - Raspberry Pi bootloader / SD card flashing

- **Build Systems:**  
  - `idf.py` for ESP32  
  - CMake / Makefiles for STM32 and Raspberry Pi  
  - Arduino build system support

---

## 📂 Project Structure

nucleos/
├── components/ # Optional: stripped ESP-IDF components
├── core/ # Custom kernel, scheduler, and init code
│ ├── start.S # Low-level startup entry point
│ └── main.c # First C function (main)
├── gui/ # Kernel GUI and user interface layers
├── apps/ # Embedded applications (explorer, tools)
├── ports/ # Platform-specific code and startup files (esp32, stm32, rpi, arduino)
├── CMakeLists.txt # IDF-compatible project definition (esp32)
├── Makefile # Optional manual build system
├── link.ld # Custom linker script
├── LICENSE # MIT License
└── README.md # This file


---

## 🧑‍💻 About the Author

**NucleOS** was created and developed by **Kunsh Jain**, with a passion for bare-metal systems, embedded simplicity, and open development.

> **If you use or modify the low-level kernel, boot, or startup code, attribution to Kunsh Jain is required as part of the MIT license.**

---

## 📄 License

This project is licensed under the **MIT License**.  
You're free to use, modify, and distribute this code in your own projects — just **credit the author** if you use the bare-metal core, kernel, or startup code.

See [`LICENSE`](./LICENSE) for details.

---

## 📣 Contributions & Support

Pull requests, feature ideas, and improvements are welcome.  
If you're using NucleOS in a project, let the author know — we’d love to hear about it!

---

> ⚡ Designed to be minimal. Built to be powerful.  
> Welcome to **NucleOS**.
