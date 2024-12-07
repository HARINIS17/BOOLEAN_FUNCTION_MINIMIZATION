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

Logic diagram for f1:

![WhatsApp Image 2024-12-06 at 8 19 31 PM](https://github.com/user-attachments/assets/3a10df26-31d0-4d85-b3bb-3d70e3bb3d39)

Logic diagram for f2:

![WhatsApp Image 2024-12-06 at 8 27 14 PM](https://github.com/user-attachments/assets/24aa4902-4ade-4396-b859-0c3a1e766ac5)

**Truth Table**

Truth table for f1:

![Screenshot (6)](https://github.com/user-attachments/assets/8495451a-b10a-49c0-a6e0-4ae10b42e980)

Truth table for f2:

![Screenshot (7)](https://github.com/user-attachments/assets/08652220-16c5-4bd6-8fcb-1ea26490fab0)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: HARINI S

RegisterNumber:24900110

module boolean(a, b, c, d, w, x, y, z, f1, f2);

input a, b, c, d, w, x, y, z;
    
output f1, f2;
    
 assign #2 f1 = (~a & ~b & ~c & ~d) | (a & ~c & ~d) |    (~b & c & ~d) | (~a & b & c & d) |  (b & ~c & d);

 assign #2 f2 = (x & ~y & z) | (~x & ~y & z) |  (~w & x & y) | (w & ~x & y) |   (w & x & y);
    
endmodule


**RTL realization**

**Output:**

![Screenshot (5)](https://github.com/user-attachments/assets/f471cfc7-e960-4ed5-8565-bb6a55aedc0b)



**RTL**

**Timing Diagram**

![Screenshot (4)](https://github.com/user-attachments/assets/a3055402-579a-491d-8a7b-d5416ded9a35)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

