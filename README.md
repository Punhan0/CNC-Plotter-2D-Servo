# 2D CNC Plotter with Arduino & GRBL (Servo Supported)

A DIY 2D CNC Plotter project built with **Arduino Uno**, modified **GRBL firmware**, and **28BYJ-48 stepper motors**. This plotter features a custom mechanical frame and a pen-lifting mechanism.

## ✨ Features
* **X-Y Axis:** Driven by 28BYJ-48 Stepper Motors (Unipolar).
* **Z-Axis:** Pen lift controlled by an SG90 Servo motor.
* **Firmware:** Custom GRBL optimized for 28BYJ-48 and Servo support.
* **Frame:** Lightweight chassis built using **wooden sticks** (DIY approach).

## 🏗️ Mechanical & Software Design
* **Mechanical Structure:** The frame is constructed from wooden sticks, demonstrating an affordable DIY engineering solution.
* **Software Workflow:** 1. Design created in **Inkscape**.
    2. G-code generated using specialized Inkscape plugins.
    3. Streamed to Arduino via **Universal Gcode Sender (UGS)**.

## 🛠️ Hardware Components
* **Microcontroller:** Arduino Uno
* **Motors:** 2x 28BYJ-48 Stepper Motors
* **Drivers:** 2x ULN2003 Driver Boards
* **Servo:** SG90 Micro Servo

## 🔌 Wiring & Pinout
To make the system work with the 28BYJ-48 motors and the Servo, use the following pin configuration:

* **X-Axis (Stepper):** Connected to Digital Pins `2, 3, 4, 5`.
* **Y-Axis (Stepper):** Connected to Analog Pins `A0, A1, A2, A3`.
* **Z-Axis (Servo):** Connected to Digital Pin `11`.

## 📜 Credits and References
This project is a modified version based on existing open-source work. Special thanks to the creators whose code and tools helped build this project:

* **Original GRBL Firmware:** (https://github.com/grbl/grbl) - The official open-source high-performance G-code parser.
* **Inkscape G-Code Extension:** (https://github.com/arpruss/gcodeplot/releases) - Used for converting vector graphics to G-code.
* **Modified Firmware by:** (https://github.com/ruizivo/GRBL-28byj-48-Servo)
* **My Contribution:** I identified and fixed several bugs in the original code, designed and built the entire physical chassis using wooden sticks, and successfully integrated the Servo-based Z-axis control.
