Miguel de Jesús Martínez Felipe

Application on September 15th
<br>
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
<br>
1 = 0001
<br>
5 = 0101
<br>
7 = 0111
<br>
10 = 1010
<br>
<br>
The method to follow for this task is to start from an array of integers as input, pass them to a binary representation and you need to find those integers whose binary representation is such that two adjacent bits are different. Once you have found those integers, you must output a superposition of states where each state is a binary representation of the indices of those integers.
<br>
<br>
Example 1
<br>
<br>
Consider the vector [1,5,4,2]
<br>
<br>
Pass the integer values to binary numbers that is [001,101,100,010]
<br>
<br>
Identifies which values whose binary representation is such that two adjacent bits are different, we can see that are 2 101 and 010, [001,101,100,010].
Returns the linear combination of the indices in which the values satisfying the criterion are found.
<br>
<br>
 The answer would be the superposition of the states |01> and |11> or 1/sqrt(2) * (|01> + |11>)
 
 
 # Solution
 The present Task, was made with the following implementations:
 
 ## Superposition
 It deals with the superposition property in quantum computing, in order to store the numbers of the vectors.
 ## QRam
 QRam was implemented in order to storage one number from the vector given in a posiion (memory cell adress).
 <br>
 https://arxiv.org/pdf/0708.1879.pdf, https://github.com/qsharp-community/qram/blob/master/docs/primer.pdf)
 ## Oracle
 The Oracle was implemented as a part of Grover algorithm to add a negative phase to the solution states. 
 ## Grover
Gorver algorithm was implemented to apply the oracle reflection; In order to complete the circuit we need to implement the additional reflection
 https://arxiv.org/abs/quant-ph/9605043 https://arxiv.org/abs/1703.10535
