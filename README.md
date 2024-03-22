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

Developed by:SUSITHRA.B
RegisterNumber:212223220113
## program
## module combinationalcircuit(A,B,C,D,F1);
## input A,B,C,D;
## output F1;
## wire x1,x2,x3,x4,x5;
## assign x1=(~A)&(~B)&(~C)&(~D);
## assign x2=(A)&(~C)&(~D);
## assign x3=(~B)&(C)&(~D);
## assign x4=(~A)&(B)&(C)&(D);
## assign x5=(B)&(~C)&(D);
## assign F1=x1|x2|x3|x4|x5;
## endmodule 


**RTL realization**
![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/fd3d1077-4e9c-4b9c-885b-1fe37ec06f72)

**Truth Table**
![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/6144801e-21b9-444a-8c47-80f5cef26beb)


**Timing Diagram**
![image](https://github.com/SusithraB/BOOLEAN_FUNCTION_MINIMIZATION/assets/146347839/5cbc106d-d6be-4e21-8ead-0c320864ee4e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

