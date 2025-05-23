# Precision-Amplifier-Circuit-CD4056-OPAmp
A project demonstrating a precision amplifier circuit using OP07 operational amplifiers and the CD4052 multiplexer. The circuit is designed for flexible amplification with selectable gain.


## Table of Contents

* [Overview](#overview)
* [Features](#features)
* [Schematic Diagram](#schematic-diagram)
* [Component List](#component-list)
* [Working Principle](#working-principle)
* [Power Supply Options](#power-supply-options)
* [Build Instructions](#build-instructions)
* [Testing the Circuit](#testing-the-circuit)
* [Optional Add-ons](#optional-add-ons)
* [Applications](#applications)
* [Viva Questions](#viva-questions)
* [Gallery](#gallery)
* [References](#references)

---

## Overview

This project demonstrates a precision amplifier circuit using OP07 operational amplifiers and the CD4052 multiplexer. It is designed to amplify small analog input voltages, such as those from temperature sensors like LM35, with high accuracy and flexibility.

---

## Features

* Selectable gain levels using switches
* High input impedance
* Low offset voltage using OP07
* MUX-based signal routing for flexible amplification
* Breadboard and PCB compatible

---

## Schematic Diagram



---![Screenshot 2025-02-24 112616](https://github.com/user-attachments/assets/cbbd6811-0577-428e-9ddb-b40fff2b1899)


## Component List

| Component       | Specification       | Quantity |
| --------------- | ------------------- | -------- |
| OP07            | Precision Op-Amp    | 4        |
| CD4052          | Dual 4-to-1 MUX     | 1        |
| LM35            | Temperature Sensor  | 1        |
| Resistors       | 10k, 100k, etc.     | 10+      |
| Capacitors      | 0.1μF, 1nF          | 3        |
| Zener Diode     | 4.7V                | 2        |
| 7805 Regulator  | Voltage Regulator   | 1        |
| Switches        | Toggle or DIP       | 2        |
| LEDs (optional) | Red/Green Indicator | 3-5      |
| 9V Battery      | or USB supply       | 1        |

---

## Working Principle

The input voltage from LM35 is fed into the amplifier stages built using OP07 op-amps. A CD4052 multiplexer is used to select different gain paths by changing the input resistance. This allows for dynamic control of amplification. The amplified output is available at output terminals CON3 and CON4.

---

## Power Supply Options

* **9V Battery + 7805 Regulator**: Most stable method
* **Arduino 5V Pin**: Only if current draw is low
* **Mobile Charger via Regulator**: Can be used with USB breakout

---

## Build Instructions

1. Place all components on a breadboard/PCB
2. Connect OP07 op-amps in standard inverting/non-inverting config
3. Wire CD4052 for gain control using switches
4. Add decoupling capacitors (0.1μF) near ICs
5. Insert LM35 at CON2 and switches at SW1/SW2
6. Connect 7805 to 9V battery for regulated power
7. Connect multimeter to output pins to observe voltage

---

## Testing the Circuit

* Use LM35 to generate an analog voltage (\~10mV/°C)
* Connect multimeter at CON3
* Observe amplified output voltage
* Change switch positions to alter gain

---

## Optional Add-ons

* **LED Indicators**: At output of each OP07 to show signal flow
* **LCD/7-segment Display**: Show amplified voltage
* **Buzzer**: Alert on high temp from LM35

---



## Applications

* Biomedical sensor signal amplification
* Environmental monitoring
* Industrial analog control systems
* Educational demonstrations

---

## Viva Questions

* What is the function of OP07?
* What does CD4052 do in this circuit?
* Why is a voltage regulator used?
* What are advantages of precision op-amps?
* How does LM35 work?

---

## Gallery
![WhatsApp Image 2025-05-23 at 6 53 46 PM](https://github.com/user-attachments/assets/3b7f17f4-5490-4892-8135-dbcc0ee91b06)

![WhatsApp Image 2025-05-23 at 6 53 45 PM](https://github.com/user-attachments/assets/235f8824-33e0-49ed-a7e8-7dbae198a452)

---

## References

* [OP07 Datasheet](https://www.ti.com/product/OP07)
* [CD4052 Datasheet](https://www.ti.com/lit/ds/symlink/cd4052b.pdf)
* [Original Project Page](https://bestengineeringprojects.com/how-to-build-a-precision-amplifier-circuit-using-op07-and-cd4052-multiplexer/)

