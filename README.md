# 🤖 Robotic_ARM-CYB

> A modular stepper-motor robotic arm prototype developed at CYBORG (The Official Robotics and Automation Club of NIT Rourkela).

---

## 📸 Project Gallery

### 🦾 Final Assembly
<p align="center">
  <img src="assets/robotic_arm_full.jpg" width="600"/>
</p>

### 🔌 Custom PCB
<p align="center">
  <img src="assets/pcb_top.jpg" width="400"/>
  <img src="assets/pcb_bottom.jpg" width="400"/>
</p>

### 🧠 Electronics Setup
<p align="center">
  <img src="assets/electronics_setup.jpg" width="600"/>
</p>

### 🎮 Joystick Control Testing
<p align="center">
  <img src="assets/joystick_test.jpg" width="600"/>
</p>

---

## Overview

Our **Robotic_ARM** is a multi-axis robotic arm prototype built with:

- Precision stepper motor control  
- TMC2209 UART configuration  
- Motion control logic & basic inverse kinematics  
- Custom PCB design  
- Mechanical prototyping and tolerance validation  

The system is based on an **ESP32-class microcontroller** driving multiple **TMC2209 stepper motor drivers** using **STEP/DIR pulses** with UART-based configuration.

---

## System Architecture

<p align="center">
  <img src="assets/system_architecture.png" width="700"/>
</p>

- **Microcontroller:** ESP32 dev board  
- **Motor Drivers:** TMC2209 (UART + STEP/DIR)  
- **Motors:** NEMA17 Stepper Motors  
- **Input Device:** 2-axis Analog Joystick  
- **Control Method:** STEP/DIR pulse generation + UART configuration  
- **Power:** External motor power supply with current limiting  

---

## Features

### Joystick Motion Control
- 2-axis real-time motor control
- Deadzone filtering
- Speed mapping based on joystick deflection

### Motion Experiments
- Constant-speed rotation tests
- Periodic motion patterns
- Maximum RPM testing
- Multi-motor synchronization

### Motion Primitives
- Straight line movement (step conversion math)
- Rectangle drawing demo
- Basic planar inverse kinematics (experimental)

### Smart Driver Configuration (TMC2209)
- RMS current configuration
- Microstepping setup
- StealthChop tuning
- UART address-based multi-driver setup


