# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of reducing a Boolean expression to its simplest or most efficient form without changing its output behavior.

BOOLEAN FUNTIONS:

Expression: combination of variables with AND, OR, NOT

Example:
F(A,B,C)=ABC+AB+C


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module exp2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```
RegisterNumber:25013604


**RTL realization**
<img width="1757" height="869" alt="Screenshot 2025-11-17 133339" src="https://github.com/user-attachments/assets/0766c567-7d50-4cfd-b697-84f94d436b1b" />

**Output:RTLTiming Diagram**
<img width="1920" height="1080" alt="Screenshot 2025-11-17 135602" src="https://github.com/user-attachments/assets/ca158a82-a836-414a-8908-7c03f00c7cf6" />

**Result:**

Thus the given logic functions are implemented using Boolean Functions and their operations are verified using Verilog programming.

