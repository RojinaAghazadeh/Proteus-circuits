
# 3-to-8 Decoder Using 74HC138 | Proteus

## Overview

This project demonstrates the design and simulation of a **3-to-8 Decoder** using the **74HC138** IC in Proteus. The decoder converts a 3-bit binary input into one of eight output lines, where only one output is active at a time.

## Components Used

* 74HC138 3-to-8 Decoder IC
* Logic State switches
* 330 Ω resistors
* LEDs
* Power supply

## Inputs

* A
* B
* C
* Enable pins

The input values are provided using **Logic State** switches.

## Outputs

* Y0–Y7

Each output is connected to a **330 Ω resistor**, followed by an **LED** and then to the power supply. The LEDs indicate which output line is active for the selected input combination.

## How It Works

1. A 3-bit binary value is applied to the inputs (A, B, and C) using the Logic State switches.
2. When the decoder is enabled, it activates one of its eight outputs based on the input combination.
3. The active output lights its corresponding LED, while the remaining LEDs stay off.
4. Changing the input values selects a different output, allowing the LEDs to visually demonstrate the decoder's operation.

## Simulation

The circuit was designed and simulated in Proteus. Different input combinations were tested to verify that only the correct output became active for each binary input.

## Results

The decoder successfully converts a 3-bit binary input into eight output lines. The LEDs provide a simple visual indication of the active output, making it easy to verify the correct operation of the circuit during simulation.