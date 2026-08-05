# Embedded Washing Machine Microcontroller Programming Project

## Overview

This project was completed as part of my first year in Electronic and Electrical Engineering at the University of Leeds.

I designed and implemented a simulated washing machine control panel using an STM32L476RG Nucleo-64 development board. The project combined embedded software development with hardware design, requiring both the physical construction of the control circuit and the implementation of the control logic in C++, as well as critical thinking to address potential limitations and ethical engineering. 

## My Contributions

For this project I:

- Designed and assembled the hardware circuit using the required electronic components.
- Developed the embedded software in C++.
- Programmed the control logic for the washing machine operation.
- Integrated hardware inputs and outputs with the software.
- Tested and debugged the complete embedded system.
- Wrote a lab journal evaluating my project and limitations I faced. 

## Features

### Power Control

- Push-button power control
- Start-up and shutdown melodies using a PWM buzzer
- LED power status indication

### Wash Cycle Selection

Four selectable wash programmes:

- Delicate
- Cotton
- Heavy Duty
- Quick Wash

Cycle selection is performed using an analogue potentiometer and displayed using:

- RGB LED
- Seven-segment display
- Serial interface

---

### Temperature Selection

Three selectable temperatures:

- 40°C
- 50°C
- 60°C

Visual feedback is provided through LEDs together with numerical output on the seven-segment display.

---

### Load Detection

An FSR sensor measures the simulated washing load.

The controller prevents operation when the load is outside acceptable limits and automatically retries before requesting a manual reset.

---

### Door Safety System

An LDR sensor simulates door detection.

The washing cycle cannot begin until the door is safely closed.

---

### Cycle Execution

The washing process progresses through multiple stages.

The RGB LED indicates:

- Wash
- Rinse
- Drain

The seven-segment display acts as a countdown timer while the serial monitor continuously reports system status.

---

### Emergency Stop

A dedicated emergency stop button immediately terminates the washing cycle and safely resets the controller.

---

## Hardware

- STM32L476RG Nucleo-64
- RGB LED
- LEDs
- Seven-segment display
- Potentiometers
- Force Sensitive Resistor (FSR)
- Light Dependent Resistor (LDR)
- PWM Buzzer
- Push buttons
- Breadboard prototype

---

## Software

- C++
- Mbed OS

---

## Skills Demonstrated

- Embedded software development
- C++ programming
- Embedded hardware integration
- Analogue and digital interfacing
- PWM control
- Serial communication
- State-machine design
- Sensor integration
- Embedded debugging
- System testing

---

## Project Images

Includes:

- Circuit overview
- Hardware prototype
- System architecture
- State diagram


---

## Future Improvements

Potential future developments include:

- LCD display
- EEPROM configuration storage
- Interrupt-driven architecture
- Non-blocking timers
- Additional wash programmes
- Mobile application interface
