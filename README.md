# Analog PWM LED Controller
A hardware-defined Pulse Width Modulation (PWM) generator designed for flicker-free LED dimming without a microcontroller.

## Project Demo
[![Watch the Demo](https://img.youtube.com/vi/0v9D-uy3l6E/0.jpg)](https://www.youtube.com/watch?v=0v9D-uy3l6E)

## Project Overview
This project focuses on the design and implementation of a variable-duty-cycle PWM controller using an **NE555 timer**. By utilizing steering diode logic, the circuit achieves independent control over the charge and discharge paths of a timing capacitor, allowing for a wide range of brightness control.

### Key Technical Features
- **Variable Duty Cycle:** Achieved a stable output range of **5% to 95%** using a 100kΩ potentiometer.
- **Steering Diode Logic:** Implemented 1N4007 diodes to isolate charging and discharging paths, ensuring linear control over the PWM signal.
- **Simulation-Driven Design:** Validated all timing transients and component stresses in **LTspice** prior to physical assembly.
- **Circuit Stability:** Integrated a **1kΩ protection resistor** to maintain timing stability and protect the IC during high-frequency discharge cycles.

## Technical Specifications
- **Core Component:** NE555 Precision Timer
- **Timing Components:** 10 nF Ceramic Capacitor, 100kΩ Potentiometer
- **Diodes:** 1N4007 High-speed Steering Diodes
- **Power Supply:** 9V DC
- **Validation Tools:** LTspice (Simulation), Digital Multimeter (Hardware Testing)

## Repository Contents
- **Simulation:** LTspice `.asc` schematic and transient analysis plots.
- **Schematics:** Detailed wiring diagrams and component-level layouts.
- **Images:** Screenshots comparing simulated waveforms vs. physical breadboard measurements.

---
Independent Project by Dylan Nguyen | Electrical Engineering student at UC Santa Cruz
