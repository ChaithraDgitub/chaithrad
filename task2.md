# Let's learn various types of RISC-V instructions
<p align="justify">RISC-V instructions are encoded using a fixed-length 32-bit format, which simplifies decoding and execution. The instruction formats are categorized into six types: R, I, S, B, U, and J. Each format serves a specific purpose and has a unique encoding structure:</p>

<details>
<summary><b>R-type instructions:
</b></summary>
<br>
<p align="justify">In RISC-V, the R-type instruction format is used for arithmetic and logical operations that involve two source registers and one destination register Eg:- Source Register 1 (rs1): x2</p>
  </details>
<details>
<summary><b>I-type instructions:
</b></summary>
<br>
<p align="justify">The I-type instruction format in RISC-V is used for operations that involve an immediate value (constant) and one or two registersEg:- ADDI x1, x2, 10
</p>
  </details>
<details>
<summary><b>S-type instructions:
</b></summary>
<br>
<p align="justify">In RISC-V, the S-type (Store) instruction format is used for storing a value from a register into memory. Eg:- SW x1, 100(x2)
</p>
  </details>
<details>
<summary><b>B-type instructions:
</b></summary>
<br>
<p align="justify">In RISC-V, the B-type (Branch) instruction format is used for conditional branch operations. Eg:- BEQ x1, x2, 100
</p>
  </details>
<details>
<summary><b>U-type instructions:
</b></summary>
<br>
<p align="justify">The U-type instructions are designed to facilitate the manipulation of the upper bits of a register or the program counter. They allow for the efficient loading of large immediate values into registers, supporting a wide range of constant values in a single instruction.Eg:- lui (load upper immediate value)</p>
  </details>
<details>
<summary><b>J-type instructions:
</b></summary>
<br>
<p align="justify">In RISC-V, there is no specific "J-type" instruction format as traditionally seen in other instruction set architectures like MIPS. Instead, the jump or branch instructions are typically encoded within the B-type (Branch) or I-type (Immediate) instruction formats. Eg:- J (jump)</p>
</details>

# Base Instructions Format

<p align="justify">The basic instruction set in RISC-V, or Reduced Instruction Set Computing - Five, encompasses a straightforward and modular design aimed at providing a foundation for a wide range of computing applications. The core instructions include R-type (Register), I-type (Immediate), S-type (Store), B-type (Branch), and J-type (Jump) formats. The R-type instructions involve operations between registers, I-type instructions handle immediate values, S-type instructions are responsible for storing data to memory, B-type instructions manage conditional branches, and J-type instructions encompass jumps and subroutine calls. Each instruction format has a consistent structure with fields such as opcode, source registers, destination registers, and immediate values. RISC-V's minimalistic approach to instruction design simplifies decoding and execution, contributing to the architecture's efficiency and versatility.
<details>
<summary><b>Instruction code format </b></summary>
	<br>
![instruction code formats] ![Screenshot 2024-02-22 153103](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/90706333-ee58-488e-9e4c-326461b526f4)

</details>

# RISC-V REGISTER FILE: 
 <p align="justify">The RISC-V register file is a key component of the RISC-V architecture, providing a set of storage locations for holding data during the execution of instructions. The register file is organized into a set of integer registers and floating-point registers, depending on the extensions implemented in the processor. Registers play a crucial role in the RISC-V architecture, as they enable fast access to data and help improve the performance and efficiency of the processor.</p>
