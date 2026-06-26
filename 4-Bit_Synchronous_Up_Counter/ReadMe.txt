# 8-Bit Synchronous Binary Counter Using 74HC161 | Proteus

## Overview

This project demonstrates the design and simulation of an **8-bit synchronous binary counter** using two **74HC161 4-bit synchronous binary counter ICs** connected in cascade. The circuit counts upward in binary with each clock pulse and displays the current count on two seven-segment displays through **74HC47 BCD-to-Seven-Segment Decoder/Driver ICs**.

By cascading two 4-bit counters, the circuit forms an 8-bit counter capable of counting from **0 to 255**.

## Components Used

* 2 × 74HC161 Synchronous Binary Counter ICs
* 2 × 74HC47 BCD-to-Seven-Segment Decoder/Driver ICs
* 2 × Seven-Segment Displays
* Clock source
* Logic State switches

## Inputs

* **CLK**: Common clock input connected to both counters
* **CLR**: Reset input
* **LOAD**: Parallel load input
* **ENP** and **ENT**: Count enable inputs

The corresponding control pins of both 74HC161 ICs are connected together so they operate synchronously using the same control signals.

## Outputs

* **Q0–Q3:** Lower 4-bit counter
* **Q4–Q7:** Upper 4-bit counter

Each 4-bit output is connected to a **74HC47 decoder**, which converts the binary value into signals for a seven-segment display. This allows the current count to be monitored visually in hexadecimal format.

## How It Works

1. A clock pulse is applied to the shared **CLK** input.
2. The lower 74HC161 increments its count on each rising edge of the clock.
3. After the lower counter completes its counting cycle, the upper counter advances, creating an 8-bit counting sequence.
4. Both counters share the same **CLK, CLR, LOAD, ENP, and ENT** signals, ensuring synchronized operation.
5. The outputs of each counter are sent to a **74HC47 decoder**, which drives its corresponding seven-segment display.
6. The displays update continuously, providing a visual representation of the current counter value.

## Simulation

The circuit was designed and simulated in Proteus by applying clock pulses and observing the counting sequence on the seven-segment displays. The reset and enable functions were also tested to verify correct operation.

## Results

The circuit successfully implements an 8-bit synchronous binary counter using cascaded 74HC161 ICs. The synchronized control signals ensure reliable counting, while the 74HC47 decoder/drivers convert the binary outputs into seven-segment display signals for easy monitoring during simulation.

