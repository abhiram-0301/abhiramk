**By Referring to C-based Lab videos and RISC-V-based lab videos**

**Snapshots of the compiled C code and RISC-V**

**Step 1: check whether the leafpad is installed in ur machine by using the commands
leafpad sum1ton.c& (sum1ton.c is the file name)
If the leafpad editor is opened without any errors then type the C code.**
****If the leafpad is not installed in ur machine then install by using the following command**

**sudo snap install leafpad****
![35f66339-213d-459a-adcf-431684119dfd](https://github.com/abhiram-0301/abhiramk/assets/149863256/15299254-c043-42c1-b212-29fe2d864187)



****Step 2: Writing the C code in the leafpad editor** using the following command

**leafpad sum1ton.c&**
![61b19bf3-fcda-45fc-8528-c78907a9a714](https://github.com/abhiram-0301/abhiramk/assets/149863256/c2166b6d-2bc5-41e0-ab6f-f8122a9d1b6d)



**Step 3: After writing the C code save the editor by Ctrl+s**

**Step 4: Check for the errors by using the following command(compilation step)**

**gcc sum1ton.c**
![35f66339-213d-459a-adcf-431684119dfd](https://github.com/abhiram-0301/abhiramk/assets/149863256/ba866201-1dbc-4657-9ac5-e2cee6cc1763)



**Step 5: Check the output by using the command**

**./a.out**
![35f66339-213d-459a-adcf-431684119dfd](https://github.com/abhiram-0301/abhiramk/assets/149863256/a7ea3b28-1629-44fd-af8b-9cea86c78e20)

**The results will be displayed as** 

**Sum of numbers from 1 to 500 is 125250**


********************************************************RISCV Compilation and Execution*****************************************************

**Step 1: View the C Code in the editor window using the following command**

**cat sum1ton.c**
![677e5cee-be7a-4b48-98d0-919a16347853](https://github.com/abhiram-0301/abhiramk/assets/149863256/8ca7716a-bc51-4f92-9d9e-ea5d2ec05002)


**Step 2: Compile the code in riscv using the following command**

**riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**
![677e5cee-be7a-4b48-98d0-919a16347853](https://github.com/abhiram-0301/abhiramk/assets/149863256/5970fa1b-68bf-4156-8cbc-345c62e24c3e)



**Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.**

**use the command**

**ls -ltr sum1ton.c**
![677e5cee-be7a-4b48-98d0-919a16347853](https://github.com/abhiram-0301/abhiramk/assets/149863256/8c1a3bcc-d2e5-482d-93f1-fa606adbdfe8)

![a31c3c92-1fc2-4141-9272-0f4068dcd684](https://github.com/abhiram-0301/abhiramk/assets/149863256/d37e7dd2-3739-4aa6-94ae-cb3a404f86b6)



**Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution**

![b8ca6f8c-5e91-4ff0-ba09-3929a456eeb6](https://github.com/abhiram-0301/abhiramk/assets/149863256/d07994ea-8a4a-4946-a433-bcf173422dd0)



![b566f551-da3e-47ee-bc53-06b9a2e306f4](https://github.com/abhiram-0301/abhiramk/assets/149863256/e30c6016-ce7e-4fa3-99e0-9d4ad9b4c855)

**Step 4:**

**riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**

![8d30f96c-b9bd-4b1c-816e-d93da3e6f0e0](https://github.com/abhiram-0301/abhiramk/assets/149863256/66fb9206-f2c1-454b-bc90-b1e4d59d1540)
![b9240f92-1a8a-496d-b777-41fa5e4357f0](https://github.com/abhiram-0301/abhiramk/assets/149863256/05d036a6-af9d-4326-b13e-15d33950d730)







