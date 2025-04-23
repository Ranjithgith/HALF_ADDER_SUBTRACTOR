NAME: Ranjith R 

REG NO: 212224240131

# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

![Screenshot 2025-04-15 203551](https://github.com/user-attachments/assets/0f95c2aa-0408-4c79-a59a-8e7efad1defb)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

```
module digital3(a,b,sum,carry);  
input a,b;   
output sum,carry;  
assign sum=(a^b);   
assign carry=(a&b);  
endmodule 
```

```

module exp3(c,d,diff,borr);  
input c,d;   
output diff,borr;  
assign diff=(c^d);   
assign borr=(~c&d);  
endmodule  

```

**RTL Schematic**

![Screenshot (44)](https://github.com/user-attachments/assets/b5431187-6063-4460-b7f8-bfca9d2b88b3)

![Screenshot (41)](https://github.com/user-attachments/assets/4a0950b2-7ada-4858-b2ec-126770c371ad)



**Output/TIMING Waveform**
![Screenshot (45)](https://github.com/user-attachments/assets/337dfbfb-83e4-4855-83e3-fa20155ca460)

![Screenshot (43)](https://github.com/user-attachments/assets/93182851-3428-4f70-b1fd-101eff1f4d31)


**Result:**

Thus designing a half adder and half subtractor circuit and its truth table is verified in Quartus using verilog programming.
