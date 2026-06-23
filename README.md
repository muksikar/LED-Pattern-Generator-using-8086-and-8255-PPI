# LED-Pattern-Generator-using-8086-and-8255-PPI


## Overview

This project presents the design and implementation of an **LED Pattern Generator** using the **8086 Microprocessor** and **8255 Programmable Peripheral Interface (PPI)**. The system generates various LED blinking and shifting patterns by interfacing LEDs with the 8086 microprocessor through the 8255 PPI.

The project demonstrates the fundamentals of microprocessor interfacing, I/O programming, and digital system design. By sending different output data patterns to the 8255 PPI, multiple LED sequences can be generated and observed in real time.

---

## Objectives

* Interface the 8086 microprocessor with the 8255 PPI.
* Generate different LED patterns using assembly language programming.
* Understand microprocessor-based I/O operations.
* Learn the configuration and operation of the 8255 PPI.
* Simulate and verify LED patterns using digital hardware.

---

## Theory

### 8086 Microprocessor

The 8086 is a 16-bit microprocessor developed by Intel. It consists of a Bus Interface Unit (BIU) and an Execution Unit (EU), making it capable of handling data processing and memory interfacing efficiently.

### 8255 Programmable Peripheral Interface (PPI)

The 8255 is a programmable I/O device that provides 24 input/output lines divided into three 8-bit ports:

* Port A (8-bit)
* Port B (8-bit)
* Port C (8-bit)

These ports can be configured as input or output ports depending on system requirements.

### LED Pattern Generation

The microprocessor sends binary data to the output port of the 8255. Each bit controls the ON/OFF state of an LED.

Example:

```text
00001111
```

* Lower four LEDs ON
* Upper four LEDs OFF

By continuously changing the output data, different LED patterns such as blinking, shifting, and running lights can be generated.

---

## Tools Used

| Tool                                | Purpose              |
| ----------------------------------- | -------------------- |
| 8086 Microprocessor Kit / Simulator | Program Execution    |
| 8255 PPI                            | I/O Interfacing      |
| Assembly Language                   | Programming          |
| LEDs                                | Output Display       |
| Proteus / Hardware Setup            | Circuit Verification |

---

## Project Structure

```text
LED-Pattern-Generator-using-8086-and-8255-PPI
│
├── Source_Code/
│   ├── LED_Pattern.asm
│
├── Circuit_Diagram/
│   ├── Interfacing_Schematic
│
├── Simulation_Results/
│   ├── LED_Patterns
│
├── Documentation/
│   └── Project_Report.pdf
│
└── README.md
```

---

## System Architecture

```text
8086 Microprocessor
         │
         ▼
   8255 PPI
         │
         ▼
    LED Array
         │
         ▼
 Pattern Display
```

---

## Circuit Operation

### Step 1: Initialization

* Configure the 8255 PPI in output mode.
* Initialize control word register.

### Step 2: Data Transmission

* The 8086 sends binary data to the output port.
* Each output bit corresponds to an LED state.

### Step 3: Pattern Generation

* Different binary values are transmitted sequentially.
* LEDs display predefined patterns.

### Step 4: Repetition

* Delay routines create visible blinking effects.
* Patterns continuously repeat to generate animations.

---

## Simulation Results

### Pattern 1: Alternate LEDs

```text
10101010
```

### Pattern 2: Running Light

```text
00000001
00000010
00000100
00001000
...
```

### Pattern 3: All LEDs Blink

```text
11111111
00000000
```

The observed LED outputs successfully match the programmed binary sequences.

---

## Applications

* Digital Display Systems
* Embedded System Education
* Industrial Indicator Panels
* Sequential Control Systems
* Microprocessor Laboratory Experiments
* Learning Hardware Interfacing Concepts

---

## Learning Outcomes

Through this project, the following concepts were explored:

* 8086 Microprocessor Architecture
* Assembly Language Programming
* Memory-Mapped and I/O-Mapped Interfacing
* 8255 PPI Configuration
* Digital Output Control
* Hardware-Software Integration
* Timing and Delay Generation

---

## Future Work

* Add switch-based pattern selection.
* Interface seven-segment displays and LCDs.
* Develop programmable pattern generators.
* Integrate microcontrollers such as 8051 or Arduino.
* Create dynamic LED animations using interrupts and timers.

---


---

## Acknowledgements

This project was completed as part of the Microprocessors and Interfacing Laboratory to gain practical experience in 8086 programming, peripheral interfacing, and digital hardware design.

---

### Repository Link

GitHub Repository: https://github.com/muksikar/LED-Pattern-Generator-using-8086-and-8255-PPI

