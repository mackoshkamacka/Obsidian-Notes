## Simplifying a Logic Gate
### Brute force method
When given a circuit, looking at the output gates to the inputs can give an algebraic expression for the circuit

![[Pasted image 20250120200414.png]]
$$\begin{gather}
y=(A \wedge \neg B )
\\ y= ((C\vee D )\wedge \neg B)
\\ y = ((C\vee D )\wedge \neg (D \oplus E))
\\ y = (((x_1 \oplus x_3)\vee D )\wedge \neg (D \oplus E))
\\ y = (((x_1 \oplus x_3)\vee (x_1 \oplus x_2))\wedge \neg (D \oplus E))
\\ y = (((x_1 \oplus x_3)\vee (x_1 \oplus x_2))\wedge \neg ((x_1 \oplus x_2) \oplus E)) \\
\\ y = (((x_1 \oplus x_3)\vee (x_1 \oplus x_2))\wedge \neg ((x_1 \oplus x_2) \oplus (x_3\oplus x_4))
\end{gather}$$
This method can be verbose, and is typically used when other methods of simplification do not work. 
### Pattern Method

An alternative way to see how this circuit behaves (or can be simplified into) is by looking for patterns in the inputs that entail a true result.  
![[Pasted image 20250120201214.png]]
![[Pasted image 20250120201325.png]]

