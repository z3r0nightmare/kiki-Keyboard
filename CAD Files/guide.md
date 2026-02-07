# Kiki v1: 3D Printing & CAD Guide 🛠️

This folder contains the structural components for the Kiki v1. The design is optimized for the **Corne v4.1 Cherry** form factor but adapted for integrated RP2040 components.

## 📁 File Descriptions
* **`Case_Top.stl`**: The main bezel for the switch plate.
* **`Case_Bottom.stl`**: The base enclosure. Includes cutouts for the USB-C port and OLED.
* **`Kiki_v1_Full_Assembly.step`**: Use this CAD file if you want to modify the design in Fusion 360, Blender, or FreeCAD.

## 🖨️ Printing Recommendations
* **Material**: PLA for standard builds; PETG or ABS if you want more heat resistance.
* **Infill**: 20% or higher for a solid "thocky" sound.
* **Supports**: Required for the USB-C port opening and the OLED window.
* **Layer Height**: 0.2mm is standard, but 0.16mm will give the curves a smoother finish.

## 🛠️ Post-Processing
1. Remove support material carefully around the MCU area.
2. Use M2 or M3 screws (check your specific PCB holes) to secure the PCB to the bottom case.
