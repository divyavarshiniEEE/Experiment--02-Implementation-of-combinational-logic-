# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
* A combinational logic circuit implement logic functions where its output depends only on its current combination of input values. on the other hand sequential circuits,unlike combinational logic, have state or memory.
* some logic operations may require more than one logic gate. Different combinations of gates are designed for different operations. the brhaviour ofvthe combined logic gates can be determined by constructing a truth table of the combined gates.
  

## Logic Diagram
## Procedure
1. create a project with required entities.
2. create a module along with respective file name.
3. run the respective programs for tha given boolean equations.
4. run the module and get the respective RTL otuputs.
5. create a university program(VWF)foe getting timming diagram.
6. give the respective input for the timming diagram and obtain the result.  
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: DIVYAVARSHINI K.S
RegisterNumber:212222050012  
*/

program for F1

module combilogic(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire G1,G2,G3,G4.G5'
assign G1=((~A)&(~B)&(~C)&(~D));
assign G2=((A)&(~C)&(~D));
assign G3=((~B)&(C)&(~D));
assign G4=((~A)&(B)&(C)&(D));
assign G5=((B)&(~C)&(D));
assign F1=G1|G2|G3|G4|G5;
endmodule



program for F2

module combilogic(W,X,Y,Z,F);
input W,X,Y,Z;
output F;
wire G6,G7,G8,G9,G10;
assign G6=((X)&(~Y)&(Z));
assign G7=((~X)&(~Y)&(Z));
assign G8=((~W)&(X)&(Y));
assign G9=((W)&(~X)&(Y));
assign G10=((W)&(X)&(Y));
assign F=G6|G7|G8|G9|G10;
endmodule

## RTL realizatuon:



## Output:



## RTL

output for F1
![RTL F1](https://github.com/divyavarshiniEEE/Experiment--02-Implementation-of-combinational-logic-/assets/128978058/00166dc0-a9f8-42fc-b689-36448c44d147)


output for F2
![RTL F2](https://github.com/divyavarshiniEEE/Experiment--02-Implementation-of-combinational-logic-/assets/128978058/7c851ba3-e9c7-4f7c-acd6-d4a475351104)






## Timing Diagram

for F1
![TIMMING F1](https://github.com/divyavarshiniEEE/Experiment--02-Implementation-of-combinational-logic-/assets/128978058/45a4c026-5e5c-4708-8d9f-71f06a635b53)

for F2
![TIMMING F2](https://github.com/divyavarshiniEEE/Experiment--02-Implementation-of-combinational-logic-/assets/128978058/4a5a3104-80ff-47d3-96b2-8831841cc8a6)




## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
