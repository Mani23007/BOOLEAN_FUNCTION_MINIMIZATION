# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/
module Exp3(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d) | (~a & d) | (a & b & ~c));
endmodule 

module exp3(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z) | (x & y) | (w & y));
endmodule 


**RTL realization**
![RTL](https://github.com/user-attachments/assets/3e99310d-6798-41e2-b852-5ae4737dbcce)
![RTL](https://github.com/user-attachments/assets/50337223-4b88-4c4a-bd57-f0c14742420b)

**Timing Diagram**
![time waveform](https://github.com/user-attachments/assets/76fd41a1-0fa8-48af-bee9-86e8cc104c93)
![png 2](https://github.com/user-attachments/assets/273dfac7-4b3e-46c0-8c5a-cf357f1419be)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

