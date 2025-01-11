2024-12-2618:03
Status: 
Tags: [[Proofs]] [[Discrete mathematics]]
### Course Learning Outcomes 
- Problem modeling 
- Modeling formalisms 
- Problem-solving 
- Communication 
- Characterization of algorithms + correctness/efficiency 
- Proofs 
- Explain how computers work 
---- 
## Modeling 
Propositional logic 
Predicate logic 
Combinational Circuits 
DFA's 
NFA's 
Regular expressions 
Sequential circuits 
## Problem-Solving 
Making the problem more precise
Understanding the problem better 
Reason about the problem 
Provide a solution (if possible)
## Validating Solutions ([[Proofs]])
"Proving arguments to support solutions"
Constructive/non-constructive proofs of existence  
Generalizing from the generic particular 
Antecedent assumption 
Proof by cases 
Proof by contrapositive or other equivalent 
Proof by contradiction 
Induction 
## Reasoning about [[Algorithms]]  
"Reason about simple algorithms" = solutions  
Prove solutions are correct for certain inputs 
Prove how efficient they are 
Compare solutions  
## [[Circuits]]  
## [[Discrete mathematics]]

--- 
## Math Review 
### Divisibility 
$m=n \cdot q + r$
A number is divisible if there is no remainder $r, r=0$
$n$ does not divide $m$, $n \nmid m$ which means that $m$ is not divisible by $n$
$n$ always divide 0, 0 never divides $n$ ($\frac n 0$)
Odd numbers can be expressed as $2k+1$, where $k$ is an integer
Even numbers can be expressed as $2k$, where $k$ is an integer
Prime numbers have no factors but itself and 1, e.g. 2, 3, 5, 7, 11 ...
Composite numbers are not prime numbers
1 is neither a composite number nor a prime number 
A number is divisible by 2 if it is even 
A number is divisible by 3 is the sum of the digits are 
A number is divisible by 5 if it ends with 5 or 0 
A number is divisible by 7 if it 
A number is divisible by 9 if it the sum of the digits are divisible by 9. ($144 = 1+4+4 = 9/9 \therefore 9 | 144$)
### Exponentiation 
The exponentiation $a^n$ is equal to the multiplication of a repeated $n$ times. For the expression $a^n$, $a$ is called the base while $n$ is the exponent (also called the power). 
$a^0 = 1$
$a^1 = a$
$a^\frac 1 2 = \sqrt a$
$a^{-n} = \frac 1 {a^n}$
$a^{n+m} = a^n \cdot a^m$ 
$(a^n)^m= a^{nm}$
$(a\cdot b)^n = a^n\cdot b^n$
See [[Binomial Theorem]] for $(a+b)^n$
### Logarithms 
The inverse operation of exponentiation is the logarithm. If $a^n = c, \log _a c= n$. $\log_2$ is used most often for computer science. 
Applications for logarithms in CS are proofs that require logarithms, processing/delay time for circuits of an arbitrary size, when comparing varying runtime ([[Time complexity]]), Big O Notation. 
$a^{log_a x} = x$ 
$\log _a 1 = 0$
$log_a a = 1$ 
$\log_a(x\cdot y) = \log _a x + \log_a y$
$\log_a(\frac x y) = \log _a x - \log_a y$
$\log _a (x^b) = b \log_a x$$\log _a x = \frac {\log _k x}{\log _k a}$
In general, the larger the base, the slower it grows. E.g. $\log_5$ grows slower than $\log _2$ 
### Inequalities 
To evaluate the runtime of algorithms, inequalities are necessary for proofs. 
An inequality is a relation that makes a comparison between two mathematical expressions. 
*This will be more advanced than high school's application*
If $a\le b$ then $a+c \le b + c$ and $a - c \le b -c$ 
If $a \le b$ then $-a \ge b$. Imagine flipping building heights across a horizon 
If $a \le b$ then $\frac 1 a \ge \frac 1 b$. Take $a =2$ and $b =3$ to see that this is true. 
### Summation 
In order to take the sum of a sequence of numbers, sums are used $\Sigma ^n _{i=0} f(x)$. Basically a for loop where numbers are added to each other. 
$n \Sigma ^5_{n=1} = n \Sigma ^2_{n=1}  + n \Sigma ^5_{n=3}$
### Product 
Similar to summation, product multiplies all the terms: $\Pi ^n _{i=1} f(x)$
### Recursive Functions 
By using the function in its definition, the function repeats itself to complete the remaining terms. A factorial is an example of this.
$n! = n * (n-1) * (n-2) ... * 3 * 2 * 1 = \Pi _{i=1}^n k$
Fibonacci can be defined as $F_n = 1 (where\  n=1,2), and\  F_{n-1} + F_{n-2} otherwise$ 
### Floor and Ceiling 
To take the floor of a real number, truncate the decimals or round down. (If it's already an integer it stays the same) 
$\lfloor \pi \rfloor = 3$, $\lfloor 3 \rfloor = 3$ 
To take the ceiling of a real number, round up to the next integer. (If it's already an integer is stays the same) 
$\lceil \pi \rceil = 3$, $\lceil 3 \rceil = 3$
 