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
Developed by: JEECIKASRINA M
RegisterNumber: 23013947 


##  CODE:
```
Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
```
Full adder program:
```
module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```
##  TRUTH TABLE:
HALF ADDER TRUTH TABLE:

![image](https://github.com/Jeecikasrina23013947/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148515300/9be864b5-5285-4d6e-bdfd-ec60fb430c5a)

FULL ADDER TRUTH TABLE:

![image](https://github.com/Jeecikasrina23013947/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148515300/9ebb53a2-d304-4627-a697-b49afc2ae1ee)


##  RTL VIEW:

HALF ADDER RTL VIEW:

![image](https://github.com/Jeecikasrina23013947/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148515300/905be14c-70ae-410d-abbb-381627391ece)

FULL ADDER RTL VIEW:

![image](https://github.com/Jeecikasrina23013947/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148515300/6302558b-714f-466f-a2bc-8c80efa98749)


##  OUTPUT:

HALF ADDER:

![image](https://github.com/Jeecikasrina23013947/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148515300/bd71104a-543a-4ccd-90a2-d65af4c5326a)

FULL ADDER:


![image](https://github.com/Jeecikasrina23013947/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/148515300/9adb8ada-f979-481f-83a8-60281afed480)


##  Result:

Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
