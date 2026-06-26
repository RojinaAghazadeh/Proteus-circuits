# 4-Bit Magnitude Comparator | Proteus

## Overview

This project demonstrates the design and simulation of a **4-bit Magnitude Comparator** in Proteus. The comparator determines the relationship between two 4-bit binary numbers and indicates whether one value is greater than, less than, or equal to the other.

To demonstrate both digital logic design and practical implementation, two different versions of the circuit were developed.

## Project Versions

### 1. Logic Gate Implementation

The first design was built entirely using basic logic gates. This implementation demonstrates the internal logic used to compare two binary numbers by generating three outputs:

* **A > B**
* **A = B**
* **A < B**

### 2. 74HC85 IC Implementation

The second design uses the **74HC85 4-Bit Magnitude Comparator IC**, providing the same functionality with a dedicated comparator integrated circuit. This version illustrates how digital systems can be simplified using standard logic ICs.

### Logic Gate Version

* Logic State switches
* Logic Probes
* AND Gates
* OR Gates
* XOR Gates
* NOT Gates

### IC Version

* 74HC85 Comparator IC
* Logic State switches
* Logic Probes

## Inputs

* A3, A2, A1, A0
* B3, B2, B1, B0

## Outputs

* A > B
* A = B
* A < B

The output signals are monitored using **Logic Probes**, allowing the comparison result to be observed directly during simulation.

## Simulation

The circuits were designed and tested in **Proteus** by applying different binary values to the input switches and observing the output through the logic probes.

## Results

Both implementations successfully compare two 4-bit binary numbers and produce identical outputs for all possible input combinations. The logic gate version provides insight into the underlying comparison process, while the 74HC85 version demonstrates a compact and efficient hardware implementation.

