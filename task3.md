By Referring to C-based Lab videos and RISC-V-based lab videos

Snapshots of the compiled C code and RISC-V

Step 1: check whether the leafpad is installed in ur machine by using the commands leafpad sum1ton.c& (sum1ton.c is the file name) If the leafpad editor is opened without any errors then type the C code. **If the leafpad is not installed in ur machine then install by using the following command

sudo snap install leafpad**
![photo1](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/e4439bd0-14e3-4eac-8a31-7edddbc9d306)
**Step 2: Writing the C code in the leafpad editor using the following command
leafpad sum1ton.c&

![photo2](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/9032568f-0411-4156-9c0d-e020d667c9f7)

Step 3: After writing the C code save the editor by Ctrl+s

Step 4: Check for the errors by using the following command(compilation step)

gcc sum1ton.c

Step 5: Check the output by using the command

./a.out

The results will be displayed as

Sum of numbers from 1 to 500 is 125250

***RISCV Compilation and Execution

Step 1: View the C Code in the editor window using the following command

cat sum1ton.c

**Step 2: Writing the C code in the leafpad editor using the following command

riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![photo3](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/bb623a9e-e9be-44f3-93f9-fcbff336e82f)

Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.

use the command
ls -ltr sum1ton.c


![photo4](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/d9293c6e-ad7f-4b29-a42b-f8b8acbcb412)

Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution

![photo5](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/421b49e0-bd71-4f66-8aa5-f20f82c95a11)

![photo6](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/ff61a1ef-b789-4a68-b425-4796dd41b62d)

Step 4:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

![photo7](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/16cc4a4a-e5fb-45b4-ab24-0835017829b6)

![photo8](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/898f1eb3-6308-40e7-a5f6-4e8fa70de107)
