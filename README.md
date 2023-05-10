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
Developed by: sangavi suresh
RegisterNumber:212222230130  
module halfadder(A,B,C,S);
input A,B;
output S,C;
xor(S,A,B);
and(C,A,B);
endmodule

FULL ADDER:

module fulladd(A,B,Ci,S,Co);
input A,B,Ci;
output S,Co;
wire D,E,F;
xor(D,A,B);
xor(S,D,Ci);
and(E,Ci,D);
and(F,A,B);
or(Co,E,F);
endmodule
*/

Logic symbol & Truthtable

### Output:
RTL realisation

RTL realisation of half adder:
![image](https://github.com/Sangavi-suresh/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118541861/e57aa5c0-3d0b-4636-9615-226ecd5124f4)

RTL realisation of full adder:
![image](https://github.com/Sangavi-suresh/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118541861/05da47b7-e32c-4b0c-be7e-064430b24fc3)

### TIMING DIAGRAM
half adder
![image](https://github.com/Sangavi-suresh/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118541861/9b6a0cd5-2e1e-4fba-bb89-2cce99b784ba)

full adder
a![image](https://github.com/Sangavi-suresh/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118541861/9fde0ab9-1de6-4d66-b14b-70dd2d016a1b)

### TRUTH TABLE 
Truth table of Half adder:
![image](https://github.com/Sangavi-suresh/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118541861/e5f4f895-7bb6-48f7-a4ee-c67a5628db81)

Truth table for full adder:
![image](https://github.com/Sangavi-suresh/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118541861/9f812c1c-5107-4926-a157-72423afe07bc)

### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
