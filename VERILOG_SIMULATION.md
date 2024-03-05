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
![1](https://github.com/abhiram-0301/abhiramk/assets/149863256/cd3c9748-0843-4de3-892c-ab0656274369)

## 3. INSTRUCTION SET OF RISC-V RV32I
![2](https://github.com/abhiram-0301/abhiramk/assets/149863256/a47243f2-b040-4bb4-ba5e-67ce5993c794)

![3](https://github.com/abhiram-0301/abhiramk/assets/149863256/8cc89500-2a5d-41dd-9301-3a4859f64f02)

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
![Screenshot from 2024-03-02 12-12-52](https://github.com/abhiram-0301/abhiramk/assets/149863256/1e1f1d0d-6370-4da0-9240-bde6063a6f41)


- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/Abdulbitm/Abdul
 $ cd Abdul
```
![Screenshot from 2024-03-02 12-12-26](https://github.com/abhiram-0301/abhiramk/assets/149863256/7011a73c-81b1-4aae-a8cf-274274a01073)

- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```
![Screenshot from 2024-03-02 13-04-30](https://github.com/abhiram-0301/abhiramk/assets/149863256/73ac1ae0-7b6d-42cf-a387-3db2b724c809)


- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![Screenshot from 2024-03-02 13-04-30](https://github.com/abhiram-0301/abhiramk/assets/149863256/057fea12-d197-43e8-aeda-55e1360c1ecd)

### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
<img width="1282" alt="309717644-9475de20-c117-476a-bebc-54dd3548c109" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/14cbf220-7ff4-4a81-a8a1-6a5b4d0332cf">

 Instruction 2:sub r7,r1,r2
<img width="1280" alt="309717941-2c95f18f-191e-4500-9cda-e7e838d1e609" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/f206864a-55bd-4683-8fa7-944c53c2af14">

Instruction 3:and r8,r1,r3
<img width="1282" alt="309718134-18bfdf76-1173-4984-b50b-83443ab48596" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/d591f9e3-5432-436f-86e3-9f050dace321">

Instruction 4:or r9,r2,r5
<img width="1294" alt="309718310-4f214bb2-c934-4778-bf46-841efe877fb8" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/2dab716e-ac57-43dc-a38a-0322067c9fb1">

 Instruction 5:xor r10,r1,r4
<img width="1293" alt="309718453-6fa91f49-5e73-4133-8bf6-84ec4aca64da" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/bb6c7539-c8ea-4dad-9a99-7fde6db6b951">

 Instruction 6:slt r11,r2,r4
<img width="1290" alt="309718574-c9c32048-62ed-4f55-8e11-9763816b1bd1" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/bbe60435-c164-48d6-a599-d6f6dff76998">

 Instruction 7:addi r12,r4,5
<img width="1285" alt="309718717-308b8a9d-46c8-4a0e-8824-90e11d9a6a1e" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/e627cd91-6a3c-4b67-991d-f4b97d6ef96a">

 Instruction 8:sw r3,r1,2
<img width="1280" alt="309718858-84f16d7f-9d16-4236-b64d-615e187a00ff" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/2633c70f-118f-4a9e-94c7-e14eab9978b3">

 Instruction 9:lw r13,r1,2
<img width="1295" alt="309719046-c7bc7d9a-6745-4eeb-903d-fa723dca1394" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/e57c1868-009c-4bf8-b66b-a0e11af3d17e">

 Instruction 10:beq r0,r0,15
<img width="1287" alt="309719144-a1c6781f-c301-45d9-a502-fb32e6204e4c" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/60421b92-f443-4616-957f-8c6c73aa5ee2">

 After branching, performing
 Instruction 11:add r14,r2,r2
<img width="1287" alt="309719297-56b50ce0-60aa-41fe-8f53-0b4583b39665" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/41287e99-4545-40cb-9e1d-f2bf9a0a24be">

  Full 5-stage instruction pipeline and pc-increment description Waveform
  <img width="1325" alt="309719447-e5ebc923-ad2c-44fc-a577-3ce7b8419bce" src="https://github.com/abhiram-0301/abhiramk/assets/149863256/6429156c-1518-4d4b-9d99-79457c9d379a">

![Screenshot from 2024-03-02 12-58-34](https://github.com/abhiram-0301/abhiramk/assets/149863256/b217cbf7-dd39-4344-8ae6-8f0aef75eddd)

![Screenshot from 2024-03-02 12-45-33](https://github.com/abhiram-0301/abhiramk/assets/149863256/bf77c786-2fdf-4ff6-92bc-c37a31d05e4e)



