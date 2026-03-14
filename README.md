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
module boolean_function_4var (
    input  wire A,
    input  wire B,
    input  wire C,
    input  wire D,
    output wire F
);

assign F = (~A & B) | (C & D) | (A & ~D);

endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: VIGNESH J RegisterNumber:212225230297

**Output:**
<img width="1037" height="562" alt="image" src="https://github.com/user-attachments/assets/6584f285-8f84-4e53-b0da-92f726a37f80" />

**RTL realization**
<img width="1037" height="268" alt="image" src="https://github.com/user-attachments/assets/e8787255-9869-4f43-a53e-016ea976aed7" />

**Timing Diagram**

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

