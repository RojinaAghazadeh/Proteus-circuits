The 6116 is a static random-access memory (SRAM) chip that can store 2K × 8 bits of data. It is commonly used in digital systems to temporarily store information that can be read or modified during operation. Unlike ROM, the contents of RAM can be changed at any time while power is supplied.

In this Proteus simulation, the 6116 RAM is used to demonstrate basic memory operations, including writing data to a memory location and reading data from it. The address lines are used to select a memory location, while the data lines transfer information into or out of the memory.

To write data, the desired address is selected, the data value is applied to the data inputs, and the Write Enable (WE) signal is activated. To read data, the address is selected and the Output Enable (OE) signal is activated while the Write Enable signal remains inactive. The stored data then appears on the data output lines.

This experiment helps demonstrate how RAM stores, retrieves, and updates data in digital systems.


ce = chip enable
we = write enable 
oe = output enable 

1. Select a memory address using the address inputs (A0-A10).
2. Put the desired 8-bit data on the data lines.
3. Set CE = 0, WE = 0, and OE = 1 to write the data.
4. Return WE = 1 after writing.
5. To read, keep the same address, set CE = 0, WE = 1, and OE = 0.
6. Observe the stored data on the output lines.