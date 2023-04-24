# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Tejusve Kabeer.F
RegisterNumber: 212222100054
```python
module ha(x,y,s,c);
input x,y;
output s,c;
xor(s,x,y);
and(c,x,y);
endmodule

module full_adder(x, y, z, s, c, x1, x2, x3);
input x,  y,z;
output s ,c, x1, x2, x3;
xor(x1, x, y);
xor(s, x1, z);
and(x2, x, y);
and(x3, x1, z);
or(c, x2, x3);
endmodule
```
*/
Logic symbol & Truthtable
RTL realization

## Output:

## RTL
### Half Adder
![Screenshot (54)](https://user-images.githubusercontent.com/118364993/233892475-78a7c4f5-381a-42b9-a092-f39cb3febfcb.png)

### Full Adder
![Screenshot (55)](https://user-images.githubusercontent.com/118364993/233892353-114d5d67-ab3b-4ebe-ad44-cf1b6976dbcf.png)

## TIMING DIAGRAM
### Half Adder
![Screenshot (56)](https://user-images.githubusercontent.com/118364993/233892672-c06bc1ff-1e40-46a9-8da0-7c4734c772e5.png)

### Full Adder
![Screenshot (57)](https://user-images.githubusercontent.com/118364993/233893015-3b9b193b-5552-477f-9d68-f598985c3bb1.png)

## TRUTH TABLE 
![Screenshot (58)](https://user-images.githubusercontent.com/118364993/233893210-2efcd2e1-df8a-4c92-9b6a-ee75a2eee871.png)

## Result:
Therefore,half adder and full adder is verified
