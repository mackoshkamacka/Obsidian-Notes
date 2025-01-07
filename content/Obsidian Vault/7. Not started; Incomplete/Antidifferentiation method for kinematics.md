2024-09-2711:45
Status: #PHYS106 
Tags: [[Kinematics]]

![[Pasted image 20240927111424.png]]

We can use small time steps method to make predictions: https://scratch/mit/edu/projects/576886731/editor
### Antidifferentiation method
This method can be used to find $v(t)$ and $x(t)$ explicitly if $F$ is a known function of time: If force is a known function of time, $\frac F m = a(t)$, then $\frac {dv}{dt}=a(t)$. To find $v(t)$ given $v(t_0)$, find a function $w(t)$ whose derivative is $a(t)$. Then $v(t)=w(t) + C$. Choose the number $C$ so that the velocity at $t=t_0$. 

If force is a known function of time, $\frac{dv}{dt} = f(t)$. To find $v(t)$ given $v(t_0$): Find a function $g(t)$ whose derivative is $f(t)$. Then $v(t) = g(t) + C$. Choose the correct number $C$ so that the velocity at $t=t_0$ is correct. Use the same procedure to find $x(t)$ given $v(t)$ and $x(t_0)$. I.e. $\frac{dx}{dt} =v(t)$. 

Note: constant acceleration is when $a = \frac F m$ is constant: $\frac {dv}{dt}=a$. 
Thus, $\frac {dv}{dt} = a \to v(t)=v_0 + at$. Moreover, 
$\frac {dv}{dt} = v_0 + at \to x = x_0 + v_0t+\frac 1 2 a t^2$. 
This can be derived by remembering the relationship between $x$ and its integral, $v$ and its derivative/integral, and $a$ and its integral (or antidifferentiation). And that $$z_{new} = z_{old}+ \frac {dz}{dt}t $$
Note that $\frac {dx} {dt}$ can be substituted for "velocity". Which has the same general formula. This nesting substitution can go on until there is a constant rate. 
##### Example 
![[Pasted image 20240927111716.png]]

![[Pasted image 20240927112500.png]]

$$\begin{gather} \vec x = \int 2t+1  dx
\\ \vec x= t^2 + t + C
\\ (3) = (1)^2+(1) +C \ \ \ \ \therefore C=1
\\ at \ t=3, \vec x =(3)^2 + 3 + 1 = 13 
\end{gather}$$
