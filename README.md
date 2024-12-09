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

Developed by: BHUVANESHWARAN TU 
RegisterNumber:24009351*/


**RTL realization**
code

    modulle logic_functions(
    input A,B,C,D
    input w,x,y,z
    output F1,F2
    );
    assign F1= (~A & ~B & ~C & ~D) | (A & ~C & ~D) | (~B & C & ~D) | (~A & B & C & D) | (B & ~C & D);
    assign F2= (X & ~Y & Z) | (~X & ~Y & Z) | (~W & X & Y) | (W & ~X & Y) | (W & X & Y);
    endmodule

k-map
![Screenshot 2024-12-03 200858](https://github.com/user-attachments/assets/f8d2b3ca-8029-4c5f-9368-c2e4de859be6)
![Screenshot 2024-12-03 201935](https://github.com/user-attachments/assets/5313ff4d-bfd6-4b8f-bc50-e3dea9c3ba7c)

**Output:**

![Screenshot 2024-12-03 204129](https://github.com/user-attachments/assets/ffbc4128-4021-4ba6-b286-0964dfba6ea6)


**RTL**

**Timing Diagram**
![waveform exp 2](https://github.com/user-attachments/assets/422b3c73-5493-431d-b3b6-e7e310b8bdfe)
![waveform  exp 2 (2)](https://github.com/user-attachments/assets/27ace2f6-17c0-4e5a-88f1-c48c01d6fbef)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

