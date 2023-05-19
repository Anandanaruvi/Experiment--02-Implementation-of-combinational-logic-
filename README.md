### Experiment--02-Implementation-of-combinational-logic

Implementation of combinational logic gates
 
### AIM:

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
 
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
### Equipments Required:

1. Hardware – PCs, Cyclone II , USB flasher
2. Software – Quartus prime

### Theory
 
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Combinational logic gates are digital circuits that produce outputs based solely on the current inputs. These gates are the building blocks for implementing digital systems and are used in a wide range of applications, including arithmetic and logic operations, memory devices, and control circuits.

The two functions, F1 and F2, can be implemented using a combination of logic gates such as AND gates, OR gates, and NOT gates.

### Procedure
1.Use module projname(input,output) to start the Verilog programmming.

2.Assign inputs and outputs using the word input and output respectively.

3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.

4.Use each output(RTL Viewer and Timing Diagram) to represent F1 and F2.

5.End the verilog program using keyword endmodule.

### Program:
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

DEVELOPED BY: A.ARUVI

REGISTER NO:212222230014
```
F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

module exp2f1(A,B,C,D,f1);
input A,B,C,D;
output f1;
assign f1=(~B&~D)|(A&B&~C)|(~A&B&D);
endmodule

F2=xy’z+x’y’z+w’xy+wx’y+wxy

module exp2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=(~y&z)|(x&y)|(w&y);
endmodule
```
### Output:

### RTL

### F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://github.com/Anandanaruvi/Experiment--02-Implementation-of-combinational-logic-/assets/120443233/8a575474-8dc8-4aa6-b138-9d4a8b21a7cb)

### F2=xy’z+x’y’z+w’xy+wx’y+wxy

![image](https://github.com/Anandanaruvi/Experiment--02-Implementation-of-combinational-logic-/assets/120443233/20bcfdb2-a6e9-4971-a53c-eabde15c39d6)

### Timing Diagram

### F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://github.com/Anandanaruvi/Experiment--02-Implementation-of-combinational-logic-/assets/120443233/de199ca1-3670-412b-9e7c-9a5f9e21d459)

### F2=xy’z+x’y’z+w’xy+wx’y+wxy

![image](https://github.com/Anandanaruvi/Experiment--02-Implementation-of-combinational-logic-/assets/120443233/336dfc52-20e8-41a5-8531-173dcd9dd7c8)

### Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
