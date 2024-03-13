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
```
module combinationalcircuit(A,B,C,D,F1);
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

Developed by: Manikandan R

RegisterNumber:212223230120


**RTL realization**

**Output:** OUTPUT FOR 1.F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

![image](https://github.com/Manikandanrag/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849491/06f77914-567b-4f6b-bb41-e8f4252391a7)

**Timing Diagram**


![image](https://github.com/Manikandanrag/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849491/df49787a-a60d-411d-863a-8ed09f9fc492)

2.F2=xy’z+x’y’z+w’xy+wx’y+wxy HERE X=A, Y=B , Z=C AND W=D

![image](https://github.com/Manikandanrag/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849491/9eb7d231-dd32-4f16-b742-3dd70d81215a)

**Timing Diagram**

![image](https://github.com/Manikandanrag/BOOLEAN_FUNCTION_MINIMIZATION/assets/138849491/e2d4c193-b11c-408e-849b-ab77766ed2e0)

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

