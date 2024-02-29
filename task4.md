# **The C code should undergo the simulation of normal GCC X86 Compiler and riscv compiler** (**SPIKE Simulation**) 

**AS PER THE REQUIREMENT OUTPUT OF GCC (F1) SHOULD BE EQUAL = TO OUTPUT OF RISCV GCC (F2)**

![WhatsApp Image](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/b443f806-47d8-41da-8bfb-bdce83bff75d)

**Step - 1**: To Run the code in the normal GCC Compiler</p>


  To compile the code: 
            
        gcc sum1ton.c -o sum1ton
   To Get the output use:
       
       ./a.out
  Here the output finds to be -Sum of numbers from 1 to 250 is 31375

![WhatsApp Image 1](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/0a7b3613-3b70-4d0f-8c14-6c0086ceb7bb)

**Step - 2**: To Run the code in the RISC-V GCC Compiler</p>
To compile the code :</p>

    riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
    gcc sum1ton.c -o sum1ton
    ./sum1ton
 Here the output finds to be -Sum of numbers from 1 to 250 is 31375</p>

  ![WhatsApp Image 2](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/a980e344-c309-4913-92df-a28b1f0a8717)

   To compile the code:
  
    riscv64-unknown-elf-gcc -o sum1ton sum1ton.c
  or
    
    riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
  or

    riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
 (by referring the image given below) </p>
 To Get the output use:

    ./a.out
 Here the output also finds to be -Sum of numbers from 1 to 250 is 31375

![WhatsApp Image 3](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/924f4cd4-ef3e-4424-91c0-010fcc0db36a)

 

