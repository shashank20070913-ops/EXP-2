**Program:**
```
implement F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D, F2=xy’z+x’y’z+w’xy+wx’y+wxy

module ex2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

**Developed by:** shashank s 
**RegisterNumber:** 212225040406


**RTL realization:**
<img width="1187" height="858" alt="Screenshot 2026-08-08 001239" src="https://github.com/user-attachments/assets/0e2285f3-0640-448a-9be1-08205e15c74a" />

**Output:**

**RTL**
<img width="1757" height="495" alt="Screenshot 2026-08-08 001306" src="https://github.com/user-attachments/assets/a1676bf4-494d-4c5c-86d2-67a9f6aff677" />

**Timing Diagram**
<img width="1598" height="901" alt="Screenshot 2026-08-08 001343" src="https://github.com/user-attachments/assets/6d74adcb-10a2-4c1c-8882-db6efa9e9713" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
