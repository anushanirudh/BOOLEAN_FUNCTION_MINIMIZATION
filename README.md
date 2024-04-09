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

Developed by:R Anirudh  RegisterNumber: 212223230016
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




**RTL realization**

![Screenshot 2024-04-09 133246](https://github.com/anushanirudh/BOOLEAN_FUNCTION_MINIMIZATION/assets/151725737/581a8ff5-a232-45af-bfdd-244c384f851e)

**Truth Table**

![Screenshot 2024-04-09 133505](https://github.com/anushanirudh/BOOLEAN_FUNCTION_MINIMIZATION/assets/151725737/3aea14b1-3930-4ac9-a8e2-796c994c8710)

![Screenshot 2024-04-09 133554](https://github.com/anushanirudh/BOOLEAN_FUNCTION_MINIMIZATION/assets/151725737/fda34394-46da-4070-a645-26bd9179cf5c)


**Output:**

![Screenshot 2024-04-09 133637](https://github.com/anushanirudh/BOOLEAN_FUNCTION_MINIMIZATION/assets/151725737/9801db89-16f6-4ccd-9345-bbba553937c1)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

