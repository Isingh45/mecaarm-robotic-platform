# MecaArm Robotic Platform

## Overview

MecaArm is an STM32-based mobile robotic platform developed as the Senior Design Capstone project for **CMPE 492 / CMPE 493** at **California State University, East Bay**.

The platform integrates omnidirectional Mecanum-wheel locomotion, a multi-servo robotic arm, a custom four-layer PCB, embedded firmware, Bluetooth communication, and a mobile application into a complete robotics system.

The project demonstrates end-to-end embedded systems engineering by combining custom hardware design, firmware development, wireless communication, power electronics, and system-level validation.

---

## Technologies

* STM32F429VET6
* ESP32-WROOM-32
* C
* STM32 HAL
* STM32CubeMX
* Bluetooth (UART)
* PWM Motor Control
* Fusion 360 Electronics
* MIT App Inventor
* RT7258 Buck Regulators
* TB6612FNG Motor Drivers

---

## System Architecture

```text
MIT App Inventor Mobile App
             │
        Bluetooth
             │
      ESP32-WROOM-32
             │
      UART (115200 baud)
             │
      STM32F429VET6
      ┌───────────────┐
      │               │
      ▼               ▼
DC Motor Drivers   Servo Control
(TB6612FNG)        (PWM Timers)
      │               │
      ▼               ▼
Mecanum Drive     Robotic Arm
```

---

## Features

* **Custom Four-Layer PCB:** Designed a custom four-layer PCB centered around the STM32F429VET6 microcontroller with dedicated power distribution, motor drivers, communication interfaces, and debugging support.

* **Omnidirectional Mecanum Drive:** Controls four independently driven Mecanum wheels using PWM motor control and dual TB6612FNG motor drivers for omnidirectional robot movement.

* **Robotic Arm Control:** Controls a multi-servo robotic arm using STM32 hardware timers and PWM signals for coordinated actuator movement.

* **Bluetooth Wireless Communication:** Uses an ESP32 as a Bluetooth-to-UART bridge, allowing a custom MIT App Inventor mobile application to wirelessly control the robot.

* **Embedded Firmware:** Developed STM32 firmware using STM32 HAL to manage motor control, servo control, UART communication, and command processing.

* **Multi-Rail Power Architecture:** Designed dedicated power rails for motors, auxiliary peripherals, and logic circuitry to improve electrical stability and isolate high-current motor loads from sensitive electronics.

* **System Integration and Validation:** Successfully demonstrated integrated hardware, firmware, Bluetooth communication, mobile application control, robotic locomotion, and robotic arm operation.

---

## Repository Structure

```text
Documentation/
├── Final Project Report
└── Final Presentation

Hardware/
├── PCB Schematic
├── PCB Layout
├── Fusion 360 Design
├── Bill of Materials
└── Power Budget

Firmware/
├── STM32 Firmware
└── ESP32 Bluetooth Bridge

Mobile-App/
└── MIT App Inventor Application

Validation/
└── System Demonstration Video
```

---

## What I Learned

* Designing custom embedded hardware using a four-layer PCB.
* Developing embedded firmware with STM32 HAL and hardware timers.
* Implementing Bluetooth communication between mobile devices and embedded systems.
* Integrating power electronics, embedded software, wireless communication, and robotic actuators.
* Performing hardware bring-up, debugging, validation, and complete system integration.

---

## Future Improvements

* Add wheel encoder feedback for closed-loop motor control.
* Implement inverse kinematics for robotic arm positioning.
* Integrate ROS 2 for higher-level robot control.
* Add onboard sensors for autonomous navigation.
* Expand the platform with additional perception modules.

---

## Institution

**California State University, East Bay**

**Course:** CMPE 492 / CMPE 493 – Senior Design Capstone (2025–2026)

---

## Authors

* Inderpal Singh
* Sukhpinder Singh
* Feranmi Falodun
* Pierreline Jacob
