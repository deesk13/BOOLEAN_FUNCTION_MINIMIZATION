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

Developed by:I.DEVA DHARSHINI
RegisterNumber:212223240026
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


**RTL realization**
![Screenshot 2024-03-21 081944](https://github.com/deesk13/BOOLEAN_FUNCTION_MINIMIZATION/assets/150927063/84ee5fbe-3f75-4c59-9cf4-1c6460ad24ea)



**RTL**
![image](https://github.com/deesk13/BOOLEAN_FUNCTION_MINIMIZATION/assets/150927063/3998d01f-ebdb-4feb-9c45-1ffb51e03000)

**Output**
![image](https://github.com/deesk13/BOOLEAN_FUNCTION_MINIMIZATION/assets/150927063/87b30949-c62b-4b22-a744-e5d7a524877e)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

