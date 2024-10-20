![Screenshot 2024-10-20 120100](https://github.com/user-attachments/assets/6fc85c0b-e235-4dc3-b21e-d4738317a925)# FULL_ADDER_SUBTRACTOR

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
# FULL ADDER:

![Screenshot 2024-10-20 120135](https://github.com/user-attachments/assets/01b0aa09-2174-4d11-b3ed-a8aff891eb94)

#  FULL SUBTARCTOR:


![Screenshot 2024-10-20 120151](https://github.com/user-attachments/assets/474f2abd-4c12-4224-93de-651590dbcece)

**Procedure**

Write the detailed procedure here

**Program:**
 # Developed by:PRASANNA I
 # RegisterNumber:212223220079
 # FULL ADDER:
 ```
module proj_41(a,b,cin,sum,carry);
input a,b,cin;
output sum, carry;
assign sum=(a^b^cin);
assign carry=((a&b)|(b&cin)|(cin&a));
endmodule
```


 # FULL SUBTARCTOR:
 ```
module proj_42(a,b,bin,borr,diff);
input a,b,bin;
output diff, borr;
assign diff=(a^b^bin);
assign borr=((~a&b)|(b&bin)|(bin&~a));
endmodule

```

**RTL Schematic**
# FULL ADDER:
![Screenshot 2024-10-20 120100](https://github.com/user-attachments/assets/596521ce-ba77-45f8-9936-ae0f9a765834)





# FULL SUBTARCTOR:
![Screenshot 2024-10-20 120111](https://github.com/user-attachments/assets/916bae75-28e6-4de2-b48e-5eeb1f0e1df4)


**Output Timing Waveform**




# FULL ADDER:

![Screenshot 2024-10-20 120119](https://github.com/user-attachments/assets/fcd79eb5-9ee6-4a17-a55c-fae03925f1df)



# FULL SUBTARCTOR:



![Screenshot 2024-10-20 120125](https://github.com/user-attachments/assets/30f5a160-93c2-4928-8bc9-d8cde444834d)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



