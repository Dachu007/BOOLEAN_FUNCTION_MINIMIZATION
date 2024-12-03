# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

F1
```
module funct_1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule
```
F2
```
module func(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

Developed by:Dharshini.S RegisterNumber:24900257


**RTL**

F1
![Screenshot (9)](https://github.com/user-attachments/assets/403019be-30f2-4145-8ec4-19d97c21b454)

F2
![Screenshot (12)](https://github.com/user-attachments/assets/b1a9c2b5-72e3-462a-9f2a-009ac33cf037)



**Timing Diagram**

F1
![Screenshot (11)](https://github.com/user-attachments/assets/abb4fd13-5833-484a-b91f-a2caecdd620a)

F2
![Screenshot (13)](https://github.com/user-attachments/assets/dbd886bd-c6b6-4cca-8cdf-cc091a6e5c55)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

