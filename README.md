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

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: Meyyappan T 

RegisterNumber: 212223240086
```
module ex02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```


**RTL realization**

**Output:**

![ex-output2](https://github.com/akash7812/BOOLEAN_FUNCTION_MINIMIZATION/assets/146819826/1f65b886-29e5-40e1-a37f-00c204d52827)

**Truth Table**

![285832032-236326de-e839-4fad-908b-bb236e0a13dd](https://github.com/sanjayashwinP/BOOLEAN_FUNCTION_MINIMIZATION/assets/147473265/399f99d5-79cc-443a-b54a-41d7a0326a5c)


**RTL**

**Timing Diagram**

![Screenshot 2024-04-10 110400](https://github.com/akash7812/BOOLEAN_FUNCTION_MINIMIZATION/assets/146819826/6e1f1acc-2b74-4869-afd8-2f1910c9d372)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

