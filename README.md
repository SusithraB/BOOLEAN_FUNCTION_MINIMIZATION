
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
module booleanfun(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
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

