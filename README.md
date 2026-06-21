# MecaArm Robotic Platform

An STM32-based mobile manipulation platform featuring omnidirectional Mecanum-wheel locomotion, a multi-degree-of-freedom robotic arm, custom PCB hardware, embedded firmware, Bluetooth communication, and mobile-app control.

Senior Design Capstone Project
California State University, East Bay
CMPE 492 / CMPE 493 (2025–2026)

---

## Overview

MecaArm is a custom mobile robotic platform designed to provide direct access to embedded control, hardware interfaces, and system integration without relying on proprietary robotics controllers.

The project replaces vendor electronics with a custom STM32-based control board that integrates locomotion, arm actuation, wireless communication, sensing interfaces, and power management into a single embedded system.

The platform combines:

* Omnidirectional Mecanum-wheel drive
* Multi-joint robotic arm control
* Custom 4-layer PCB design
* STM32 embedded firmware
* ESP32 Bluetooth bridge
* MIT App Inventor mobile application
* Multi-rail power architecture
* End-to-end system integration and validation

---

## System Architecture

Hardware Components:

* STM32F429VET6 Microcontroller
* ESP32-WROOM-32 Bluetooth Bridge
* TB6612FNG Motor Drivers
* RT7258 Buck Converters
* LSM6DSR IMU
* Multi-servo robotic arm
* Four-wheel Mecanum drive platform
* Custom 4-layer PCB

Power Architecture:

* 7.4V LiPo Battery
* Dedicated high-current servo rail
* Independent 5V motor rail
* Independent 5V auxiliary rail
* 3.3V logic rail

The separated power rails were implemented to isolate motor loads from sensitive logic and communication circuitry, improving system stability during dynamic operation.

---

## Key Features

### Omnidirectional Locomotion

Four independently controlled Mecanum wheels enable:

* Forward and reverse movement
* Lateral translation
* In-place rotation

### Robotic Arm Control

Multi-joint robotic arm controlled through STM32-generated PWM signals with Bluetooth command input from a mobile application.

### Wireless Mobile Control

Control path:

Mobile App → Bluetooth → ESP32 → UART → STM32 → Motors & Servos

### Custom PCB Hardware

Custom 4-layer PCB designed, fabricated, assembled, debugged, and validated as part of the project lifecycle.

---

## Contributions

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

* STM32 firmware development and integration
* Motor control implementation
* Bluetooth communication integration
* Embedded system validation and testing

### System Integration

* End-to-end platform integration
* Hardware and firmware debugging
* Demonstration preparation
* Validation testing

---

## Repository Contents

### Documentation

* Final technical report
* Final project presentation

### Hardware

* Schematic files
* PCB layout files
* Fusion design files
* Power budget analysis
* Bill of Materials

### Firmware

* STM32 embedded firmware
* ESP32 Bluetooth bridge firmware

### Mobile App

* MIT App Inventor project source

### Validation

* End-to-end demonstration video

---

## Results

The completed platform successfully demonstrated:

* Bluetooth communication
* Mobile application control
* STM32 command processing
* Mecanum-wheel locomotion
* Multi-servo robotic arm actuation
* Stable multi-rail power operation
* Full-system integration

The project validated a complete embedded robotics workflow spanning hardware design, firmware development, power systems, communication interfaces, and system integration.

---

## Future Improvements

Potential future enhancements include:

* Closed-loop wheel velocity control
* Joint feedback integration
* Inverse kinematics
* Autonomous navigation
* ROS 2 integration
* Improved PCB thermal design
* Cost optimization for future revisions

---

## Technologies

Hardware:

* STM32F429VET6
* ESP32-WROOM-32
* RT7258
* TB6612FNG

Firmware:

* C
* STM32 HAL
* STM32CubeMX

Software:

* MIT App Inventor

Tools:

* Fusion 360 Electronics
* Embedded Debugging Tools
* Oscilloscope Validation
* PCB Manufacturing Workflow
