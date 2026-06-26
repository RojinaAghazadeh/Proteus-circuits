# 8-Bit Register Using 74HC574 | Proteus

## Overview

This project demonstrates the design and simulation of an **8-bit register** using the **74HC574 Octal D-Type Flip-Flop with Three-State Outputs** in Proteus. The register stores an 8-bit binary value on the rising edge of the clock and holds the data until a new value is loaded.

The simulation illustrates the basic concept of data storage, one of the fundamental building blocks of digital systems and computer architecture.

## Components Used

* 74HC574 Octal D-Type Flip-Flop
* Logic State switches
* Clock source
* Logic Probes

## Inputs

* **D0–D7**: 8-bit data inputs
* **CLK**: Clock input
* **OE̅**: Active-low Output Enable

## Outputs

* **Q0–Q7**: Stored 8-bit data outputs

The outputs are monitored using **Logic Probes**, making it easy to observe the stored binary value during simulation.

## How It Works

1. Set the desired 8-bit binary value using the data input switches (D0–D7).
2. Apply a rising edge to the **CLK** input.
3. The input data is stored inside the register.
4. When **OE̅ = 0**, the stored data appears at outputs **Q0–Q7**.
5. When **OE̅ = 1**, the outputs enter the high-impedance (Hi-Z) state while the stored data remains preserved internally.

## Simulation

The circuit was designed and tested in Proteus by applying different binary input values and clock pulses. Logic probes were used to verify that the register correctly stores and outputs the data according to the timing of the clock and the state of the active-low Output Enable pin.


## Results

The register successfully stores 8-bit binary data on the rising edge of the clock and maintains the stored value until new data is loaded. The active-low Output Enable allows the outputs to be enabled or placed in a high-impedance state, demonstrating the operation of tri-state logic commonly used in shared digital buses.
