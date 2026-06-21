# MecaArm Robotic Platform

An STM32-based mobile robotic platform featuring omnidirectional Mecanum-wheel locomotion, a multi-servo robotic arm, custom PCB hardware, Bluetooth communication, and mobile-app control.

Senior Design Capstone Project
California State University, East Bay
CMPE 492 / CMPE 493 (2025–2026)

---

## Overview

MecaArm is a custom embedded robotics platform developed as a senior design capstone project. The project replaces vendor control electronics with a custom STM32-based control board, providing direct access to embedded hardware, motor control, communication interfaces, and power management.

The platform combines hardware design, embedded firmware development, Bluetooth communication, mobile-app integration, and system-level validation into a single robotics platform.

---

## Key Features

### Custom 4-Layer PCB

Designed, fabricated, assembled, and validated a custom 4-layer PCB centered around the STM32F429VET6 microcontroller.

Features include:

* Multi-rail power architecture
* Motor driver integration
* Servo interfaces
* Bluetooth communication interface
* Expansion support for future sensor integration
* Debug and programming interfaces

### Embedded Control System

The STM32 firmware provides:

* PWM motor control
* Servo control
* UART communication
* Bluetooth command processing
* Real-time actuator control

An ESP32 module serves as a Bluetooth-to-UART bridge between the mobile application and the STM32 controller.

### Mobile Application Control

A custom MIT App Inventor application enables wireless control of:

* Mecanum-wheel locomotion
* Robotic arm movement
* System operation through Bluetooth communication

### Multi-Rail Power Architecture

The platform utilizes a dedicated power distribution architecture:

* 7.4V battery rail
* Independent 5V motor rail
* Independent 5V auxiliary rail
* Dedicated 3.3V logic rail

This separation helps isolate high-current motor loads from sensitive logic circuitry and communication interfaces.

---

## Demonstrated Functionality

The completed system successfully demonstrated:

* Bluetooth communication
* Mobile application control
* ESP32-to-STM32 communication
* Mecanum-wheel movement
* Multi-servo robotic arm control
* Custom PCB operation
* Stable multi-rail power delivery
* End-to-end hardware and firmware integration

---

## System Architecture

```text
Mobile App
     ↓
Bluetooth
     ↓
ESP32 Bridge
     ↓
UART
     ↓
STM32F429VET6
     ↓
Motors + Servos
```

---

## My Contributions

### Hardware Engineering

* Schematic capture support
* PCB layout support
* Power architecture design
* RT7258 regulator integration
* Power budget analysis
* Decoupling strategy implementation
* Manufacturing preparation
* Hardware bring-up support
* Power validation and debugging

### Embedded Systems

* STM32 firmware contribution
* Motor-control implementation support
* Bluetooth communication integration
* Embedded system testing and validation

### System Integration

* Hardware and firmware integration
* Platform validation
* Demonstration testing
* End-to-end system verification

---

## Repository Structure

```text
Documentation/
├── Final Report
└── Final Presentation

Hardware/
├── Schematic Files
├── PCB Layout Files
├── Fusion Design Files
├── Power Budget
└── Bill of Materials

Firmware/
├── STM32 Firmware
└── ESP32 Bluetooth Bridge

Mobile-App/
└── MIT App Inventor Project

Validation/
└── Demonstration Video
```

---

## Technologies

### Hardware

* STM32F429VET6
* ESP32-WROOM-32
* RT7258 Buck Converters
* TB6612FNG Motor Drivers
* Mecanum Drive Platform
* Multi-Servo Robotic Arm

### Software & Firmware

* C
* STM32 HAL
* STM32CubeMX
* UART Communication
* Bluetooth SPP

### Development Tools

* Fusion 360 Electronics
* MIT App Inventor
* ST-Link Debugging Tools

---

## Notes

The custom PCB includes provisions for future expansion, including sensor and peripheral interfaces. While these interfaces were incorporated into the hardware design, the final demonstrated system focused on locomotion, robotic arm control, Bluetooth communication, embedded control, and full-system integration.

---

## Project Team

* Inderpal Singh
* Sukhpinder Singh
* Feranmi Falodun
* Pierreline Jacob

California State University, East Bay
Department of Engineering
