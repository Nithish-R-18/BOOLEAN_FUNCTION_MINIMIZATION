# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**
```
Boolean function minimization is the process of simplifying a Boolean expression to its most basic form, using the fewest logic gates, variables, and operators. This is critical for digital circuit design as it leads to more efficient, faster, and cheaper circuits by reducing complexity, power consumption, and manufacturing costs. Key methods for achieving minimization include algebraic manipulation and the use of a Karnaugh map (K-map).
```

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

1.
```
module DE2(a,b,c,d,f1); 
input a,b,c,d; 
output f1; 
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c)); 
endmodule 

```
2.
```
module DE2(w,x,y,z,f2); 
input w,x,y,z; 
output f2; 
assign f2=((~y & z)|( w & y )|(x & y)); 
endmodule

```

**RTL realization**


1.![alt text](<LOGICAL DIAGRAM 2.1.png>)

2.![alt text](<LOGICAL DIAGRAM 2.2.png>)

**Output:**

1.![alt text](<WAVEFORM 2.1.png>)

2.![alt text](<WAVEFORM 2.2.png>)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

