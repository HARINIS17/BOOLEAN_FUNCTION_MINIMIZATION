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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:HARINI S

RegisterNumber:24900110

module boolean(a, b, c, d, w, x, y, z, f1, f2);

    input a, b, c, d, w, x, y, z;
    
    output f1, f2;
    
    assign #2 f1 = (~a & ~b & ~c & ~d) | (a & ~c & ~d) |    (~b & c & ~d) | (~a & b & c & d) |  (b & ~c & d);

    assign #2 f2 = (x & ~y & z) | (~x & ~y & z) |  (~w & x & y) | (w & ~x & y) |   (w & x & y);
    
endmodule


**RTL realization**

**Output:**
![Screenshot (92)](https://github.com/user-attachments/assets/7e1774ab-aefc-4ab1-af5a-aa899a459fb5)


**RTL**

**Timing Diagram**
![Screenshot (91)](https://github.com/user-attachments/assets/d9a6551a-4bde-457b-9021-8401f999e4b5)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

