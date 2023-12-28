# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

## Theory

 Logic gates are electronic circuits which perform logical function on one or more inputs to produce one output.

## Logic Diagram

![285640765-45817589-6ade-49e7-bdaa-20886e99e840](https://github.com/jesu-smartia05/Experiment--02-Implementation-of-combinational-logic-/assets/148514819/0863971e-5a6f-4299-b263-07a9df05eaed)


![285640774-c173b0ce-4bdb-4801-9b2d-81b74c538b79](https://github.com/jesu-smartia05/Experiment--02-Implementation-of-combinational-logic-/assets/148514819/c377c9ab-c98f-4f4a-85ad-3fdb2e900ac4)


## Procedure
*Create a project with required entities. *Create a module along with respective file name. 
*Run the respective programs for the given boolean equations. 
*Run the module and get the respective RTL outputs. 
*Create university program(VWF) for getting timing diagram. 
*Give the respective inputs for timing diagram and obtain the results.

## Program:
/*
## Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
### Developed by: JESU SMARTIA A
### RegisterNumber:  212223110016

module combinational(a,b,c,d,w,x,y,z,fl,f2);
input a,b,c,d,w,x,y,z;
output fl,f2;
wire g1=((~a)&(~b)&(~c)&(~d)); 
wire g2=((a)&(~c)&(~d));
wire g3=((~b)&(c)&(~d));
wire g4=((~a)&(b)&(c)&(d)); 
wire g5=((b)&(~c)&(d));
assign fl=g1|g2|g3|g4|g5; 
wire g6=((x)&(~y)&(z));
wire g7=((~x)&(~y)&(z));
wire g8=((~w)&(x)&(y)); 
wire g9=((w)&(~x)&(y));
wire g10=((w)&(x)&(y)); 
assign f2=g6|g7|g8|g9|g10;
endmodule

*/
# Output:

## RTL realization of NAND AND NOR gates:

![285640807-bdbc50f4-a5fd-4a9e-9a30-fd2090ed984d](https://github.com/jesu-smartia05/Experiment--02-Implementation-of-combinational-logic-/assets/148514819/04330c0e-55fa-419a-879f-63d09404c598)


## Truthtable of NAND gate:

![285639665-24364ce7-4c4e-4482-951d-394a31e2cbf0](https://github.com/jesu-smartia05/Experiment--02-Implementation-of-combinational-logic-/assets/148514819/024eb439-9ab5-4776-9956-e69e0a4227bf)

## Truthtable of NOR gate:

![285639708-bfd0a856-c799-472e-a543-a7987bbc5304](https://github.com/jesu-smartia05/Experiment--02-Implementation-of-combinational-logic-/assets/148514819/182038ef-8791-44f3-8901-20f5564294f6)


## Timing Diagram

![285639511-b12d744e-2043-42ad-adc7-96d70c2a7c71](https://github.com/jesu-smartia05/Experiment--02-Implementation-of-combinational-logic-/assets/148514819/d686cee2-c4cd-4bce-91a3-2ecfddf0c6af)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
