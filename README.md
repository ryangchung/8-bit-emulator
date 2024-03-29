# 8-Bit-Emulator

This is an emulator inspired by Ben Eater's breadboard CPU. It parses 8-bit binary instructions and runs it.

## Instruction set:
| Instruction | Operator |
| ----------- | -------- |
| NOP         | 0000     |
| LDA         | 0001     | 
| ADD         | 0010     |
| SUB         | 0011     |
| STA         | 0100     |
| LDI         | 0101     |
| JMP         | 0110     |
| JC          | 0111     |
| JZ          | 1000     |
| DEBUG       | 1001     |
| OUT         | 1110     |
| HLT         | 1111     |


## 8-bit instruction:
A valid instruction is 8 bits: 4 bit operator + 4 bit operand. An operand can be any 4 bit binary number. Any characters after 8 bits is considered a comment.

Due to the artificial limitation of 16 bytes of virtual RAM, only the first 16 lines of binary code will run.

## Technology Choices

Python was chosen due to its binary type system and conversions. To make it more efficient and applicable to real use, C would be preferrable.

## How to Install and Use
1. Pull this repository down to your computer
2. Run the script, with your binary file as CLI input
