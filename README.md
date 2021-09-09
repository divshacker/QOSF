# QOSF
## Task 1 
Given a vector/array of integer and one need to find the numbers position where (When changed in binary) adjecent bits are opposite of each other. 
Example (Given in task ) [1,5,7,10] so the position will be 01 and 11 as 5 and 10 are correct answers in the array.
[1 5 7 10] = [0001 0101 1110 1010] here only two binary strings are only there 0101 and 1010. We are required to return a praticular state which contains equal probabilities of the correct position in the given array.
In the given array the returned state should be (1/sqrt(2))(|01>+|11>).

## My approach (In Brief)
- Initialisation  (Imported and defined all things)
- QRAM  (Configured QRAM according to given data )
- Oracle (Configured Oracle to check the right solutions)
- QRAM (Same QRAM function as defined before also no need to take care of reverse order as QRAM is commutative)
- Diffuser (Standard Diffuser used in Grover's Algorithm)
- Measurement  (Measure the address qubits)
- Plot and visualization (Running the circuit on qasm_simulator and plotting the results in the form probabilities of all shots)