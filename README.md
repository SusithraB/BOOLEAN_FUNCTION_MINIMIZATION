
# BOOLEAN_FUNCTION_MINIMIZATION
```
Developed by: SUSITHRA.B

RegisterNumber: 212223220113
```

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

```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

```
## Logic symbol & Truthtable:
![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/9179c0bd-fe5b-4db5-a1f0-3575ffed7354)

![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/58d5f0e5-0864-4fe7-b6e0-6dafc3692fdf)


**RTL realization**

![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/87da947d-c8a0-4a99-b40f-922b269a0724)

![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/b2c9fbb9-877e-4512-9848-658645efd506)


**Output:**
![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/c99265d0-65c1-418d-afeb-19aaf90c93ec)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

