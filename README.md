![pic 1](https://github.com/user-attachments/assets/5664c8ed-052c-4b21-af63-be7b93a44d9d)![pic 1](https://github.com/user-attachments/assets/62c36c1f-f3f1-42d8-9294-0fdd16f00301)# HALF_ADDER_SUBTRACTOR

NAME:P.VIGNESHWARAN

REF NO:24900068

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
![pic 1](https://github.com/user-attachments/assets/2308559c-843e-4519-b928-a9f9b315762a)

![pic 2](https://github.com/user-attachments/assets/08f1f072-8988-4017-b7d7-8f816d19f2f2)






**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
i)HALF ADDER

module ha(a,b,sum,carry);

input a,b;

output sum,carry;

assign sum= (a ^ b);

assign carry= ( a & b);

endmodule

ii)HALF SUBTRACTOR

module hs(a,b,difference,borrow);

input a,b;

output difference,borrow;

assign difference= (a ^ b);

assign borrow= ( ~a & b);

endmodule



Developed by: RegisterNumber:*/

**RTL Schematic**
1)HALF ADDER

![ex -3 1](https://github.com/user-attachments/assets/8886682c-57cb-4a51-bacd-b224d97ed0c3)


**Output/TIMING Waveform**
1)HALF ADDER

![ex -3 2](https://github.com/user-attachments/assets/4603cb67-c70b-42a1-829f-2b267a2945c1)

![ex -3 2](https://github.com/user-attachments/assets/bf465bac-5ca6-42fb-ba95-4b222afafb02)



**Result:**
Thus program is verified sucessfully.
