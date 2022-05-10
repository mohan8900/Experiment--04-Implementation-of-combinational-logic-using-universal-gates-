# Experiment--04-Implementation-of-combinational-logic-using-universal-gates-
 ## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.
F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate


## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

## Theory:
A universal gate is a logic gate which can implement any Boolean function without the need to use any other type of logic gate. The NOR gate and NAND gate are universal gates. This means that you can create any logical Boolean expression using only NOR gates or only NAND gates. In practice, this is advantageous since NOR and NAND gates are economical and easier to fabricate than other logic gates. Similarly, an OR gate is typically realised as a NOR gate followed by an inverter.
A universal gate is a logic gate which can implement any Boolean function without the need to use any other type of logic gate. The NOR gate and NAND gate are universal gates. This means that you can create any logical Boolean expression using only NOR gates or only NAND gates. In practice, this is advantageous since NOR and NAND gates are economical and easier to fabricate than other logic gates. Similarly, an OR gate is typically realised as a NOR gate followed by an inverter.
 


## Procedure

1.Create a project with required entities.

2.Create a module along with respective file name.

3.Run the respective programs for the given boolean equations.

4.Run the module and get the respective RTL outputs.

5.Create university program(VWF) for getting timing diagram.

6.Give the respective inputs for timing diagram and obtain the results.

## Program:
/*
Program to design a Implementation of combinational logic using universal gates-  and verify its truth table in quartus using Verilog programming.
Developed by: A K mohan raj  
RegisterNumber: 212221230064
*/
```
NAND GATE PROGRAM:

module un1(a,b,c,d,f);
input a,b,c,d;
output f;
assign  f=((~(~c&b&a))&(~(~d&c&a))&(~(c&(~b)&a)));
endmodule
```

## Output:

## Truthtable(F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate)


![git log](m1.jpeg)



##  RTL realization(F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate)


![git log](m2.jpeg)


## Timing diagram (F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate)


![git log](m3.jpeg)

### Program:
 
Program to design a Implementation of combinational logic using universal gates-  and verify its truth table in quartus using Verilog programming.
Developed by:A K MOHN ARAJ 
RegisterNumber:  212221230064

```
NOR GATE PROGRAM:
module nor1(a,b,c,d,f);
input a,b,c,d;
output f;
assign  f=(~(~((c&(~b)&a)|(d&(~c)&a)|(c&(~b)&a))));
endmodule
```
## Truthtable(f=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' USING NOR GATE)


![git log](m4.png)

## RTL realization(f=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'USING NOR GATE)


![git log](m5.jpeg)

## Timing diagram (f=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'USING NOR GATE)

![git log](m6.jpeg)


## Result:


The given logic function is implemented using NAND and NOR gates and it is verified successfully in Quartus using Verilog programming.
