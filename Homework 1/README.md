Homework 1: Two 4-Bit Adder and Subtractor

Purpose: This circuit can output the sum or difference of two 4-bit numbers, depending on the user input on the "Op" switch.

How To Use:

For the "Op" switch (meaning "Operation"): 0 means Addition (A3 A2 A1 A0) + (B3 B2 B1 B0) = (S3 S2 S1 S0); 1 means Subtraction (A3 A2 A1 A0) - (B3 B2 B1 B0) = (S3 S2 S1 S0)

For 2's Complement, ALWAYS ignore the carry out digit, and focus on the 4-bit binary 2's complement answer (S3 S2 S1 S0). Make sure that (A3 A2 A1 A0) + (B3 B2 B1 B0) <= 0111 and that (A3 A2 A1 A0) - (B3 B2 B1 B0) >= 1000. This is because the range of a 4-bit 2's complement numer is from 1000 (-8 in decimal) to 0111 (+7 in decimal) inclusive. Any answers outside that range would produce overflow, demonstrating that the answer would be incorrect.

For Unsigned, ALWAYS ignore the carry out digit, and focus on the 4-bit binary unsigned answer (S3 S2 S1 S0). Make sure that (A3 A2 A1 A0) + (B3 B2 B1 B0) <= 1111 and that (A3 A2 A1 A0) - (B3 B2 B1 B0) >= 0000. This is because the range of a 4-bit unsigned number is from 0000 (0 in decimal) to 1111 (+15 in decimal) inclusive. Any answers outside of that range would produce overflow, demonstrating that the answer would be incorrect.
