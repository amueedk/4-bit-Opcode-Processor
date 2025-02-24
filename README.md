# 4-bit Opcode Simulator for 16-bit Architecture

## Overview
This project is a **4-bit opcode simulator** designed for a **16-bit architecture**. It simulates the execution of machine-level instructions, allowing users to test and understand low-level processing.

## Files Included
- **addition.txt**: Sample program for performing addition.
- **multiplication(5x3).txt**: Sample program demonstrating multiplication.
- **processor_simulator222.ui**: Qt UI file for the graphical interface.
- **simulator.py**: The main Python script for executing the simulation.
- **subroutine_to_shift_AC.txt**: Sample subroutine for shifting the accumulator.

## Features
- Simulates a **4-bit opcode system** for a **16-bit architecture**.
- Provides a graphical interface using Qt for easy interaction.
- Supports **memory and register operations**, allowing users to perform arithmetic and logical computations.
- Includes a built-in **assembler-like environment** where users can write, execute, and save their programs.
- Allows loading **pre-written programs** from sample files for testing.
- Future updates will introduce **I/O operations** to enhance simulation capabilities.

## Running the Simulator
### Prerequisites
- Install Python 3.x
- Install required dependencies (if any)

### Steps to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/amueedk/4-bit-Opcode-Processor.git
   ```
2. Navigate to the project directory:
   ```bash
   cd 4-bit-Opcode-Processor
   ```
3. Run the simulator:
   ```bash
   python simulator.py
   ```

## Writing, Loading, and Saving Programs
- Users can **write their own programs** directly in the simulator and **save** them using the **Save** option in the menu.
- They can **load and test** sample programs using the **Load** option in the simulator.

## Supported Mnemonics
### Memory Reference Instructions
- **LDA** - Load data from memory to AC
- **STR** - Store data from a register to memory
- **JMP** - Jump to a specified memory location
- **JZE** - Jump if the AC is Zero
- **JSA** - Jump and save return address
- **AND** - Perform bitwise AND operation
- **OR** - Perform bitwise OR operation
- **XOR** - Perform bitwise XOR operation
- **ADD** - Add values in AC
- **SUB** - Subtract values in AC
- **MUL** - Multiply values in registers
- **INC** - Increment and skip if zero
- **DEC** - Decrement and skip if zero

### Register Reference Instructions
- **CRA** - Clear register AC
- **CRE** - Clear flag E
- **CTA** - Complement AC
- **CTE** - Complement E
- **CPA** - Compare accumulator with a value
- **INA** - Increment AC
- **SKP** - Skip if AC > 0
- **SKN** - Skip if AC
- **CRA** - Circulate right Shift AC and E
- **CLA** - Circulate left Shift AC and E
- **HAL** - Halt the processor

### I/O Reference Instructions *(Not yet implemented, but planned for future updates)*
- **INP** - Input character to AC
- **OUT** - Output character from AC
- **SFI** - Skip on input flag
- **SFO** - Skip on output flag
- **PUT** - Output data to a specified I/O device
- **OPT** - Perform an operation on the I/O device
- **SPI** - Send data to the serial peripheral interface
- **SPO** - Receive data from the serial peripheral interface
- **SIE** - Set/Reset interrupt enable flag

## NOTE
The simulator includes a **widget for I/O operations**, but it is **not yet implemented**. Future updates will integrate full I/O functionality.

## Future Improvements
- Implement I/O operations.
- Enhance UI for better usability.
- Add debugging features.

## Contributions
Feel free to fork, contribute, or report issues!

## License
This project is open-source under the MIT License.

---
This README provides a comprehensive guide on how to use and extend the **4-bit opcode simulator for a 16-bit architecture**. Let me know if you need any modifications! 🚀

