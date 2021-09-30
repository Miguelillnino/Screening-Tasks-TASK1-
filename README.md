Miguel de Jesús Martínez Felipe

Application on September 15th
Solution send on September 29th

# Screening-Tasks-TASK1-
Task from QC Mentorship program

# Task 1

Design a quantum circuit that considers as input the following vector of integers numbers: 
<br>
<br>
[1,5,7,10]
<br>
<br>
returns a quantum state which is a superposition of indices of the target solution, obtaining in the output the indices of the inputs where two adjacent bits will always have different values. In this case the output should be: 1/sqrt(2) * (|01> + |11>) , as the correct indices are 1 and 3.
1 = 0001
5 = 0101
7 = 0111
10 = 1010
The method to follow for this task is to start from an array of integers as input, pass them to a binary representation and you need to find those integers whose binary representation is such that two adjacent bits are different. Once you have found those integers, you must output a superposition of states where each state is a binary representation of the indices of those integers.
