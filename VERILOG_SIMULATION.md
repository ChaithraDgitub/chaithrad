## 1. FUNCTIONAL SIMULATION

### 1.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 1.2 Installing iverilog and gtkwave

- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```
![1](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/14970f2b-f8a5-4f75-a555-89f3e8c80469)

- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/ChaithraDgitub/chaithrad.git
 $ cd 
```
![2](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/de7a925b-1327-498f-8112-17d3dc8952f1)

![3](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/46848864-2936-4986-8bd4-4021e57fd6ed)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![4](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/6ba0039e-fdc4-4d66-b031-8d73d8da6a27)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```

![5](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/4ea7ecbb-bcbf-495c-86d3-b9967da5dd23)


![6](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/f5cfeb92-06d7-4383-b502-6c05742b796d)

### 1.3 The output waveform

![7](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/0e5d7362-9cbe-4383-b0f5-cc22662f9e3b)

![8](https://github.com/ChaithraDgitub/chaithrad/assets/160298555/184b5688-79e5-4048-a181-a0f9c4f87b26)






 
















