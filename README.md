16-bit ALU Design using Verilog

📖 Overview
This repository contains the design and verification of a 16-bit Arithmetic Logic Unit (ALU) implemented in Verilog. The ALU performs a range of arithmetic, logical, and shift operations based on a control signal (opcode) and generates corresponding status flags.

The project is intended to demonstrate fundamental digital design concepts, including combinational logic design, flag generation, and functional verification using a testbench.

🎯 Objectives
Design a parameterized 16-bit ALU
Implement multiple arithmetic, logical, and shift operations
Generate and verify status flags
Develop a testbench to validate functionality across different cases

⚙️ Features
✔ Arithmetic Operations

Addition

Subtraction

Increment

Decrement

✔ Logical Operations

AND

OR

XOR

NOT

✔ Shift Operations

Logical Left Shift

Logical Right Shift

Arithmetic Right Shift

Rotate Right

✔ Status Flags
Z (Zero): Set when result is zero

C (Carry): Indicates carry/borrow in arithmetic operations

N (Negative): Reflects sign bit (MSB) of result

V (Overflow): Indicates signed overflow

🧠 Design Approach

The ALU is implemented using a combinational logic approach with a case statement driven by a 4-bit opcode.

Inputs:
Two 16-bit operands (A, B)
Operation select (opcode)

Outputs:
16-bit result
Status flags (Z, C, N, V)

Arithmetic operations use an intermediate register to capture carry-out, while overflow detection is handled using sign-based logic. Logical and shift operations are implemented using standard Verilog operators.

🔢 Opcode Mapping
Opcode	Operation

0000  Addition

0001	Subtraction

0010	Increment

0011	Decrement

0100	AND

0101	OR

0110	XOR
0111	NOT
1000	Shift Left
1001	Shift Right
1010	Arithmetic Shift Right
1011	Rotate Right
