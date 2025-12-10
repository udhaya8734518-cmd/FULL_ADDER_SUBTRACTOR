# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
i)FULL ADDER

module fa(a,b,cin,sum,carry); input a,b,cin; output sum,carry; assign sum=( (a ^ b)^cin); assign carry= ( (a & b)| ( cin &(a ^ b ))); endmodule

ii)FULL SUBTRACTOR

module fs(a,b,bin,difference,borrow); input a,b,bin; output difference,borrow; assign difference= ( (a ^ b)^bin); assign borrow= ( ( a & b)| ( bin & ((a ^ b )))); endmodule
Developed by:UDHAYA GIRI V RegisterNumber:25015458
*/

**RTL Schematic**
<img width="807" height="344" alt="image" src="https://github.com/user-attachments/assets/92ef5084-c882-42eb-826d-51e6488c753f" />
<img width="897" height="248" alt="image" src="https://github.com/user-attachments/assets/852e5ab4-2753-4e88-a5ea-e55ba856c0f7" />

**Output Timing Waveform**
<img width="814" height="243" alt="image" src="https://github.com/user-attachments/assets/ce97e23d-bc66-4b77-bfd8-010b8f7241b0" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



