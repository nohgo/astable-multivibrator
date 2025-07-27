# BJT Astable Multivibrator

## Project Overview
This project is a classic two-transistor astable multivibrator built to develop a hands-on understanding of transistors as electronic switches.

## Demo
![astable-multivibrator](https://github.com/user-attachments/assets/3e3eb8e3-a319-4156-be18-4c09b3521d21)


## Technical Specifications
- Topology: Astable Multivibrator
- Active Components: 2x 2N2222 NPN BJT Transistors
- Timing Components: 2x 100k&Omega; resistors, 2x 10&mu;F Capacitors
- Calculated Time Period: ~1.38s
- Measured Time Period: ~1.14
- Power Source: 9V Battery

## How It works
The circuit works by using two transistors that turn eachother on and of in a continous cycle. The speed of the cycle is determined by the RC time constant of the base resistors and the timing capacitors. When one transistor turns on, it forces the other transistor off by discharging the capacitor connected to its base. This "off" transistor then begins to chareg its own base capacitor until it reaches the turn-on voltage, flipping the state of the circuit. This cross-coupled process created a stable, oscillating square wave output.

## Design and Validation Process

1. Simulation

I first simulated the circut in LTspice to predict its behavior and develop a conceptual understanding. The LTSpice simulation confirmed the predicted time period and showed the square wave created by the circuit.

Circuit Schematic | Waveform Output
--------| --------
<img width="544" height="414" alt="Screenshot 2025-07-27 at 5 02 14 PM" src="https://github.com/user-attachments/assets/3a9e27d7-dcac-4494-a123-49abfbbc78d6" /> | <img width="544" height="414" alt="Screenshot 2025-07-27 at 4 52 53 PM" src="https://github.com/user-attachments/assets/9deab294-9226-4684-88af-17143c74b586" />

2. Physical Prototype

I then constructed the circuit on a solderless breadboard, and timed the blinking using video. Additionally, I tested the voltage differences at various points using a digital multimeter.

![E5E6D20B-95C7-44F2-8710-F8119AF032DB_4_5005_c](https://github.com/user-attachments/assets/868e0fc7-8980-44a7-865a-fe4fc319c442)

## Challenges & Learnings

My most significant challenge was problems with my simulation, one caused by a misoriented transistor and one caused by 1Meg resistors not providing enough current to the base of the transistors. The first issue was a trivial fix, and the second issue I fixed by proportionally changing my resistor and capacitor values so I could maintain the same time constant. It was interesting to experience a taste of component selection. On the other hand, my biggest learning opportunity was using the breadboard and multimeter for the first time, which gave me the first taste of physical lab work. Overall I enjoyed the mini project, it feels fufilling to actually see your circuit function.

