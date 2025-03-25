NAME: YUVASHREE R

REG NO: 212224040378

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
module
logic(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~a)&(~b)&(~c)&(~d))|(a&
(~c)&(~d))|(~b)&c&(~d)|((~a)&b&c&d)|
(b&(~c)&d);
assign f2=(x&(~y)&z)|((~x)&(~y)&z)|
((~w)&x&y)|(w&x&(~y))|(w&x&y);
endmodule

```

Logic symbol & truth table:

![lt1](https://github.com/user-attachments/assets/b08c63b4-8a86-464e-807b-1a7a04745977)

![it2](https://github.com/user-attachments/assets/48da70f7-88f8-4563-8b2d-1410f1de09b2)



**RTL realization**

![Screenshot 2025-03-25 213715](https://github.com/user-attachments/assets/823dc6f7-cb36-472d-b64f-21a238384fe7)


**RTL Waveform**
![Screenshot 2025-03-25 215307](https://github.com/user-attachments/assets/9d2f16db-44f2-4ecd-9bc8-3fb0ff2c0828)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

