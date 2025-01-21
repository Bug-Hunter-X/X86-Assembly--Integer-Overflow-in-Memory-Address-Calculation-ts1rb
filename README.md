# x86 Assembly: Integer Overflow in Memory Address Calculation

This repository demonstrates a common error in x86 assembly programming: integer overflow during memory address calculation.  The `bug.asm` file contains code that exhibits this issue, leading to unpredictable behavior. The `bugSolution.asm` file provides a corrected version.

The bug is caused by a lack of bounds checking on the ECX register before performing the address calculation.  If ECX exceeds a certain value, multiplying it by 4 results in an integer overflow, leading to an incorrect memory address.