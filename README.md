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
![WhatsApp Image 2024-12-09 at 23 12 53_dac3d2d0](https://github.com/user-attachments/asse![WhatsApp Image 2024-12-09 at 23 12 54_eda5c472](https://github.com/user-attachments/assets/294dba4e-e20f-421a-ae2e-a6878a4adad0)
ts/4cd1d38a-c715-4023-baed-6ddabce72ef1)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**


Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:shaiklahir RegisterNumber:24005737
        
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
![Screenshot 2024-11-15 132441](https://github.com/user-attachments/assets/34d4ef78-5b8f-498f-9c2a-ff9f814c033a)
![Screenshot 2024-11-15 134410](https://github.com/user-attachments/assets/a3288490-bfb1-43b9-8223-1c056351edc4)

**TIMING Waveform**
![Screenshot (13)](https://github.com/user-attachments/assets/fee3b88e-8da4-4536-b158-61048076d93e)
![Screenshot 2024-11-15 134558](https://github.com/user-attachments/assets/1735d4af-956c-4482-89ed-fe0162d4f9bc)

**Result:**
Thus the Half and Full Adders are studied and the truth tables are verified.
Thus the Half and Full Subtractors are studied and the truth tables are verified.
