# Advance Thermo-Resistive Fire Detection and Alert System

> a simple fire alarm, entirely done using analog electronics, without the use of any microcontroller – for once, the classic methods do work!

---

## What's This About?

The project was made during the 2nd semester of B.Tech Electrical Engineering in the course **“Electronic Devices & Circuits”** (EC108), while studying in **SVNIT Surat**. The basic concept was to build a device that detects the increase in temperature and screams (literally, buzzes) about it.

No Arduino. No coding. Just pure old analog electronics!
---

## The Team

- **Nishant Tiwari**
- **Jyotirmoi Biswas**

**Timeline:** March – April 2026

---

## How Does It Actually Work?

In the middle of this system, an **NTC thermistor** acts as a major part – a component whose resistivity decreases when there's any rise in temperature. We used this basic behavior for alarming us.

Here's the sequence in understandable terms:

1. No fire → high resistance of thermistor → transistor remains off → no alarm generated.
2. Fire or heat in vicinity → low resistance of thermistor → high current towards the base of transistor → transistor on → **buzzer activated + LED turns on**.
3. A potentiometer controls sensitivity in the circuit and sets alarm threshold accordingly.

That's it. No firmware to flash, no libraries to install.

---

## Circuit Diagram

![Circuit Diagram](circuit_diagram.jpg)

---

## Development Process

The circuit was first tested on a breadboard and later soldered onto a General Purpose PCB (Perfboard) for permanent implementation.

| Breadboard Prototype | Final PCB (Build 1) | Final PCB (Build 2) |
|---|---|---|
| ![Prototype](photos/prototype.jpg) | ![PCB Build 1](photos/pcb_build_1.jpg) | ![PCB Build 2](photos/pcb_build_2.jpg) |

---

## Components Used

| Component | Quantity |
|---|---|
| BC547 NPN Transistor | 1 |
| NTC Thermistor (10 kΩ) | 1 |
| 10 kΩ Potentiometer | 1 |
| 220 Ω Resistor | 1 |
| Piezo Buzzer | 1 |
| Red LED | 1 |
| 9V Battery & Clip | 1 |
| General Purpose PCB (Perfboard) | 1 |

---

## What We Learned

Indeed, there is much that we learned that went beyond what we imagined when we started the project:

- About the performance characteristics of NTC sensors under varying temperatures (and their application in sensor design)
- How to use a BC547 transistor as a switch instead of an amplifier
- Practical skills in soldering circuit elements on to a board without killing them
- About how to debug a circuit when it does not seem to work right off the bat
- The experience of creating a safety system from scratch

---

## Where Can This Go From Here?

We made it easy for our coursework purposes, however, there is great potential for making this project into a full-fledged one:

- **Attach a MQ-2 smoke sensor** – sense real smoke, not temperature only
- **Throw in an Arduino microcontroller** – for intelligent handling, threshold setting, logging
- **Put an LCD/OLED screen** – display the temperature on the go
- **Make it IoT** – receive notifications to your mobile whenever the fire gets going
- **Battery monitor** – detect when you need to recharge the board

---

## Acknowledgements

Big thanks to our course instructors and the lab staff at SVNIT Surat for their patience, guidance, and for letting us use the equipment. This wouldn't have come together without their support.

---

*Built with resistors, solder, and a healthy fear of fire *
