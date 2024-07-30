2024-07-1617:50
Status: #IBnotes 
Tags: [[Redox & Electrochemistry]]

A voltaic cell is an energy source where a reduction half reaction and oxidation half reaction are separated to allow the electrons to flow through an electrical circuit from anode (o1/2) to cathode (r1/2). The voltage could be calculated by finding the difference between the two half reactions’ voltages (balancing the electrons has no bearing on the voltage of the reaction).
### $V=IR$
Potential difference (Potential, Difference, Voltage), $V$ is a measure of energy that is given our as each unit of charge passes between two points. (Think of it as gravitational potential). It is measured in coulombs per second $C/s$.

The current is the rate of electrons, measured in Amperes, Amps (A) = $C/s$

Resistance is how hard it is for electrons to pass through a metal. It is more formally due to the collisions between the delocalized electrons and the cations that get in the way of the electrons moving through the metal. Think of a material with a high resistance as a road with too many cars or a narrow road. Compare that to a 26 lane highway where “people go faster with more lanes” - just pretend that this is actually true (I hate that I think in Albertan).

Resistance is also the ratio of potential difference across a component and the current passing through it: $V=IR$.

## $E-V=Ir$
The electromotive force, $E$ is the theoretical energy made available by the chemical reaction. Not all energy is transferred primarily due to internal resistance, $r$. The terminal potential, $V$ is always less than the electromotive force as energy is always lost to friction and never gained.

If you substitute the previous definition of voltage into this:

$$ E-V=Ir \\ E-(IR) = Ir \\E=I(R+r) $$

If the resistance is 1, then the internal resistance is 0 and the current is equal to the electromotive force: meaning that there are no collisions (or energy lost to resistance) between the cations and delocalized electrons. Because of their relationship the sum of the internal resistance and the resistance is equal to one.

The resistance and internal resistance depend on the nature of the cells, temperature of the solution, and the electrolyte concentrations within the cell.

## Nernst Equation: $E=E\degree -(\frac {RT}{nF})lnQ$
If $E\degree > 0$ then the reaction is spontaneous. So $G<0$ Gibbs Free Energy is negative for spontaneous reactions, meaning that the system is using its own free energy to do work. Inversely, if Gibbs free energy is positive, it needs the energy of the surroundings to commence, nonspontaneous. The standard potential is based on $\frac {1-mol} L$ at $C\degree$.

(Gibbs free energy is the energy available (free) to do work)

Recall the reaction quotient, $Q$ is the measure of $[product]$ to $[reactant]$ in the same relationship as $K_c$, but with non equilibrium concentrations ($aA+bB\rightleftharpoons cC+dD \to Q=\frac {[C]^c[D]^d}{[A]^a[B]^b}$). If $Q>K_c$ then the reaction favors the products, if $Q<K_c$, the reaction favors the reactants, and if $Q=K_c$ then the reaction is at equilibrium. If the reaction is spontaneous then it will favor the products, if it is nonspontaneous, then it will favor the reactants.

Just memorize the equation: $E=E\degree -(\frac {RT}{nF})lnQ$ - this is the Nernst equation. Where $E$ is the actual energy potential, $E\degree$ is the theoretical potential, $R =8.3145...$, $T$ is the temperature in $K$, $n$ is the amount of electrons transferred in the half reaction (mol of electrons per mol of substance), $F$ is Faraday’s constant = $96,485 C/mol_{e^-}$, and $Q$ is the reaction quotient.

There is another formula:

$$\begin{gather} \Delta G =\Delta G\degree + RT\ln Q\\-nFE=-nFE\degree + RT \frac {log Q} {\log e} \\ E=E \degree \frac {8.3145\cdot298}{n\cdot 96485} \cdot \frac {\log Q}{0.43429...} \\ \therefore E=E\degree -\frac {0.0591\log Q} n \end{gather}$$

Battery life and its effectiveness is related to its **change** in Gibbs Free Energy in addition to temperature, concentrations, and nature of compounds.

The total work obtained from a cell depends on the quantity of the materials used. All processes lose energy as heat, this is to increase the entropy of the universe: $q=-T\Delta S$. The amount of energy available increases with the number of electrons transferred. The total work can be obtained from a cell depends on the quantity of the materials.

$$ Power= \frac {Work} {time} = \frac {Voltage \cdot charge } {time} = VI $$

Larger batteries deliver more power as they deliver more charge per unit time. Increasing the size of the electrodes decreases internal resistance, so more power is delivered as current is increased.

## Types of Cells

### Primary Cells: Nonchargeable

These contain materials that will not be reversed in reactions. These can be minuscule so they have good applications in small devices (hearing aids, watches, radio transmitters etc.)

### Lead Acid Batteries (Secondary Cells)

They provide a significant amount of energy (high current) in short bursts. The solid product $PbSO_{4(s)}$ remains on the electrodes which makes recharging impossible. They have limited recharge cycles so must be replaced and recycled ($Pb_{(s)}$ is bad for the environment).

### $NiCad$ Batteries

These are smaller and have low internal resistances which allows for quicker recharging, but are very toxic. The first principle of rechargeable batteries, these had issues with reducing potential charge if you recharged too early.

### Lithium-ion Batteries
These are super reactive lithium atoms in non-aqueous state (polymer) and can hold charge and recharge better than $NiCad$. $Li_{(s)}$ and all group 1 and 2 metals are SRA's but do not make for good electrodes (anodes) because they will react with water if aqueous. Instead, polymers are used to isolate the solid lithium and gain voltage. The SOA in A lithium battery varies. Additionally, there is a reduced by not zero risk of fire with these kinds of batteries.

### Hydrogen Fuel Cells
These are incredibly expensive, but make harmless water as a product. They can be in a completely sealed alkali environment using porous carbon electrodes coated in platinum or palladium catalysts. Fuel cells require a constant supply of fuel. We still separate the OA and the RA in the case with the hydroxide paste. We now have $CH_3OH, NH_3$ … cells that all generally take hydrogen and make it into water. The first one was designed by NASA in the 1960s

### Proton Exchange Membranes (PEM) Cells
These cells use $H^+$ions to transfer electrons through an external circuit: you can use many fuels including hydrogen or alcohols. These are an alternative to alkali cells, but they still require separation of the anode and cathode with a membrane.

### Microbial Fuel Cells
Has the potential to turn waste water treatment facilities into energy producers if we can develop it on a larger scale. These do not produce a lot of energy, but can make a waste treatment facility have a net 0 on energy consumption. Organic matter is decomposed by bacteria to produce energy and small amounts of carbon dioxide to drive a fuel cell. The bacteria must be anaerobic because we separate the cathode oxygen so electrons flow towards it.

![[table.png]]