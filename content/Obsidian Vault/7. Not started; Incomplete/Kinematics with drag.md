2024-09-2421:06
Status: #PHYS106 
Tags: [[Kinematics]]
###### Alternative Definitions of Newton's Second Law
Newton's Second Law: the rate of change of momentum is equal to the net force on that object:  $\frac {d \vec p} {dt}= \vec F_{net}$. A more familiar version would be: $\vec{F_{net}}=m\vec a$. However, the most useful formulation is: 
$$\frac {d\vec v}{dt}=\frac {\vec{F}_{net}}{m} $$
Newton's 2nd law: $\frac {d\vec{v}}{dt}=\frac 1 m \vec{F}_{net}$ Where we must calculate this from $\vec x, \vec v$ and knowledge of the environment. This gives us the definition of velocity (by cancelling $m$): $\frac {d\vec x}{dt}=\vec v$. In other words, 
- The rate of change of position is equal to the velocity 
- The rate of change of velocity is equal to the force over mass (force can be calculated from position, velocity and knowledge of the environment)
(This is true for each component)

In a small amount of time $\delta t$: 
- Position changes by $\vec v \delta t$ where $\vec v$ is the rate of change of position: 
  $\vec x_{new}=\vec x_{old} + v\delta t$
- Velocity changes by $\frac {\vec F} m \delta t$ where $\frac {\vec F} m$ is the rate of change of velocity
  $\vec v_{new} = \vec v_{old} + \frac {\vec F} m \delta t$
We can predict the future $\vec x, \vec v$ from present $\vec x, \vec v$: 
##### Predicting the Future
![[Pasted image 20240923112717.png]]![[Pasted image 20240923112730.png]]
![[Pasted image 20240923112743.png]]
![[Pasted image 20240923112757.png]]
![[Pasted image 20240923112809.png]]
![[Pasted image 20240923112821.png]]
![[Pasted image 20240923112834.png]]
![[Pasted image 20240923112852.png]]

##### Example: Projectile Motion with Air Drag (Air Resistance)
![[Pasted image 20240923113026.png]]
![[Pasted image 20240923113113.png]]

https://www.youtube.com/watch?v=pW0JfEBE9h8 = "Dynamics and Control of Flow around Circular Cylinder" - This is very complicated so we will use the following approximation (objects of low velocity, size, + depends on viscosity - Reynold's number). 

For small velocities, viscous fluids, and small objects use: 
$$|F_{drag}\approx bv|$$
For large velocities, less viscous fluids, and large objects use: 
$$|\vec{F}_{drag}\approx cv^2|$$
Where $b$ and $c$ are numbers: measured experimentally and $v$ is the velocity

| Time  | Position x | Velocity v                             | Force F  |
| ----- | ---------- | -------------------------------------- | -------- |
| 0 s   | 2 m        | 3 m/s                                  | - 1.5 N  |
| 0.1 s | 2.3 m      | 2.95 m/s (3m/s + (-1.5N / 3kg) * 0.1s) | //////// |
| 0.2 s | ...        |                                        |          |
$$x_{new} = x_{old} + v \delta t \ \ \ \ \ v_{new} = v_{old} + \frac Fm \delta t$$
Doing this process by hand is very laborious, so computers often do this, 
https://www.youtube.com/watch?v=GMmNKUlXXDs&t=1s

