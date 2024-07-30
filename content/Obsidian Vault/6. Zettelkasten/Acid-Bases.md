2024-07-1015:56
Status: #IBnotes 
Tags: [[Reaction equilibrium]]

## Review of Acid-Bases 

![[Pasted image 20240710155952.png]]
## Water equilibrium
At standard conditions, water is in the following equilibrium:
$$ 2H_2O_{(l)} \rightleftharpoons H_3O^+_{(aq)}+OH^-_{(aq)} \ \ \ \ K_c = K_w =1.0 \times 10^{-14} $$
$K_a$ = acid ionizations constant. ($HF_{(aq)} +H_2O_{(l)} \rightleftharpoons H_3O^+_{(aq)}+F^-_{(aq)}$)
$K_b$ = base ionization constant. ($F^-_{(Aq)} =H_2O_{(aq)} \rightleftharpoons OH^-_{(aq)} +HF_{(aq)}$)
They are conjugate acid-base pairs.
$\frac 1 {K_a} \ne K_b$ These are not reverse reactions. Rather:
$K_a \times K_b= (\frac {[H_3O^+][F^-]}{HF}) (\frac {[OH^-][HF]}{[F^-]})=[H_3O^+][OH^-]=K_w$
Because $K_w$ is temperature dependent, the $pH$ of the water can fluctuate. $K_w$ can be used to convert $[H_3O^+]$ and $[OH^-]$ directly.
### Example 1
What is the $[OH^-]$ in a solution with a $pH$ of $14.25$ ?

- Method 1
$$ \begin{gather} pOH=(14.25) = -0.25 \\ \ [OH^-]= 10^{-(-0.25)}= 1.8 \frac {mol} L \end{gather} 
$$

- Method 2:
$$ \begin{gather} [H_3O^+]=10^{-(pH)} = 10^{(-14.25)}= 5.623 \times 10^{-15} \\ \ [OH^-] = \frac {K_w}{[H_3O^+]}= \frac {1.0 \times 10^{-14}}{5.623 \times 10^{-15}}= 1.8 \frac {mol} L \end{gather} $$
## Strengths of Acids and Bases 
### Strength of Acids 
Strong acids ionize completely in water and are quantitative reactions. For example: $$HCl_{(aq)} +H_2O_{(l)} \to H_3O^+_{(aq)}+Cl^+_{(aq)}$$Weak acids ionize partially and are measured and quantified by $K_a$. An example of this is: $CH_3COOH_{(aq)} + H_2O_{(l)} \rightleftharpoons H_3O_{(aq)} ^++CH_3COO^-_{(aq)}$.
#### Example 2
What is the $pH$ of $0.10M\ CH_3COOH_{(aq)}$ ($K_a$ is $1.8\times 10^{-5}$) and

| |CH3COOH(aq)|H3O+(aq)|CH3COO-(aq)|
|---|---|---|---|
|I|0.10|0|0|
|C|-x|+x|+x|
|E|0.10-x|x|x|

$$ 1.8 \times 10 ^{-5} = \frac {x^2}{0.10-x} \approx\frac {x^2}{0.1} \\x= 0.00134... M \\pH=-\log(0.00134...)=2.87 $$

### Strengths of Bases
A strong base are metal hydroxides that dissociate completely. When they enter water, they produce $OH^-$ directly. Ignore $Mg(OH)_{2(aq)}$.
$$ NaOH_{(aq)} \rightarrow Na^+_{(aq)}+3OH_{(aq)} $$
A weak base is any compound that reacts with water to produce $OH^-$. (Must have water)
$$ NH_{3(aq)} +H_2O_{(l)} \rightleftharpoons OH^-_{(aq)}+NH_{4(aq)}^+ $$
#### Example 3
What is the $K_b$ for $HSO_{3(aq)}^-$? (If $K_b$ is being asked for, treat the substance as a base. Find the conjugate acid)
$$ K_w = K_aK_b \to K_b =\frac {K_w}{K_a}\\ K_b= \frac {1.0\times 10^{-13}}{1.4 \times 10^{-2}} = 7.1 \times 10^{-13} $$
#### Example 4
What is the $pH$ of a $0.10 \frac {mol} L$ sodium hydrogen sulfite solution? Provide a reason why it should be treated as an acid.
$$ NaHSO_{3(aq)} \to Na^+_{(aq)} + HSO_{3(aq)} ^- $$
This should be treated as an acid for the following reason:

$$HSO_{3(aq)} \ K_a = 6.3 \times 10^{-8} \\HSO_{3(Aq)} ^- \ K_b = \frac {1.0\times to^{-14}}{1.4 \times 10^{-2}}=7.1 \times 10^{-13}$$
| |HSO3(aq)-|H3O(aq)+|SO3(aq)-|
|---|---|---|---|
|I|0.10|0|0|
|C|-x|+x|+x|
|E|0.10-x|x|x|
$$ 6.3\times 10^{-8} = \frac {x^2}{0.10-x}\\ \to_{approx} 6.3\times to ^{-8} = \frac {x^2}{0.10} \\x=7.94 \times 10^{-5} \\pH= 4.10 $$
#### Example 5
What is the $pH$ of a $0.10 \frac {mol} L$ ammonia solution.

$$ NH_{(aq)} +H_2O_{(l)} \rightleftharpoons OH^-_{(aq)} + NH_{4(aq)}^+  
$$
$$ \begin{gather}K_b=\frac {K_w}{K_a}= \frac {1.0\times 10^{-14}}{5.6\times10^{-10}} = 1.7857...\times 10^{-5} \\ K_b = \frac {x^2}{0.10-x} \to_{approx} \frac {x^2} {0.10} \\x= 1.3379...\times 10^{-3} = [OH^-]\\-log(1.3379..\times 10^{-3} )= 2.874_{pOH} \\ 14-2.874 = pH = 11.13\end{gather}
$$
## Brønsted-Lowry (BL) Theory of Acids and Bases

### BL Acids
Acids are defined as compounds that donate protons, $H^+$. Those protons bond with $H_2O_{(l)}$ to form $H_3O_{(aq)}$ . (Note that acids can donate $H^+$ ions to other substances)
### Strong BL acid example

$$ H_2SO_{4(aq)_{strong \ acid}} + H_2O_{(l)_{base}} \to H_3O^+_{(aq)_{conjugate \ acid}} + HSO_{4(aq)_{conjugate \ base}} ^- $$

$H_2SO_{4(aq)}$ is the strongest acid and as $H_2O_{(l)}$ is the strongest base, the two react with each other. As $H_2SO_{4(aq)}$ donates a $H^+$ ion to the $H_2O_{(l)}$ molecule, $H_2SO_{4(aq)}$ acts as the acid and $H_2O_{(l)}$ acts as the base. The conjugate base for $H_2SO_{4(aq)}$ is $HSO_{4(aq)}^-$ and the conjugate acid for $H_2O_{(l)}$ is $H_3O_{(aq)} ^+$. Because this is a strong acid, it is a $>99.9\%$ forward reaction and is considered a quantitative reaction (Hence the ‘→’)
### Weak BL acid example

$$ H_3PO_{4(aq)_{weak \ acid}} + H_2O_{(aq)_{base}} \rightleftharpoons H_3O^+_{(aq)_{conjugate \ acid}} + H_2PO_{4(aq)_{conjugate \ base}} ^- $$

$H_3PO_{4(aq)}$ is the strongest acid (despite being considered a weak acid it is still a stronger acid than $H_2O_{(l)}$ ). Whereby $H_3PO_{4(aq)}$ acts as the acid as it donates a $H^+$ to the $H_2O_{(l)}$ molecule and $H_2O_{(l)}$ acts as the base as it accepts the $H^+$ ion. The conjugate base for $H_3PO_{4(aq)}$ is $H_2PO_{4(aq)}^-$ as the reverse reaction takes a $H^+$ ion from the $H_3O^+$ ion. Similarly, for $H_2O_{(l)}$ , it accepts a $H^+$ ion and acts as a base in the forward reaction. However, it’s conjugate acid, $H_3O^+ _{(aq)}$ donates a $H^+$ ion to $H_2PO_{4(aq)}$ in the reverse reaction. Because this is a weak acid, it is an equilibrium reaction, and $\rightleftharpoons$ are used to denote this behavior.
### BL Bases
Bases are defined as substances that can accept a form of $H^+$ from water and create $OH^-$. Whereby bases are proton acceptors. (It can also accept $H^+$ from a variety of different compounds, not solely from water.) $H_2O_{(l)}$ in these interactions can act as an acid, donating $H^+$ if there is a stronger base.
#### Strong bases
$$ Ba(OH)_{2(aq)} \to Ba^{2+} _{(aq)} + 2OH^-_{(aq)} $$
Note that $Ba(OH)_{2(aq)}$ does not react with water, as it is already an ionic compound that dissociates in water, unlike the acids which have to ionize. This relationship is depicted using a ‘→’ as dissociation is a process that does not likely result in a reverse reaction ($>99\%$.)
#### Weak bases
Weak bases are the conjugate bases of all the weak acids.

The conjugate bases of the strong acids do not meet the qualification of a base and should be considered neutral. ($ClO_4^-, I^-, Br^-, Cl^-, HSO_4^-, NO^-_3$)
### Ionic substances
Ionic substances often produce a conjugate base to a weak acid. For example:
#### Example 6
$$ NaCN_{(aq)} \to Na_{(aq)_{neutral}} ^++ CN^-_{(aq)_{weak \ base}} \\ CN^-_{(aq)} + H_2O_{(l)} \rightleftharpoons HCN_{(aq)} + OH^-_{(aq)} $$
### Amphiprotic ions and substances
Some ions can act as both an acid or a base. A common trend for such ions is having at least one free (as in not bonded to a polyatomic ion) $H^+$ and having an overall charge of $1-$ or less. This allows for $H^+$ ions to be accepted and donated. In addition, water can act as both an acid and a base. Some examples include: $HSO_{3(aq)} ^-, H_2PO_{4(aq)} ^-, HCO_{3(aq)} ^-, HPO_{4(aq)} ^ {2-}, HOOCCOO^-_{(aq)}$ However, based on their $K_a/K_b$ value, they will have a tendency to act more like an acid/base. ** An important note that $HSO_{4(aq)}^-$ acts as an acid exclusively.
#### Amphoteric but not amphiprotic substances
An amphoteric substance is any substance that can act as both an acid and a base. Amphiprotic - through the donation/acceptance of $H^+$. There are also non-amphiprotic but amphoteric substances. Primarily Oxides and hydroxides such as:
$$ Al_2O_{3(s)} + 6HCl_{(aq)} \to AlCl_{3(aq)} + 3H_2O_{(l)} \\ Al_2O_{3(s)} + 2NaOH_{(aq)} + 3H_2O_{(l)} \to 2Na[Al(OH_4] $$
### 5 Step BL method
1. List all entities present (ions, molecules, molecules). Dissociate ionic compounds and ionize strong acids if necessary.
2. Identify and label all compounds as acidic, basic or neutral.
3. Identify the strongest acid and strongest base.
    1. Acids that are ‘higher up’ on the table within the data book or have a higher $K_a$ value are the stronger acid.
    2. Bases that are ‘lower down’ on the table within the data book or have a lower $K_a$ value (subsequently having a higher $K_b$ value) are the stronger base.
4. Isolate the strongest acid and base and create a separate equation showing the transfer of a proton, $H^+$ directly between the two.
5. Predict the equilibrium position (reactant favored or product favored)
    1. If an acid is positioned higher relative to the base on the table within the data book, then the reaction is product favored.
    2. If the base is positioned higher relative to the acid then the reaction is product favored.

#### Example 7
Predict the BL equation and equilibrium position for the reaction between nitrous acid and sodium acetate.

|Step 1|HNO2(aq)|Na(aq)+|CH3COO(aq)-|H2O(l)|
|---|---|---|---|---|
|Step 2|Acid|Neutral|Base|Acid/Base|
|Step 3|Strongest acid|-|Strongest base|-|

Step 4: $HNO_{2(aq)} + CH_3COO^-_{(aq)}\rightleftharpoons NO^-_{2(aq)} + CH_3COOH_{(aq)}$
Step 5: Product favored.
### BL Exceptions
#### Carbonates
Carbonates and bicarbonates neutralize acids to produce water and carbon dioxide.
$$ \begin{gather} CaCO_{3(s)} +2HCl _{(aq)} \rightleftharpoons CaCl_{2(aq)} + H_2O_{(l)} +CO_{2(g)} \\ NaHCO_{3(s)} +H_2SO_{4(aq)} \rightleftharpoons NaHSO_{4(aq)} +H_2O_{(l)} +CO_{2(g)} \end{gather}$$
#### Acidic metals
$$ Mg_{(s)} + 2HCl _{(aq)} \rightleftharpoons MgCl_{2(aq)} + H_{2(g)} $$


#### Metal oxides (basic)
$$ CuO_{(aq)} \to Cu^{2+} + O^{2-} _{(aq)} \\O^{2-} _{(aq)} + H_2O_{(l)} \rightleftharpoons 2OH_{(aq)} ^- $$
#### Non-metal oxides (acidic) $CO_x, NO_x, SO_x$

$$ CO_{2(g)} + H_2O_{(l)} \rightleftharpoons H_2CO_{(aq)} \\ NO_{2(aq)} + H_2O_{(l)} \rightleftharpoons H_2NO_{3(aq)_{acid \ rain}} \\ SO_{2(aq)} + H_2O_{(l)} \rightleftharpoons H_2SO_{(4(aq)_{acid \ rain}} $$
## pH Curves

The variation in $pH$ that occurs during an acid-base reaction is what a $pH$ curve visualizes. Where the $pH$ is plotted against the a volume of titrant added to the sample. Examples of a strong base/strong acid titrations:

![[wuhr.png]]![[ererer.png]]![[43rwefefew.png]]
![[tyhyurty.png]]
### Polyprotic titration curves
A polyprotic compound is a compound that can donate more than one proton: $(H_2SO_4, H_2SO_3, H_2CO_3, H_3PO_4)$ . A polybasic compound is a compound that can accept more than one proton, and often is a conjugate base of a polyprotic acid:$(CO_3^{2-}, PO_4^{2-} , SO_3^{2-})$. Additionally, there are amphiprotic substances that can accept or donate $H^+$ions.

For these titrations, only one proton is transferred at a time.
#### Example 8

![[ergerg.png]]
#### Example 9

![[uyrtghty.png]]

## Indicators
A solution of weak acid where the acid and its conjugate base have different color.
Several indicators are abbreviated as they are massive, complex molecules. For example phenolphthalein has a chemical formula of $C_{20} H_{14}O_{4(aq)}$ but is referred to as $HPh_{(aq)}$The point where the color change occurs is when the concentration of the indicator, $[HIn]$ is the same as its conjugate base, $=[In^-]$ or when $K_a=[H_3O^+]$ $-log(K_a)=pKa=pH$.

$$ HIn_{(aq)} + H_2O_{(l)} \rightleftarrows H_3O^+_{(aq)} + In_{(aq)} ^- $$

$$ K_a= \frac {[H_3O^+][In^-] }{[HIn]} $$

### Example 6:
Predict the $pH$ where methyl orange will change color
$$ K_a = [H_3O] = 3.5 \times 10^{-4} \\-log(3.5\times 10^{-4}) =3.456 \\ 3.2 < 3.456 < 4.4 $$

The $pH$ at which an indicator changes color is called the transition point, and lies between within the range in the data-booklet. (This value is subjective)
### How does an indicator work?
Adding $H_3O^+_{(aq)}$ or $OH^-_{(aq)}$ , an equilibrium shit occurs. For example:
$$ HPh_{(aq)_{colourless}} +H_2O _{(l)} \rightleftharpoons H_3O_{(aq)} ^+ + Ph ^-_{(aq)_{pink}} $$
- If $H_3O^+$ is added the concentration of $H_3O^+$ increases, the equilibrium shifts left and becomes ‘more colorless’.
- If $OH^-$ is added, the concentration of $OH^-$ increases, the equilibrium shifts right and becomes ‘more pink;’. (neutralization)
### Choosing indicators
An indicator should change color near the endpoint of the reaction. When choosing an indicator do not choose the one that changes along one of the ‘buffer zones’ An indicator should change color near or at the end point of the reaction. The indicator must not change color in the buffer zone. (If there is only one color change, there is no buffer zone)

When indicating color change, make sure to state $x$ to $y$. (E.g. red to blue)

![[kjhjkhl.png]]

## Buffers
An acid-base buffer helps reduce the impact of adding a stress to a system (such as adding an acid or base). A buffer is made up of roughly equal concentrations of a weak acid and its conjugate base. This is not natural.

$$ H_3COOH_{(aq)} (0.50M)+ H_2O_{(l)} \rightleftharpoons CH_3COO^-_{(aq)} (0.50M) + H_3O^+_{(aq)} $$

To make the buffer above, there are two methods to do so:

1. Take the weak acid, and add its conjugate base in the form of ionic salt. E.g. $CH_3COOH_{(aq)} (0.50M) + NaCH_3COO^-_{(aq)} (0.50M)$
2. Take the weak acid, and convert half of it by adding a strong base. E.g. $CH_3COOH_{(aq)}(1.0M\to 0.50M) + OH^-_{(aq)} \to CH_3COO^-_{(aq)} +H_2O_{(l)}$

### Blood example
A great example is human blood: Which buffers against all the acids we like to eat. In addition to this, blood can act as an important breathing censor.
$$ CO_{2(gq)} +H_2O_{(l)} \rightleftharpoons H_2CO_{3(aq)} +H_2O_{(aq)} \rightleftharpoons H_3O_{(aq)}^++HCO_{3(aq)}^- $$

### Buffer Capacity 
Is the measure of the ability to resist $pH$ change. Higher concentrations of buffers resists more

$$ \beta = \frac n {\Delta pH} $$

Where $\beta$ is the buffer capacity, $n$ is the amount of moles . The amount of (moles) of a/b needed to change 1L of buffer pH by 1. 

## Equilibrium of Acid-Bases
Since $K_a$ and $K_b$ vary over such a great range that another log scale can be applied.
$$ \begin {gather} pKa = -\log(K_a) \ \ \ pK_b =-\log (K_b ) \\ K_a = 10^{-pK_a} \ \ \ K_b = 10^{-pK_b} \\ pK_a +pK_b = 14 =pK_w \end{gather} $$
This information can be found in table 21 in the IB data booklet.
### Hydrolysis
Hydrolysis is a reaction with water
$$ \begin{gather} SA \ \ \ HCl_{(aq)} +H_2O_{(l)} \to H_3O^+_{(aq)} +Cl^-_{(aq)} \\ WA \ \ \ \ \ \ HF_{(aq)} +H_2O_{(l)} \rightleftharpoons H_3O^+ _{(aq)} +F^-_{(aq)} \\ SB \ \ \ \ Ba (OH)_{2(aq)} \to_{H_2O} 2OH^-_{(aq)} + Ba^{2+}_{(aq)} \\... \end{gather}$$

For amphiprotic species, a comparison of their $K_a$ and $K_b$ is done. The larger value,
### Brønsted-Lowry (BL) Model
Acids are compounds that donate a $H^+$ion to water and create $H_3O^+$, can also donate to other species.
A BL acid is a proton, $(H^+)$ donor.
Bases are compounds that can accept a $H^+$ ion from water and create $OH^-$, can also receive from other species.
A BL base is a proton, $(H^+)$ donor.
$$\begin{gather} SA \ \ \ \ H_2SO_{4(aq)_{acid} }+H_2O_{(l)_{base}} \to H_3O^+ _{(aq)} + HSO_{4(aq)}^- \\ WA \ \ \ H_3PO_{4(aq)_{acid}} + H_2O_{(l)_{base}} \rightleftharpoons H_3O^+_{(aq)_{base}}+H_2PO_{4(aq)_{base}} \end{gather}$$

Water acts as a base within the $SA$, strong acid and example

## Lewis Acid-Bases 
### Lewis acids
A Lewis acid is an electron pair acceptor. Which is a material that must be electron deficient. Wherein they must have empty orbitals and must be ‘positively’ charged.

Lewis acids extend the definition of an acid as an electron pair acceptor does not necessarily have to give away a $H^+$ to accept the electron pair.

A Lewis acid often creates a scenario where the $H^+$ from a nearby water molecule is donated instead. Lewis acids ‘encourage’ other materials to be acidic.
### Lewis base
A Lewis base is a material that donates an electron-pair (lone pairs or electrons in $\pi$ bonds) In addition, an electron pair donor, a LB can always donate electrons to $H^+$, which is the same as accepting/attracting $H^+$, a BL base.

The Lewis definition does not add any new bases,
## Transition metals as complex ions
When a transition metal is dissolved, it will have a positive charge. This positive charge will attract the negative dipole of ligands such as water molecules. Because such transition metals have a high amount of compounds that have a hydrogen ion surrounding the ion, the bonded hydrogen is more likely to be donated to another substances. This forms a complex metal ion (mad of ion (metal) and ligands (usually water) that have a coordinate covalent bond. Common examples include $Cu^{2+}$ and $Al^{3+}$.

![[yrthrfgx.png]]

$$ \begin{gather} Cu^{2+}_{(aq)} +6H_2O \rightleftharpoons [Cu(H_2O)_6]^{2+} _{(aq)} + H_2O \rightleftharpoons [Cu(H_2O)_5OH]^{+}+ H_3O^+_{(aq)} \\ Cu^{+2}+7H_2O_{(l)} \rightleftharpoons [Cu(H_2O)_5OH]^+_{(aq)} +H_3O^+_{(aq)} \end{gather}$$

The bonds that form between ion and ligands have a special name: coordinate covalent bond/dative bond. Wherein a covalent bond where only one partner provides both electrons.

### Non-metal oxides ($SO_x, NO_x, CO_x$) and acid anhydrides:
$$ SO_{3(aq)_{lewis \ acid}} + H_2O_{(l)} \rightleftharpoons H_2SO_{4(aq)_{BL \ acid}} +H_2O \to H_3O^+_{(aq)} + HSO_{4(aq)} ^- $$
![[yujhg.png]]
## Henderson Hasselbalck
$pH$ of a buffer: $pH = pKa +log(\frac {[base]}{[acid]})$.
### Example n.1:
What is the $pH$ of the $CH_3COOH (0.50M)/CH_3COO^-(0.50M)$ buffer system?

$$\begin{gather} pH =pKa + log (\frac {[base]}{[acid]}) \\ pH = -log(1.8 \times 10 ^-5 )+ log(\frac {0.50}{0.50}) \\pH = 4.74 \end{gather}$$
### Example n.2
What happens when $0.020 M \ HCl_{(aq)}$ is added to this buffer system?
$$ \begin{gather} CH_3COOH = 0.50M \to 0.52M \\CH_3COO^-= 0.50 M \to 0.48M \\pH = -\log (1.8 \times 10^{-5} ) + \log (\frac {0.48}{0.52}) \\pH = 4.71 \end{gather}$$
