# Overview
 This repository has my design for the Duke 250/16 CPU, a 16-bit MIPS-like, wordaddressed RISC architecture.  The
architecture’s instructions are specified in the table below.
 
 There are 8 general purpose registers: $r0-$r7. The register $r7 is the link register for the jal instruction (similar to $ra in MIPS). The user of the CPU may write to it with other instructions, but that would mess up function call/return for them. Users of the CPU are also advised to use $r6 as the stack pointer. $r0 is the constant value 0 (i.e., an instruction can specify it as a destination but “writing” to $r0 will not change its value). 

# Instructions
![Alt text](./InstructionSet.png?raw=true "Title")
