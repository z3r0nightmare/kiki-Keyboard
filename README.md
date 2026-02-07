# Kiki v1 ⌨️

Kiki v1 is a modernized, high-performance split mechanical keyboard. This design is inspired by the **Corne v4.1 (Cherry Version)** but optimized for the **RP2040** processor. It features integrated MCU support, dual rotary encoders per side, and native **Vial** compatibility for real-time configuration.

---

## 📂 Repository Contents
* **/Hardware**: Gerber files, PCB designs, and BOM (Bill of Materials). Optimized for **NextPCB** assembly.
* **/Firmware**: Compiled `.uf2` files and QMK/Vial source code.
* **/Case**: STL files for 3D printing and CAD models for custom enclosures.

---

## 🛠 Hardware Build & Assembly
This PCB integrates the Raspberry Pi RP2040 directly onto the board, eliminating the need for separate Pro Micro controllers.

### 1. PCB Manufacturing
The files in the `/Hardware` folder are optimized for the **NextPCB** workflow. By using their assembly service with the provided **BOM** and **CPL** files, you can receive your boards with all SMD components (MCU, diodes, resistors) pre-soldered.

### 2. Rotary Encoders
The Kiki v1 supports dual encoders per side for maximum control. Note that firmware updates are ongoing to further optimize pin assignments; always ensure you are flashing the latest `.uf2` from the `/Firmware` folder to keep your hardware features fully active.

---

## 🚀 Software & Customization

### 1. Vial Support (Real-time Edits)
The Kiki v1 is **Vial-ready**, allowing you to change your layout, RGB effects, and encoder behavior without ever touching a line of code.
* **Download**: [vial.today](https://get.vial.today/)
* **Usage**: Plug in your keyboard, open the Vial app, and start remapping.
* **Reset**: If the layout visuals appear incorrectly in the app, navigate to `Security -> Reset to Factory Defaults` in the Vial menu to refresh the coordinate map.

### 2. Layout Options
The firmware supports multiple physical configurations:
* **3x6_3**: Standard 6-column experience.
* **3x5_3**: Compact 5-column layout for minimal finger travel.

### 3. OLED & Bongo Cat
The integrated OLED displays feature a reactive **Bongo Cat** animation. The cat's typing speed scales with your WPM (Words Per Minute), and the screen also displays your current layer and last key pressed.



---

## ⚡ How to Flash
1. Hold the **BOOT** button on the PCB while plugging in the USB-C cable.
2. A drive named `RPI-RP2` will appear on your computer.
3. Drag and drop the provided `.uf2` file onto that drive.
4. The keyboard will automatically reboot and be ready to use.

---

## 🎨 Credits & Inspiration
* **Base Inspiration**: Inspired by the **Corne (Crkbd) v4.1 Cherry** by foostan.
* **Firmware Framework**: Powered by [QMK Firmware](https://qmk.fm/) and [Vial](https://get.vial.today/).
* **Optimizations**: Custom RP2040 pinout integration and dual-encoder support.

---

## 📜 License
Open-source for personal use. If you build a Kiki v1 or feature it in a project, please link back to this repository!
