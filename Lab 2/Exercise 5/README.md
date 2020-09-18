Exercise 5: Adders

Purpose:
This circuit takes in two 4-bit numbers (A B C D and E F G H) and adds them together to output a 4-bit number (S3 S2 S1 S0).

How to Use:

Input: First, choose the context of your 4-bit numbers. 0 means the Unsigned Number System; 1 means the 2's Complement Number System. Second, input the two 4-bit numbers that you want to add together. The first 4-bit number can be put into the first hex keyboard (A B C D), and the second 4-bit number can be put into the second keyboard (E F G H).
	
Output:

For unsigned numbers, ALWAYS ignore the Cout output because the Cout digit would make the number a 5-bit number. The "Invalid" binary probe will display a 1 if there is overflow, meaning that the answer given is invalid. Otherwise, it will display a 0. Overflow will occur when the correct answer surpasses 1111. This is because 4-bit unsigned numbers range from 0000 to 1111, meaning that if any answer surpasses 1111, it will not be correctly represented by a 4-bit unsigned number. No need to worry about surpassing 0000 since all the hex inputs are positive numbers, so adding positive numbers will only produce positive numbers.
      
    Examples:
      0000+0001=0001; Invalid=0
        Since the correct answer is within the range from 0000 to 1111, then the answer is valid, displaying a 0 for the "Invalid" probe.
      1111+1111=1110; Invalid=1
        Since the correct answer is not within the range from 0000 to 1111, then the answer is invalid, displaying a 1 for the "Invalid" probe.

For 2's complement numbers, ALWAYS ignore the Cout output because the Cout digit would make the number a 5-bit number. The "Invalid" binary probe will display a 1 if there is overflow, meaning that the answer given is invalid. Otherwise, it will display a 0. Overflow will occur when the correct answer goes outside the range 1000 to 0111. This is because 4-bit 2's complement numbers range from 1000 to 0111, meaning that if any answer goes outside the bounds of 1000 to 0111, it will not be correctly represented by a 4-bit 2's complement number.

	Examples:
	  0100+0011=0111; Invalid=0
                Since the correct answer is within the range from 1000 to 0111, then the answer is valid, displaying a 0 for the "Invalid" probe.
          0100+0100=0000; Invalid=1
                Since the correct answer is not within the range from 1000 to 0111, then the answer is invalid displaying a 1 for the "Invalid" probe.
          1000+0111=1111; Invalid=0
                Since the correct answer is within the range from 1000 to 0111, then the answer is valid, displaying a 0 for the "Invalid" probe.
          1010+1010=0100; Invalid=1
                Since the correct answer is not within the range from 1000 to 0111, then the answer is invalid, displaying a 1 for the "Invalid" probe.
