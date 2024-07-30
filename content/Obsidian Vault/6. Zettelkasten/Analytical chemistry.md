2024-07-1617:07
Status: #IBnotes 
## Introduction
Our perceptions of chemistry are limited to fragrances, color change, and whatever measurements we can perform. Analytical chemistry allows us to measure things that we cannot see in order to visualize a molecule, composition and structure.

The purpose of analytical chemistry is to find:
- Elemental composition
- How atoms are arranged/bonded (aliphatic, aromatic, or other functional groups.
# Spectroscopy
Spectroscopy is a branch of science concerned with the investigation and measurement of spectra produced when matter interacts with the electromagnetic spectrum.
A wave can be defined using the following:
$$ c=\nu \cdot\lambda=f\cdot\lambda $$
Where $c$ is the speed of light, $\approx 3.00 \times 10^8 m/s$, $\nu = f$=frequency ($Hz$), and $\lambda$ is the wavelength
A particle’s energy can be defined using the following:
$$ E = h\nu $$
Where $E$ = Energy of the particle, $h$ is Planck’s constant, and $\nu$ is the frequency.
Substituting the speed of light’s frequency equation into the energy equation a new formula for the energy of a particle.
$$ E=\frac {hc} \lambda $$

Recall that atoms exist in several energy levels, however, they prefer to stay in a quantized energy level. These come about is bonds in molecules, stretch bend rotate or as energy from one orbital to another.

As with energy states of atoms, the energy state of molecules can be quantized - they only exist at discrete amounts.
### Process
1. Expose the sample with EMR (Electromagnetic radiation)
2. The sample will absorb specific energies and reflect others.
3. The detector will pick up the reflected energy and also determine what was absorbed.
## Frequencies of light
- Microwave: Absorbed by nuclei, increases the rotational energy of polar molecules
- Infrared: Absorbed by the bonds, which causes them to stretch
- Visible/UV: Can reveal electron transitions (flame tests)
- X-rays: Can reveal interatomic distances.
## Percent composition:
Tells you by mass what percent of each element is present in a compound. The steps for calculating:
1. Find the molar mass of the elements
2. Find the mmolarmass of the compound
3. Divide the components by the total $\times 100\%$
### Example 1
What is the percent composition of phosphorous and chlorine in $PCl_5$?
$P=30.97\frac g{mol} \cdot 1 mol =\frac {30.97} {208.22} \cdot 100\%=14.9\%$
$Cl=35.45 \frac g {mol} \cdot5mol =\frac {177.25}{208.22}\cdot100 \% = 85.1 \%$
### Example 2
Propose a reasonable molecular formula given the following percent composition.
$C=\frac{66.63\%}{12.01g} =5.55$ $\ \ \ \ \ H=\frac {11.18\%}{1.01g}=11.1 \ \ \ \ \ \$ $?=22.19\%$
$5.55 : 11.1=1:2 \ \ \ \ \ \therefore C_nH_{2n}X_Y$

|C|H|X| |
|---|---|---|---|
|1|2|||
|12.01|2.02|4.00g|18.02g|
|66.63%|11.18%|22.19%|100%|

Increasing the number of carbons e.g.
$C_4 = 48.04g; H_8 =8.08g; O=16.00g$ fits the ratio: $C_4H_8O, C_8H_{16}O_2, C_8H_{16}S...$ and …
$C_7=84.07g; H_{14}=14.14; N_2=28.00g$ fits the ratio: $C_7H_{14}N_2$.
## Index of Hydrogen Deficiency (IHD)
The IHD is the count of how many molecules of $H_2$ can be added to the structure to make it saturated. The IHD number tells us how many double, triple bonds, or cyclic rings are present:

$IHD =0.5[2c+2-H-X+N]$

Where each carbon determines the maximum amount of hydrogen, $2C+2$.
Take away the hydrogens already present.
Oxygen forms two bonds and has no impact on hydrogen count.
Nitrogen forms three bonds, therefore added hydrogen.
Halogens, $X$ replaces hydrogen
0.5 is used to account for the $H_2$ nature of hydrogen.
## Mass Spectroscopy
Mass spectroscopy is a physical analytical technique, and does not use EMR. This results in a stereograph, an image that compares the abundance percentage to mass. Molecules are converted to ions and then sorted by their mass to charge ratio: (m/Z).

This is done by introducing a small amount of the compound into a vacuum chamber, where it is vaporized and the sample is bombarded with high energy electrons.

$$\begin{gather} M+e^-\to M^++2e^- \\CH_3OH_{(g)} e^-_{beam} \to CH_3OH^+_{(g)} + offshot \ e^- \end{gather}$$

The molecular ions are then accelerated by an electric field and they form a beam of powerful charged particles that move into a powerful magnetic field. The ions are deflected by the magnetic field based on their charge and their mass (heavier compounds deflect the lens).

![[Mass-Spectrometry-MS.webp]]

In the mass spectrometer produces a graph that plots the relative abundance of particles as a function of mass-to-charge ration (the scales vary).
### Example 2:
![[edfghjk.png]]
![[rfvbnkjhgb.png]]

When a molecule is bombarded with electrons, it forms the parent molecule (the highest mass and significant peak), often denoted $M^+$.

Continued bombardment creates fragments called daughter molecules (not all fragments are possible to theoretically show up on the spectrometer)
### Distinct isotope patterns worth noting:
Chlorine, $Cl = 35.45g$ $^{35}Cl:^{37}Cl = 3:1$ $M$ is 3 times as large as $M+2$.
Bromine, $Br = 79.90g$ $^{79}Br:^{81}Br = 1:1$ $M$ is as large as $M+2$.
## Infrared Spectroscopy (IR Spec)
*IR Spec is notoriously unreliable* 
IR is used to determine the types of bonds (works best for polar bonds) in a compound. Passing IR radiation ($f=\nu=500-400cm^{-1}$) through a sample. IR radiation causes excitation of covalent bonds for ‘stretching and bending’ of bonds.
Percent (%) transmittance is the amount of radiation that passes through the sample and is detected (a 100% transmittance would indicated that the molecule did not absorb any IR).
A wavenumber is the number of waves/centimeter = $wavenumber = \frac 1 {wavelength(cm)} = cm^{-1}$ .
Machines operate in the $5000-400cm^{-1}$ range. Each $\lambda$ is fired at the molecule one at time.

![[001.png]]
![[002.png]]![[003.png]]![[004.png]]
![[005.png]]
![[006.png]]![[007.png]]![[008.png]]

## Nuclear Magnetic Resonance Spectroscopy (NMR Spec)
[[Electrodynamics]] 
NMR spectroscopy is predominantly used for detecting $C-H$ bonds. It only works when there is an odd number of protons or an odd number of neutrons. ($^{13}_{\ 6}C \ (6p^+, 7n^0)$ works but $^{12} _{\ 6}C \ (6p^+, 6n^0)$ does not). Because carbon-12 does not have odd neutrons or protons, it does not have spin. For organic chemistry, $^1_1H$ is used as it has an odd number of protons, spin, and creates its own magnetic field.

NMR is the most useful technique for detecting organic structures. Nuclei are made of charged particles, and nuclei of isotopes with an odd mass number have a $\frac 1 2$ spin. Nuclei have magnetic fields that can be manipulated: in solution these nuclei are in random positions, but they can be manipulated in a magnetic field to be uniform and aligned with each other.

In a magnetic field, protons will all oppose each other ($\beta$ spin state) or face the same direction ($\alpha$ spin state). The $\alpha$ spin state has a lower energy state than that of the $\beta$ spin state. The majority of the protons will be in the $\alpha$ spin state as it is the lowest, most stable state.

![[1303.gif]]

![[images (1).png]]

*With the increase of magnitude to the applied magnetic field, $|B_0|$, the difference in energy between the $\alpha$ and $\beta$ states, $\Delta E$, increases proportionally.
$$\Delta E=hV=h[\frac {\gamma}{2\pi}B_0]$$

Where $h$ is Planck’s constant, $\gamma$ is the gyromagnetic ratio, and $B_0$ is the applied magnetic field. When there is a jump to the $\alpha$ state from the $\beta$ state, a radiofrequency, $rf$ is emitted.
### Tetramethylsilane (TMS), $(CH_3)_4Si$
This is added to the H-NMR and serves as a standard reference. All the hydrogen are the same and provide one signal that is easy to locate. TMS is inert and has a low boiling point (it can be separated from the sample).

![[edkhsdhesfwesadeas.png]]

### $^1H$ NMR (Table 27)
Each “type” of hydrogen bonding shows a different signal. This depends on the desheilding (downfield)/shielding (upfielding) nature of the bond. Shielding occurs when there are more electrons present around the nucleus of the $H$. Electrons withdrawing groups, (like an alkene or an$O$ atom) cause downfield shifts as the deshifted the $H$. This can be thought of as how “crowded the $H$ atom is.

![[009.png]]

![[010.png]]

![[NMR-chemical-shift-table-1024x774.png]]

### Interpreting $^1H \$ NMR
1. Peak area (integration trace) Peak area is proportional to the number of $H$ creating the peak (a higher peak means more $H$ atoms of that environment):![[wejhhkjwhr;.png]]
2. Spin-spin splitting Each ^1H is essentially a tiny magnet, therefore each H feels a magnetic field from its neighbors. If H has a nucleus, n, neighbors that have significantly different chemical shifts, the signal splits into n+1 peaks: A single peak = a singlet, two peaks = a doublet, triplet, quartet etc.![[sdfewdfe.png]]
*Sometimes the peaks are too tiny/overlap and splitting is not possible to determine.*
## X-Ray Crystallography
X-Ray crystallography is an analytical technique commonly used in structural biology and in organic chemistry to determine the 3D structure of small molecules (e.g. proteins).
1. Crystal formation
	- Mass produce protein, exact and purify.
	- Crystallize by dehydrating (creates an orderly structure).
2. X-Ray exposure
	- Smaller crystals require stronger X-Rays.
	- The crystal diffracts the X-Ray in a pattern that is specific to the crystal.
3. Analysis
	- “Magical math”
	- The pattern helps us solve for the 3D structure
	- Use a computer to model molecules using complex equations and algorithms

The advantages of doing so are that detailed 3D structures are produced, however it is limited in that larger proteins are really hard to crystallize and therefore can only produce very small crystals. Therefore, more powerful X-Rays are needed to model these proteins.

