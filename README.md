NAME: BLESSING JEFFREY Y.L<br>
REFERENCE NUMBER: 212223220014
# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/79546dc8-1196-4f62-82e9-3e504d9034ee)

#### Figure -01 HALF ADDER 

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/ec6faec5-401d-4068-a9f9-fb6fa413eaff)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows. 

Program:
# Half Adder:


module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule



# Full Adder


module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule



### TRUTH TABLE 
Half Adder Circuit:

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/4081b06d-2771-4a88-bd2b-7cd41cf63742)

Full Adder Circuit:-

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/d0b9a62d-42f6-45ab-800c-c9d402aaa8f2)

### RTL
Half Adder Circuit:

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/6bfb4aba-6a02-4e03-b160-e122ca77a462)

Full Adder Circuit:-

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/b8e4fa3d-6957-4139-816e-aa26844adda9)


### Output:
Half Adder Circuit:-

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/6310e7fa-94f7-4d9f-a51d-9d71d065c9d8)

Full Adder Circuit:-

![image](https://github.com/blessingjeffrey/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149134943/b37752e1-eebd-478d-a4cd-18d0cbecfe46)

### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
