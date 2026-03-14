# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module de2(
    input A, B, C, D,
    output F
);

assign F = (~A & ~B & ~C & ~D) |   
           ( A & ~C & ~D )     |   
           (~B &  C & ~D )     |    
           (~A &  B &  C &  D) |   
           ( B & ~C &  D );      

endmodule
```
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:VIGNESH J
RegisterNumber:212225230297
/*
```

**RTL realization**
<img width="811" height="555" alt="Screenshot 2026-03-12 103814" src="https://github.com/user-attachments/assets/c16cf170-9477-45f9-870c-d4f6ee0aa233" />


**RTL**
<img width="1907" height="918" alt="AdobeExpressPhotos_10c81cd5309c45569820a37832c2cc5a_CopyEdited" src="https://github.com/user-attachments/assets/881f1b27-0ad1-4bdc-9334-208601fe2055" />


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

