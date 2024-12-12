# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**
![WhatsApp Image 2024-12-13 at 07 26 44_ef86ab1c](https://github.com/user-attachments/assets/d9ca9f2c-5eb6-485a-922b-07692d49c3f3)

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**
![WhatsApp Image 2024-12-13 at 07 26 45_408f3253](https://github.com/user-attachments/assets/0a1a1d9a-17c9-4ddb-97fb-2d4535d128d0)

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

Figure -02 HALF Subtractor
![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)
**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:n.v mohan krishna
RegisterNumber:24000587

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

**RTL Schematic**
![Screenshot 2024-11-16 013022](https://github.com/user-attachments/assets/38365f81-0450-41fe-b54a-481044af6c91)
![Screenshot 2024-11-16 014525](https://github.com/user-attachments/assets/eb654845-6af2-46a6-b20f-f9f62a023ae6)

**TIMING Waveform**
![Screenshot 2024-11-16 013408](https://github.com/user-attachments/assets/25246edc-9e35-4141-a051-632f943b9312)
![ex-3hs](https://github.com/user-attachments/assets/3c30f87f-a7e2-4c84-b83c-4af9b9fe25e1)

**Result:**
