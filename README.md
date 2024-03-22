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

Developed by: GANESH PRABHU J
RegisterNumber: 212223220023
```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
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
```
//type code for f2 as like f1 endmodule


**RTL realization**
![315915944-04f5ba86-5ec6-4c85-9f21-64bb94fd0a76](https://github.com/ganeshprabhu2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/146162190/10c7c9f7-4635-4019-8360-bfac98063b16)


**Output:**
![315914208-e304bd09-b312-4ebc-a65c-8fbf5f32e951](https://github.com/ganeshprabhu2005/BOOLEAN_FUNCTION_MINIMIZATION/assets/146162190/5c1223da-5acb-4ec4-8917-44e475efd3a6)

**RTL**
![Uploading 315913995-cfef8245-474f-4443-bc8e-1eb88554cdbb.png…]()

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

