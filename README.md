# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Truth table**
<img width="805" height="442" alt="316395754-a9ccb75e-db7b-490e-8b69-10f820e6bff4" src="https://github.com/user-attachments/assets/b66c7fa6-7ca5-4da4-822e-68675ce1b42f" />
<img width="797" height="421" alt="316395946-6835b6c0-9fe5-4f55-8288-53b7d0c42104" src="https://github.com/user-attachments/assets/90490f11-9aea-41b1-bbaa-bab278227024" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule


```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: SAAINATH B RegisterNumber:25016015 */



**Output:**

**RTL**
<img width="1920" height="1080" alt="Screenshot (39)" src="https://github.com/user-attachments/assets/e9849abc-b62b-4080-86f7-e539ee28f535" />

**Timing Diagram**
<img width="1920" height="1080" alt="Screenshot (56)" src="https://github.com/user-attachments/assets/728fe837-0e2d-4193-85a4-7a2f4d5b79c6" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

