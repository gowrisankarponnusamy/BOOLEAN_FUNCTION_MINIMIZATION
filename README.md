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

# Developed by: GOWRISANKAR P

# RegisterNumber: 212222230041
*/
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


**RTL realization output**

![image](https://github.com/user-attachments/assets/c50b4b38-94fd-4b87-bc5e-0ca948ae8360)

**LOGIC SYMBOL & Truthtable:**
## TRUTH TABLE FOR F1:

![image](https://github.com/user-attachments/assets/34120d53-35fa-42da-b8fd-0d4e0612272e)

## TRUTH TABLE FOR F2:

![image](https://github.com/user-attachments/assets/be8ae30c-b836-43da-8040-48615e43d25d)

**Timing Diagram**

![image](https://github.com/user-attachments/assets/cb0f608b-bc9e-4a59-9861-8d8c57bd622f)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
