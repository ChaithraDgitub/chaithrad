# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
![p1](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/16153704-9f6d-4ed5-9c53-4c67920a26a1)

## 3. INSTRUCTION SET OF RISC-V RV32I
![p2](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/a1eafcf3-c962-4116-a76b-bc09832fe322)
![p3](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/e4c26f87-7683-4e80-a5aa-1bd6513f997a)

## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**
 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```
![p4](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/71cb0653-3b02-4b9f-9eb9-b302baf8cc0f)

- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/ChaithraDgitub/chaithrad.git
 $ cd chaithra
```
![p5](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/0c4c5a04-f764-401d-a653-7b849ef31710)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![p6](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/c8cbe9bb-0003-4a68-8161-f948e24fc5bb)

- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![p7](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/c5b08d36-91a8-4daa-8fb7-54b1a61ab954)

### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 ![p8](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/7d994f54-ec6d-424d-8f46-468c0d282f3e)

  Instruction 2:sub r7,r1,r2
  ![p9](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/e2d22358-cdb2-4bd5-858a-1817894a93d8)

  Instruction 3:and r8,r1,r3
  ![p10](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/440931ff-04e4-4638-857b-415f21a335b5)

  Instruction 4:or r9,r2,r5
  ![p12](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/3b7e84be-ed77-41b1-8223-53b998fd0c0c)

   Instruction 5:xor r10,r1,r4
   ![p13](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/fbd95c54-afe1-42f9-b260-9d06c1d75b63)

    Instruction 6:slt r11,r2,r4
   ![p14](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/00084e2a-6b58-4fa5-bc82-1a85d5e2a5ab)

     Instruction 7:addi r12,r4,5
   ![p15](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/d13b2425-cb26-4a3a-8aaa-5035da927ddc)

      Instruction 8:sw r3,r1,2
   ![p16](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/6f0a72a0-5b7e-4a66-8a1e-7db7de87ea72)

       Instruction 9:lw r13,r1,2
![p17](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/4f6c7493-1e46-4101-b03a-0422ddbe22c5)

              Instruction 10:beq r0,r0,15
   ![p18](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/4d7fcd8d-6d14-4acd-8398-81ce4d8502f9)

         After branching, performing
 Instruction 11:add r14,r2,r2
 ![p19](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/0de44b4d-2433-4af5-8878-54570c29d7f5)

 Full 5-stage instruction pipeline and pc-increment description Waveform
 ![p20](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/937d859c-965c-4605-aa9c-e55f669b432e)
 
![p21](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/e0ee5a0a-f5c3-426a-9e06-9b49b52a58b1)

![p22](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/5170364f-a0d9-4688-affc-27e7b4cffbcb)



 
















