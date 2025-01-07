2024-09-0412:53
Status: 
Tags: 

### Overview: 
Broadly how does a function behave as a certain value is approached. 
### Definitions: 
Power Law: A power law is an expression of the form $A\cdot x^n$ (as a function of $x$), where we call $n$ the index: E.g. $x^3, \pi x^{102}, c\sqrt x, - \frac 8 x, \frac 8 {x^{\frac 7 2}}, x^e, \frac A {x^b}$ etc. 
Exponential: An exponential is an expression of the form $C\cdot b ^x$ (as a function of $x$), where $b>0$ and $b$ is known as the base. E.g. $e^{2x}, 7^x, 8\cdot 2^x, -\frac 1 (\sqrt 3) \cdot \frac 1 {2^x}, \pi^x$ etc. 
### Power Law:
![[Pasted image 20240904130702.png]]

As functions get infinitely large, they "blow up" and as they approach 0, they decay. They do so at different rates: for instance in function c, as x approaches infinity (positive and negative), it decays to 0, however when $x$ approaches 0, from the left or right it approaches positive and negative infinity respectively. 

### Asymptotic Comparison 
As $x\to \infty, x^2$ will be much larger than $x$. 
Write $x^2 \gg x$ asymptotically dominates $x$. In other words... 
$\frac 1 {10^6} x^2\gg 10^6 x$ which is to say that constants don't have much bearing on the magnitude of the overall number. Thus, 
As $x \to 0, x \gg x^2$: 

![[Pasted image 20240904131833.png]]

So as $x$ approaches infinity, it does not matter what the constant is. 

Similarly, As $x\to \infty, \frac 1 x\gg \frac 1 {x^-2}$ and $x\to \infty, \frac 1 x\ll\frac 1 {x^-2}$

![[Pasted image 20240904132127.png]]

Where the red function is $|\frac 1 x|$ and the blue function is $\frac 1 {x^2}$

Any exponential growth is much greater than a power law. To get a better idea of asymptotic dominance as $x \to \infty$: 
$$e^{-x} \ll \frac {2024} {x^{100}} \ll x^{-\frac 1 2} \ll x^{-\frac 1 3} \ll \frac {1}{\log x} \ll \log \log x \ll \log x \ll (\log x )^2 \ll 1 \ll \sqrt x \ll x \ll 10^6\cdot x^{2024}\ll e^{\sqrt x} \ll e^x\ll 5^x \ll e^{x^2}$$
Generally, $\log x$, blows up slower than any power law (And any power law grows slower than any exponential law) as $x \to \infty$

As for $x \to 0^+$,
$$10^6 x^{2024}\ll x\ll x ^ {\frac 1 2}\ll x ^ {\frac 1 3}\ll 1 \sim e^x \sim e^{-x} \sim e^{x^2}\sim 5^x \ll x ^{-\frac 1 3} \ll x^ {-\frac 1 2}\ll \frac {2024}{x^{100}} $$
(Solid red then blue then green then orange then (1) purple then black then dashed version) - Observe the behavior at 1 
![[Pasted image 20240904154558.png]]
#### Logarithmic Expressions 


# Source(s)




