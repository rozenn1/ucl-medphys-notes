---
id: glpkczctcjmipdl92duipn4
title: PHAS0021
desc: ''
updated: 1679908497107
created: 1679906243362
---

# PHAS0021 Electricity and Magnetism notes Term 1 Year 2     
_last updated on 15/12/2022_

Term 1, Year 2  
Department of Physics and Astronomy  
University College London


* * *

### CONTENTS:

*   Section 1: Electric Field
*   Section 2: Electric Flux and Gauss' Law
*   Section 3: Electric Potential V
*   Section 4: Capacitance and Charge Density
*   Section 5: Magnetostatics
*   Section 6: Magnetism in Matter
*   Section 7: Electromagnetic Induction
*   Section 8: Alternating Current

* * *


## Section 1: Electric Field

Force $F$ is equal to the gradient of potential energy, so it is related to the **energy gradient**. 
$$
F=-\Delta U
$$
Conservation of charge: net charge $Q_{net}$ is always conserved.

**Coulomb's Law** gives the Electric force $\textbf{F}$ of $q_{1}$ on $q_{2}$. 
$$
\textbf{F}_{12} = \dfrac{1}{4\pi\epsilon_{0}} \dfrac{q_{1} q_{2}}{r_{12}^2} \hat{r}_{12}
$$
When calculating Coulomb force from multiple charges, add the individual forces by vector addition.

Permittivity $\epsilon=\epsilon_{0}\epsilon_{r}=\epsilon_{0}(1-\chi)$, where $\chi$ is susceptibility of the material, is inversely proportional to electric force.

**Electric field** (in $NC^{-1}$) is the Electric force a positive unit point charge would feel at a point. 
$$
\textbf{E}=\dfrac{1}{4\pi\epsilon_{0}}\dfrac{q_{1}}{r^2}\hat{r}\quad\Rightarrow\quad\textbf{F}_{12}=q_{2}\textbf{E}
$$

1.  Field lines point in the direction a positive test charge would go
2.  In systems with zero net charge, all field lines start on a positive charge and end on a negative charge
3.  The number of field lines passing through a surface is proportional to the magnitude of the field at that point

When calculating Electric field from multiple point charges, use vector addition: 
$$
\textbf{E}_{resultant}=\dfrac{1}{4\pi\epsilon_{0}}\sum_{i=1}^{n}{\dfrac{q_{i}}{r_{i}^{2}}}\hat{r}_{i}
$$
and for continuous charge distributions: 
$$
\textbf{E}(\textbf{R})=\dfrac{1}{4\pi\epsilon_{0}}\int_V{\dfrac{\textbf{R}-\textbf{r}}{|\textbf{R}-\textbf{r}|^3} \rho(\textbf{r})\space dV
$$
where $\textbf{R}$ is the distance from the origin to the point where electric field is being measured, and $\textbf{r}$ is the distance from the origin to each charge "block" $dV$.


* * *

## Section 2: Electric Flux and Gauss' Law

While electric field $\textbf{E}$ is proportional to the field lines per area, the Electric Flux $\Phi$ is proportional to the total number of field lines passing through a chosen surface. 
$$
\Phi=\dfrac{1}{\epsilon_{0}}\sum{q_{enclosed}}
$$
$\Phi=\textbf{E}a$ , where $a$ is area, for a flat surface perpendicular to $\textbf{E}$.

If $\textbf{E}\cdot\hat{n}$ varies, then use 
$$
\Phi=\int_{S}{\textbf{E}\cdot d\textbf{a}}
$$
where $d \textbf{a}=\hat{n} da $ .

**Gauss' Law** states that the net flux through a closed surface is proportional to the charge enclosed. 
$$
\Phi_{net}=\int_{S}{\textbf{E}\cdot\textrm{d}\textbf{a}}=\dfrac{Q_{internal}}{\epsilon_{0}}
$$
Use a Gaussian surface symmetrical about the point charge for simplicity.

**Solid Angle** $\Omega=\dfrac{area\space projected}{r^{2}}$. Total solid angle in sphere $=4\pi \space Sr$

Gauss' Law for a **Solid Sphere**: 
$$
E=\left\{\begin{array}{l} \dfrac{\rho r}{3\epsilon_{0}} & \textrm{for } r\lt a \\ \dfrac{1}{4\pi\epsilon_{0}}\dfrac{Q}{r^{2}} & \textrm{for } r\geq a \\ \end{array} \right.
$$
Note that for $r\geq a$, the charged ball acts like a point charge $Q$ .

For **Hollow Sphere** of negligible thickness: 
$$
E=\left\{\begin{array}{l} 0 & \textrm{for } r\lt a\\ \dfrac{1}{4\pi\epsilon_{0}}\dfrac{Q}{r^{2}} & \textrm{for } r\geq a\\ \end{array} \right.
$$
For $r\geq a$, the sphere acts like a point charge, but for $r\lt a$, the electric flux and field is zero due to 0 enclosed charge.

For uniformly **Charged Line**: 
$$
E=\dfrac{\lambda}{2\pi\epsilon_{0}r}
$$
Note that field falls off with $\dfrac{1}{r}$ .

For uniform infinite **Charged Plane**: 
$$
E=\dfrac{\sigma}{2\epsilon_{0}}
$$
So field is constant for any $r$.

**Gauss' law in differential form** is used when the electric field varies. 
$$
\textbf{$\nabla$}\cdot\textbf{E}=\dfrac{\rho}{\epsilon_{0}}
$$

  

* * *

## Section 3: Electric Potential V

**Electric potential energy** $U$ gives the joules of potential energy a charge $q_{2}$ has due to $q_{1}$. 
$$
U=\dfrac{1}{4\pi\epsilon_{0}}\dfrac{q_{1}q_{2}}{r}
$$
For multiple point charges, $U$ is equivalent to the energy needed to bring each charge near to one point: 
$$
U=\dfrac{1}{4\pi\epsilon_{0}}\sum_{\text{all pairs}}{\dfrac{q_{i}q_{j}}{r_{ij}}} =\dfrac{1}{4\pi\epsilon_{0}}\dfrac{1}{2}\sum_{i,j=1,j\neq i}{\dfrac{q_{i}q_{j}}{r_{ij}}}
$$
For a continuous charge distribution, calculate the integral of bringing in each infinitesimal shell. E.g., for a ball of radius $a$: 
$$
U_{sphere}=\dfrac{3}{5}\dfrac{Q^{2}}{4\pi\epsilon_{0}a}
$$


**Electric potential** $V$ (in $JC^{-1}$ or volts $V$) gives the potential energy a test charge would have at that point per coulomb, due to $q_{1}$. 
$$
V=\dfrac{1}{4\pi\epsilon_{0}}\dfrac{q_{1}}{r}\quad \Longrightarrow \quad U=q_{2}V
$$
Electric potential from a set of point charges $q_{j}$ : 
$$
V(x_{i},y_{i},z_{i})=\dfrac{1}{4\pi\epsilon_{0}}\sum_{j}{\dfrac{q_{j}}{r_{ij}}}
$$
Potential from a continuous charge distribution: 
$$
V(x_{i},y_{i},z_{i})=\dfrac{1}{4\pi\epsilon_{0}}\int_{V}{\dfrac{\rho(x_{j},y_{j},z_{j})}{r_{ij}}}dV
$$

**Work** $W$ (in $J$) is path-independent: 
$$
W=-q_{2}\int_{a}^{b}{\textbf{E}\cdot d\textbf{s}}=-\dfrac{q_{1}q_{2}}{4\pi\epsilon_{0}}\left(\dfrac{1}{r_{A}}-\dfrac{1}{r_{B}} \right)
$$

$$
\dfrac{W}{q_{2}}=V(b)-V(a)\quad\Longrightarrow\quad V(b)=-\int_{\infty}^{b}{\textbf{E}\cdot d\textbf{s}}
$$
where $V(b)$ is the "absolute" potential at point $b$, i.e., the work required to bring a unit test charge from infinity to $b$.

#### Electric field as the gradient of Potential
$$
\textbf{F}=-\textbf{$\nabla$}W \implies \begin{array}{l} \textbf{F}=q\textbf{E}\\ W=qV\\ \end{array} \implies \textbf{E}=-\textbf{$\nabla$}V
$$

$$
\textbf{E}=\left\{\begin{array}{l} -\left(\dfrac{\delta V}{\delta x}\hat{x}+\dfrac{\delta V}{\delta y}\hat{y}+\dfrac{\delta V}{\delta z}\hat{z}\right) \quad cartesian\\ -\left(\dfrac{\delta V}{\delta\rho}\hat{u}_{\rho}+\dfrac{1}{\rho}\dfrac{\delta V}{\delta \phi}\hat{u}_{\phi}+ \dfrac{\delta V}{\delta z}\hat{u}_z\right)\quad cylindrical\\ -\left(\dfrac{\delta V}{\delta r}\hat{r}+\dfrac{1}{r}\dfrac{\delta V}{\delta\theta}\hat{\theta}+ \dfrac{1}{r\sin{\theta}}\dfrac{\delta V}{\delta\phi}\hat{\phi}\right)\quad spherical\\ \end{array}\right.
$$

An **Electric dipole** consists of two equal and opposite charges $+q$ and $-q$, with separation $2d$. 
$$
\textbf{E}\propto\textbf{p}\quad\text{where Electric dipole moment }\textbf{ p}=2q\textbf{ d}
$$

$$
V(P)=\dfrac{q}{4\pi\epsilon_{0}}\left(\dfrac{1}{\sqrt{r^{2}+d^{2}-2rd\cos{\theta}}}-\dfrac{1}{\sqrt{r^{2}+d^{2}+ 2rd\cos{\theta}}}\right)
$$

$$
V_{dipole}=\dfrac{q}{4\pi\epsilon_{0}}\dfrac{2d\cos{\theta}}{r^2}\quad\text{for $r\gg d$}
$$
**Method of images**: for an electric field outside conductors, replace complex parts with imaginary point charges, making sure the result has the same boundary conditions.

  

* * *

  

## Section 4: Capacitance and Charge Density

A **Capacitor** consists of two conducting plates with equal and opposite charge $q_{1}$. Consider what happens when the plates of a charged capacitor are pushed apart:

1.  With battery removed: $V$ increases, charge stays the same, electric field $E$ stays the same.
2.  With battery left in circuit: energy per charge increases, so some chrages leave plates to get $\Delta V$ back to $V$ of the battery. Charge per area $\sigma$ increases, $E$ decreases.
$$
E=\dfrac{\sigma}{\epsilon_{0}}\quad\text{where}\quad\sigma=\dfrac{q_{1}}{A} \begin{array}{l} \quad\leftarrow\text{charge on one plate}\\ \quad\leftarrow\text{Area of one plate}\\ \end{array}
$$
$$
C=\dfrac{\epsilon_{0}A}{d}=\dfrac{q_{1}}{\Delta V}
$$
Energy of a capacitor: $\quad U_{cap}=\dfrac{1}{2}Q\Delta V_{initial}$$\;=\dfrac{1}{2}C\left(\Delta V_{initial}\right)^{2}$

Energy density (per volume): $\quad u=\dfrac{U}{Ad}=\dfrac{1}{2}\epsilon_{0}E^{2}$

The **Polarisation** vector $\textbf{P}$ points in the direction that electrons in a material shift to (opposite to direction of induced electric field) 
$$
\textbf{P}=\dfrac{\Delta\textbf{p}}{\Delta v} \begin{array}{l} \quad\leftarrow\text{electric dipole moment}\\ \quad\leftarrow\text{volume}\\ \end{array}
$$
$\textbf{P}=\epsilon_{0}\chi\textbf{E}_{total}$ for isotropic materials with no initial dipole. 
$$
\textbf{P}_{total}=\textbf{P}_{permanent}+\textbf{P}_{induced}\quad\text{and}\quad\textbf{E}_{total}=\textbf{E}_{0}+ \textbf{E}_{induced}
$$

#### Adding Capacitance
$$
\text{In series:}\quad\dfrac{1}{C_{total}}=\dfrac{1}{C_{1}}+\dfrac{1}{C_{2}}\qquad\text{In parallel:}\quad C_{tot}=C_{1}+C_{2}
$$

#### Dielectrics in Capacitors
*   _CASE 1_ - the dielectric is an **insulator** : The external field from the capacitor causes the insulator material to **become polarised**.
*   _CASE 2_ - the dielectric has already **polarised** molecules (eg: water) : The polarised molecules **rotate to align with the capacitor field**.

In both cases, the total electric field $\textbf{E}_{total}$ is **reduced**. Capacitance $C$ **increases**. 
$$
C_{dielectric}=\epsilon_{r}C\qquad u_{with\space dielectric}=\dfrac{1}{2}\epsilon_{r}\epsilon_{0}\textbf{E}^2
$$
More susceptible dielectric $\iff$ More increase in Capacitance

#### Spherical capacitor
![Spherical capacitor: Sphere of radius a and charge +Q enclosed within another sphere of radius b and chrge -Q. Diagram.](https://th.bing.com/th/id/R.e57fdda8cc54d580384f0506edb536da?rik=nnu04xzPeOv04Q&riu=http%3a%2f%2fwww.actucation.com%2fimg%2fuploads%2fimages%2f19G2L2th21.png&ehk=V3yjghzxuFvljVGu3M3BGjPntuLS%2fKwSxmifrf1kRs8%3d&risl=&pid=ImgRaw&r=0 "A Spherical Capacitor"){max-width: 350px, display: block, margin: 0 auto}

Gaussian surface
*   When $r\lt a\longrightarrow\textbf{E}=0$ (no net $Q$)
*   When $r\gt b\longrightarrow\textbf{E}=0$ (no net $Q$)
*   But if $a\leq r\leq b$, then field is the same as for one point charge

$$
\Delta V=V(a)-V(b)=\dfrac{Q}{4\pi\epsilon_{0}}\left(\dfrac{1}{a}-\dfrac{1}{b}\right)
$$
$$
\implies C=\dfrac{Q}{\Delta V}=4\pi\epsilon_{0}\cdot\dfrac{ab}{b-a}
$$
Imagine $b\rightarrow\infty$. Then $C_{single\space sphere}=4\pi\epsilon_{0}a$.

#### Cylindrical capacitor

![Cylindrical Capacitor: cylinder of radius a and length L open on both ends within another cylinder of radius b and length L. Diagram.](https://encrypted-tbn2.gstatic.com/images?q=tbn:ANd9GcQ4MuIZwPjm4Yj3VRol2eGBm8wvm4p5KYDRTTvy7cGHTDVP0lMu "A Cylindrical Capacitor"){max-width: 350px, display: block, margin: 0 auto}

Consider a gaussian surface with $a\leq r\leq b$. If $L\gg b$, then field is the same as infinite charged line. 
$$
\Delta V=\dfrac{Q}{2\pi\epsilon_{0}l}\cdot ln\left(\dfrac{b}{a}\right)
$$
$$
C=\dfrac{Q}{\Delta V}=\dfrac{2\pi\epsilon_{0}l}{ln(b/a)}
$$

#### Electric dipole in a field
For an electric dipole with separation $\textbf{d}$, dipole moment is 
$$
\textbf{p}=q\textbf{ d}
$$
Remember electric dipole points from negative charge to positive charge. Torque Vector and potential energy of a dipole in a field: 
$$
\tau=\textbf{p}\times\textbf{E}\quad\text{and}\quad U=-\textbf{p}\cdot\textbf{E}
$$

#### Electric displacement $\textbf{D}$
$$
\textbf{D}=\epsilon_{0}\textbf{E}+\textbf{P}
$$
Where $\textbf{E}$ is the total net electric field due to external AND induced field, and $\textbf{P}$ is polarisation - dipoles per unit volume. 
$$
\textbf{D}=(1-\chi)\epsilon_{0}\textbf{E}=\epsilon_{0}\epsilon_{r}\textbf{E}\quad\implies\quad\textbf{D}=\epsilon\textbf{E}
$$
For isotropic materials with zero initial dipole.

If total charge density $\rho$ is split into free charges and bound in molecule dipoles $\rho=\rho_{free}+\rho_{bound}$ : 
$$
\nabla\cdot\textbf{D}=\epsilon_{0}\nabla\cdot\textbf{E}+\nabla\cdot\textbf{P}=\rho-\rho_{bound}=\rho_{free}
$$
So electric displacement only depends on free charges. Within material, Gauss' law is 
$$
\int_{S}{\textbf{D}\cdot d\textbf{a}=Q_{internal}}
$$

**Conductance** $G=\dfrac{1}{R}$

**Charge density** $\textbf{J}$ is a vector defined such that the charge passing through an area $d\textbf{a}$ per unit time is given by $\textbf{J}\cdot d\textbf{a}$. Hence, 
$$
I=\int_{A}{\textbf{J}\cdot d\textbf{a}}
$$
Also, 
$$
\textbf{J}=nq\textbf{ v}_{d}
$$
where $q$ is the magnitude of each charge carrier, $n$ is the number of charge carriers per unit volume, and $\textbf{v}_{d}$ is the drift velocity.

#### Resistivity and Conductivity
Ohmic materials have constant R when current of potential difference is changed. Each material has a resistivity $\rho$: 
$$
R=\rho\dfrac{L}{A}\qquad\rho=\dfrac{1}{\sigma}\qquad\begin{array}{l}V=IR\\\textbf{J}=\sigma\textbf{E}\\\end{array}
$$

#### Electrical Power
$$
P=\dfrac{dU}{dt}=\dfrac{dQ\Delta V}{dt}=I\Delta V\qquad P=IV=I^{2}V=\dfrac{V^{2}}{R}
$$
Power is measured in watts $W=Js^{-1}=VA$ .

#### EMF
$$
\epsilon=\dfrac{dW}{dq}
$$
EMF is the work done per unit charge to move charges against electric field in a battery.
*   Kirchoff's loop rule $\quad\sum_{closed\space loop}{\Delta V}=0$
*   Kirchoff's junction rule $\quad\sum{I_{in}}=\sum{I_{out}}$

#### Capacitor current change with time
![Circuit diagrams for discharging a capacitor. Diagram (a) shows the capacitor connected to the battery and the resistor such that it is charging. Diagram (b) shows the circuit altered such that the capacitor is only connected to the resistor, so it can discharge.](https://www.webassign.net/question_assets/ncsulcpem2/lab_4/images/figure4-1.png "Capacitor Discharge circuit. (a) Capacitor is chrging as it is connected to battery. (b) Capacitor is discharging into circuit as it is no longer connected to battery"){max-width: 350px, display: block, margin: 0 auto}

$$
I(t)=\dfrac{dq}{dt}=\dfrac{\epsilon}{R}e^{-t/RC}\qquad\text{where $RC=$ time constant}
$$
$$
I(t=RC)=0.368\space I(t=0)
$$

* * *

## Section 5: Magnetostatics
The force acting on a moving point charge in a magnetic field $\textbf{B}$ (measured in Teslas; $1\;T=1\;NA^{-1}m^{-1}$) is given by 
$$
\textbf{F}_{B}=q\textbf{v}\times\textbf{B}
$$
where the right-hand rule can be used to find the direction. Equating this to centripetal force, the radius of trajectory of a charged particle in a uniform magnetic field is 
$$
r=\dfrac{mv}{qB}\quad\textrm{with}\quad\omega=\dfrac{qB}{m}
$$
If the initial velocity of the charged particle has separate perpendicular and parallel components, consider these separately to find a coil shaped trajectory.

The **Lorentz Force** is given by 
$$
\textbf{F}=q\left(\textbf{E}+\textbf{v}\times\textbf{B}\right)
$$
which can be applied to velocity selectors and mass spectrometers using crossed fields.

#### The Hall effect
![Rectangular block with current I flowing though, perpendicularly to magnetic field B across it. Height of the block is d, thickness along magnetic field direction is t.](https://i.postimg.cc/bJ2VR4TN/halleffect.png "The Hall effect"){max-width: 350px, display: block, margin: 0 auto}

External field $B$ causes charge to accumulate on one side of the conductor. This induces an electric field $E_{H}$. 
$$
E_{H}=\dfrac{\Delta V_{H}}{d}
$$
with $qv_{d}B=qE_{H}$ at equilibrium. Since $I=nqv_{d}A$, 
$$
\Delta V_{H}=\dfrac{IB}{R_{H}t}\quad R_{H}=\dfrac{1}{nq}
$$

#### Magnetic force on a wire
It is given by 
$$
\textbf{F}_{B}=I\,\textbf{L}\times\textbf{B}
$$
for $\textbf{L}$ in direction of drift velocity. For a whole wire, it is given by 
$$
\textbf{F}_{B}=I\int_{a}^{b}\textrm{d}\textbf{s}\times\textbf{B}
$$
which means that $\textbf{F}_{B}=0$ for a closed loop.

#### Torque on a rectangular current loop; magnetic dipole
$$
\boldsymbol{\tau}=I\,\textbf{A}\times\textbf{B}
$$
Where $\textbf{A}=A\boldsymbol{\hat{n}}$ is the area of the current loop. Potential energy of loop is 
$$
U=-IAB\cos\theta
$$

![Wire forking into two, then recombining to form rectangular current loop. The rectangle has width b and length a.](https://i.postimg.cc/2ybB8NWy/Screenshot-20221201-042224.png "Rectangular current loop in a magnetic field"){max-width: 300px, display: block, margin: 0 auto}

![The area of the plane in the current loop has normal vector n hat, at an angle theta to the direction of the magnetic field.](https://i.postimg.cc/BZ7W1L8R/Screenshot-20221201-042754.png "Rectangular current loop: side view"){max-width: 300px, display: block, margin: 0 auto}

Define magnetic dipole moment as 
$$
\textbf{m}=I\,\textbf{A}
$$
This is analogous to electric dipole moment.

. | Electrostatics | Magnetostatics
--------|----------|----------
Torque | $\boldsymbol{\tau}=\textbf{p}\times\textbf{E}$ | $\boldsymbol{\tau}=\textbf{m}\times\textbf{B}$
Potential Energy | $U=-\textbf{p}\boldsymbol{\cdot}\textbf{E}$ | $U=-\textbf{m}\boldsymbol{\cdot}\textbf{B}$


#### Biot-Savart Law
$$
\textbf{B}=\dfrac{mu_{0}I}{4\pi}\int\dfrac{\textrm{d}\textbf{s}\times\boldsymbol{\hat{r}}}{r^{2}}
$$
Permeability of free space: $\mu_{0}=4\pi\times 10^{-7}Hm^{-1}\qquad1\;Hm^{-1}=1\;TmA^{-1}$$

#### Magnetic field due to long straight wire
$$
B_{\textrm{long wire}}=\dfrac{mu_{0}I}{2\pi r}
$$
With direction given by the right hand rule.

#### Magnetic field due to circular current loop
$$
B_{x}=\dfrac{\mu_{0}IR^{2}}{2\left(x^{2}+R^{2}\right)^{3/2}}
$$
Where $R$ is radius of loop, and $x$ is perpendicular distance from centre.

Consider these two extreme cases:

1.  $x=0$ (loop centre) 
$$
B_{0}=\dfrac{\mu_{0}I}{2R}
$$
2.  $x\ll R$ (far away from loop) 
$$
\textbf{B}=\dfrac{\mu_{0}}{4\pi}\dfrac{2\textbf{m}}{x^{3}}
$$

#### Magnetic force between two parallel wires
$$
B_{1}=\dfrac{\mu_{0}I_{1}}{2\pi d}
$$

$$
F_{2}=\dfrac{\mu_{0}I_{1}I_{2}l}{2\pi d}
$$
Wires attract if curret parallel in same direction.


#### Ampère's law
$$
\oint\textbf{B}\cdot\textrm{d}\textbf{s}=\mu_{0}I_{\textrm{through}\,\textrm{surface}}
$$

#### Magnetic field due to a solenoid
$$
B=\mu_{0}nI
$$
Where $n$ is number of turns per unit length.

#### Magnetic field due to a toroid
$$
B=\dfrac{\mu_{0}NI}{2\pi r}
$$
within toroid, and zero field outside.

#### Magnetic field due to an infinite conducting sheet
$$
B=\dfrac{\mu_{0}J}{2}
$$
Where J is current per unit length. This is analogous to $E=\sigma/2\epsilon_{0}$.

* * *

## Section 6: Magnetism in Matter
### Magnetic Susceptibility $\boldsymbol{\chi_{m}}$
External magnetic field $\boldsymbol{B_{0}}$ can induce a magnetic field within a material. 
$$
\boldsymbol{B_{m}}=\chi_{m}\boldsymbol{B_{0}}\quad
$$
$$
\textbf{B}=\boldsymbol{B_{0}}+\boldsymbol{B_{m}}=(1+\chi_{m})\boldsymbol{B_{0}}=\mu_{r}\boldsymbol{B_{0}}
$$
where $\mu_{r}$ is relative permeability. There are three types of magnetism in matter:

Suceptibility | Type of Magnetism
-------|-------
$-1\leq\chi_{m}\lt 0$ | **Dia**magnetism
$0\lt\chi_{m}\ll 1$ | **Para**magnetism
$\chi_{m}\gg 1$ | **Ferro**magnetism


### Diamagnetism
Magnetic field induced in material which opposes external magnetic field. All materials show diamagnetism, although effect is usually very small.

### Paramagnetism
Permanent magnetic moments of atoms align with external magnetic field. 
$$
\textbf{M}=\dfrac{\textbf{m}}{V}
$$
$$
\Rightarrow\quad\boldsymbol{M_{\text{max}}}=\dfrac{N\boldsymbol{\mu}}{V}
$$
Where $\textbf{M}$ is the magnetisation vector.

Pierre Curie's law: $\quad\textbf{M}=C\dfrac{\boldsymbol{B_{0}}}{T}$, where C is Curie's constant. Only holds for small B/T.

### Ferromagnetism
Permanent magnetic moments due to aligned spins of unpaired electrons. In hard ferromagnetism, this forms a permanent magnet, in soft ferromagnetism, the material is easily demagnetised.

At Curie temperature, all alignment breaks down - no magnetic (Weiss) domains.

### Magnetic field strength H
$$
\textbf{H}=\dfrac{1}{\mu_{0}}\textbf{B}-\textbf{M}=\dfrac{1}{\mu_{0}\mu_{r}}\textbf{B}
$$
$$
\textbf{M}=\dfrac{\boldsymbol{B_{m}}}{\mu_{0}}=\dfrac{\chi_{m}\textbf{B}}{\mu_{0}}
$$
which is analogous to electric displacement.

* * *

## Section 7: Electromagnetic Induction
### Magnetic flux
Magnetic flux is defined as magnetic field perpendiculerly through a surface. 
$$
\Phi_{B}=\int_{S}\textbf{B}\cdot\textrm{d}\textbf{a}
$$
Has units of weber $= 1\,Tm^{2}$.

### Gauss' law for Magnetostatics
Using the Biot-Savart law, 
$$
\boldsymbol{\nabla}\cdot\textbf{B}=0
$$
So magnetic flux is zero over any closed surface, which is why magnetic monopoles cannot exist.

### Ampère-Maxwell law for time-varying fields
Ampère's law is incomplete - Maxwell postulated a 'displacement current' defined as $I_{d}=\epsilon_{0}\dfrac{\textrm{d}\Phi_{E}}{\textrm{d}t}$, to revise Ampère's law as 
$$
\oint\textbf{B}\cdot\textrm{d}\textbf{s}=\mu_{0}I+\mu_{0}\epsilon_{0}\dfrac{\textrm{d}\Phi_{E}}{\textrm{d}t}
$$
So magnetic fields can be produced both by conduction currents **and** time-varying electric fields. In differential form, the Ampère-Maxwell law is 
$$
\boldsymbol{\nabla}\times\textbf{B}=\mu_{0}\textbf{J}+\mu_{0}\epsilon_{0}\dfrac{\textrm{d}\textbf{E}}{\textrm{d}t}
$$

### Faraday's law of Electromagnetic induction
A changing magnetic flux through a circuit induces a transient current with induced EMF: 
$$
\varepsilon=-\dfrac{\textrm{d}\Phi_{B}}{\textrm{d}t}
$$
Lenz's law states that the induced current has a direction which **opposes** the change in magnetic flux that induced it. Note that the electric field from magnetic induction is **not** conservative and can have non-zero curl.

Faraday's law in differential form is 
$$
\boldsymbol{\nabla}\times\textbf{E}=-\dfrac{\partial\textbf{B}}{\partial t}
$$

### Stoke's Theorem
$$
\oint\textbf{B}\cdot\textrm{d}\textbf{s}=\int_{S}\boldsymbol{\nabla}\times\textbf{B}\cdot\textrm{d}\textbf{S}
$$
Sum of magnetic field over a closed path is equal to sum of curl of magnetic field over any surface enclosed by that path.

### Self-Inductance
Any circuit carrying a time-varying current self-induces 'back' EMF which opposes the source EMF. 
$$
\varepsilon_{L}=-\dfrac{\textrm{d}\Phi_{B}}{\textrm{d}t}
$$
For an immobile circuit, $\dfrac{\textrm{d}\Phi_{B}}{\textrm{d}t}\propto\dfrac{\textrm{d}B}{\textrm{d}t}\propto\dfrac{\textrm{d}I}{\textrm{d}t}$, where I is the source current. So, 
$$
\varepsilon_{L}=-L\dfrac{\textrm{d}I}{\textrm{d}t}
$$
Where L is a constant: the inductance. For an ideal solenoid inductor, 
$$
L=\dfrac{\mu_{0}N^{2}A}{l}
$$
which depends only on the geometry of the solenoid. The unit of inductance is the Henry. $1\,H=1\,VsA^{-1}$

### RL circuits
![](https://i.postimg.cc/qvYrSJSY/Screenshot-20221207-043430.png "RL Circuit diagram"){max-width: 350px, display: block, margin: 0 auto}

For an RL circuit at a time t after switch is closed, 
$$
\varepsilon-IR-L\dfrac{\textrm{d}I}{\textrm{d}t}=0
$$
$$
\therefore I(t)=\dfrac{\varepsilon}{R}\left(1-e^{-t/\tau}\right)
$$
Where $\tau=L/R$ is the time constant.

### Energy stored in Magnetic Field
$U=\dfrac{1}{2}LI^{2}\quad$ Energy stored in an Inductor

(analogous to $U=\dfrac{1}{2}\dfrac{Q^{2}}{C}\quad$, Energy stored in Capacitor)

Energy density $u=\dfrac{1}{2}\dfrac{\mu_{0}N^{2}}{l^{2}}I\:\Rightarrow\: u=\dfrac{B^{2}}{2\mu_{0}}$

(analogous to $u=\dfrac{\epsilon_{0}E^{2}}{2}$ for capacitor)

### Oscillations in an LC Circuit
![](https://i.postimg.cc/nVTknC2X/Screenshot-20221207-043017.png "LC Circuit diagram"){max-width: 350px, display: block, margin: 0 auto}

For an LC circuit at a time t after switch is closed, **oscillations** are set up. 
$$
U_{E}=\dfrac{Q^{2}}{2C};\:U_{B}=\dfrac{1}{2}LI^{2}
$$
and total energy remains constant. 
$$
\therefore\dfrac{\textrm{d}^{2}Q}{\textrm{d}t^{2}}=-\dfrac{1}{LC}Q
$$
which is a simple harmonic oscillator equation with solution 
$$
Q=Q_{\textrm{max}}\cos(\omega t)\:\Rightarrow\:I=I_{\textrm{max}}\sin(\omega t)
$$
where $\omega=1/\sqrt{LC}$

### Damped Oscillations in RLC Circuit
![An RLC circuit has an inductor, a resistor, and a capacitor connected in series, as well as a switch. Circuit diagram.](https://i.postimg.cc/XvQMfV3X/Screenshot-20221207-042644.png "RLC Circuit diagram"){max-width: 350px, display: block, margin: 0 auto}

For an RLC circuit at a time t after switch is closed, oscillations are **damped**. Rate of energy loss $-I^{2}R$ is only due to resistor. This results in damped harmonis oscillator equation 
$$
L\dfrac{\textrm{d}^{2}Q}{\textrm{d}t^{2}}+R\dfrac{\textrm{d}Q}{\textrm{d}t}+\dfrac{Q}{C}=0
$$
which has solution 
$$
Q=Q_{\textrm{max}}e^{\frac{Rt}{2L}}\cos(\omega_{d}T)
$$
for light damping, where 
$$
\omega_{d}=\sqrt{\dfrac{1}{LC}-\left(\dfrac{R}{2L}\right)^{2}}
$$

If R exceeds critical value $R_{c}=\sqrt{\dfrac{4L}{C}}$, circuit is overdamped and no oscillations occur.

* * *

## Section 8: Alternating Current
### Introduction to AC
AC voltage (50 Hz, 230V max) is used to replace energy dissipated in an RLC circuit. This EMF delivers an alternating current: 
$$
I=I_{\textrm{max}}\sin(\omega t-\phi)
$$
AC is used because it is easy to generate, transform, and use.

### AC Generators and transformers
#### AC generator

![AC generator consists of a conducting loop rotated in an external magnetic field. One metal brush touches one slip ring, while the other metal brush touches both slip rings.](https://i.postimg.cc/Hk7s9vkb/Screenshot-20221207-053551.png "Diagram of AC generator"){max-width: 350px, display: block, margin: 0 auto}

#### AC Transformer

![Transformer: Primary circiuts has N p coils of wire around iron core, which is connected to N s coils of wire from secondaty circuit.](https://i.postimg.cc/QxFWvbMd/Screenshot-20221207-054218.png "Transformer"){max-width: 350px, display: block, margin: 0 auto}

Primary circuit induces alternating magnetic flux within iron core, which in turn induces voltage drop across secondary coil. 
$$
\varepsilon_{s}=\dfrac{N_{s}}{N_{p}}\varepsilon_{p}
$$

### Simple AC EMF Circuits
#### AC circuit with resistor
Potential difference and current are **in phase**. 
$$
\Delta V_{R}=\Delta V_{\textrm{max}}\sin\omega t
$$
$$
I_{R}=I_{\textrm{max}}\sin\omega t
$$

#### AC circuit with capacitor
The current **leads** the voltage by $\pi/2$. 
$$
\Delta V_{C}=\Delta V_{\textrm{max}}\sin\omega t
$$
$$
I_{C}=I_{\textrm{max}}\sin(\omega t+\dfrac{\pi}{2})
$$
Maximum current can be written in terms of capacitive reactance 
$$
I_{\textrm{max}}=\dfrac{\Delta V_{\textrm{max}}}{X_{C}},\quad X_{C}=\dfrac{1}{\omega C}
$$

#### AC circuit with inductor
The current **lags behind** voltage by $\pi/2$. 
$$
\Delta V_{L}=\Delta V_{\textrm{max}}\sin\omega t
$$
$$
I_{L}=I_{\textrm{max}}\sin(\omega t-\dfrac{\pi}{2})
$$
Inductive reactance: 
$$
I_{\textrm{max}}=\dfrac{\Delta V_{\textrm{max}}}{X_{L}},\quad X_{L}=\omega L
$$

### The RLC Circuit
Use complex notation: $exp(j\omega t)$$\;=\cos\omega t+ j\sin\omega t$ 
$$
\begin{array}{l} \boldsymbol{\varepsilon}=\varepsilon_{\textrm{max}}\exp(j\omega t) & \varepsilon=\Re(\boldsymbol{\varepsilon}) \\ \textbf{I}(t)=\textbf{I}_{0}\exp(j\omega t) & I(t)=\Re(\textbf{I}(t)) \\ \end{array}
$$
Kirchoff's loop rule is now 
$$
\boldsymbol{\varepsilon}-R\textbf{I}-L\dfrac{\textrm{d}\textbf{I}}{\textrm{d}t}-\dfrac{\textbf{Q}}{C}=0
$$
Differentiate and rearrange to find 
$$
\boldsymbol{\varepsilon}=\textbf{IZ}
$$
$$
\textbf{Z}=R+j\left(\omega L-\dfrac{1}{\omega C}\right)
$$
where $\textbf{Z}$ is the complex impedance, which can be written $\textbf{Z}=Z\exp j\phi$ 
$$
Z=\sqrt{R^{2}+(X_{L}-X_{C})^{2}}
$$
$$
\phi=\tan^{-1}\dfrac{X_{L}-X_{C}}{R}
$$
The current can be written 
$$
\textbf{I}=\dfrac{\varepsilon_{\textrm{max}}}{Z}\exp j(\omega t-\phi)
$$

*   The voltage leads the current if $X_{L}\gt X_{C}$
*   The voltage lags behind the current if $X_{L}\lt X_{C}$
*   When $X_{L}=X_{C}$, $\omega_{0}=1/\sqrt{LC}$
*   At resonant frequency, impedance equals resistance, voltage is in phase with current and current it at maximum value.


### Power in an RLC circuit
Energy stored oscillates between capacitor and inductor, and is dissipated in resistor. 
$$
\langle P\rangle_{t}=\dfrac{1}{2}I_{\textrm{max}}\Delta V_{\textrm{max}}\cos\phi
$$
$$
I_{\textrm{rms}}=\dfrac{1}{\sqrt{2}}I_{\textrm{max}}
$$
$$
\Delta V_{\textrm{rms}}=\dfrac{1}{\sqrt{2}}\Delta V_{\textrm{max}}
$$
$$
\therefore\langle P\rangle_{t}=I_{\textrm{rms}}\Delta V_{\textrm{rms}}\cos\phi
$$
$$
\langle P\rangle_{t}=I_{\textrm{rms}}^{2}R
$$
$$
\langle P\rangle_{t}=\dfrac{(\Delta V_{\textrm{rms}})^{2}R\omega^{2}}{R^{2}\omega^{2}+L^{2}(\omega^{2}-\omega_{0}^{2})^{2}}
$$
At resonance 
$$
\langle P\rangle_{t\textrm{ max}}=\dfrac{(\Delta V_{\textrm{rms}})^{2}}{R}
$$
Quality factor 
$$
Q=\dfrac{\omega_{0}}{\Delta\omega}
$$
where $\Delta\omega$ is the full width at half-maximum.

### Maxwell's equations

Maxwell equation | Differential Form | Integral Form
------|--------|------
Gauss' law | $\boldsymbol{\nabla}\cdot\textbf{E}=\dfrac{\rho}{\epsilon_{0}}$ | $\displaystyle\int_{S}\textbf{E}\cdot\textrm{d}\textbf{S}=\dfrac{Q_{\textrm{encl.}}}{\epsilon_{0}}$
Gauss' law for magnetism | $\boldsymbol{\nabla}\cdot\textbf{B}=0$ | $\displaystyle\int_{S}\textbf{B}\cdot\textrm{d}\textbf{S}=0$
Faraday's law | $\boldsymbol{\nabla}\times\textbf{E}=-\dfrac{\partial\textbf{B}}{\partial t}$ | $\displaystyle\oint\textbf{E}\cdot\textrm{d}\textbf{s}=-\dfrac{\textrm{d}\Phi_{B}}{\textrm{d}t}$
Ampère-Maxwell law | $\boldsymbol{\nabla}\times\textbf{B}=\mu_{0}\textbf{J}+\epsilon_{0}\mu_{0}\dfrac{\partial\textbf{E}}{\partial t}$ | $\displaystyle\oint\textbf{B}\cdot\textrm{d}\textbf{s}=\mu_{0}I+\epsilon_{0}\mu_{0}\dfrac{\textrm{d}\Phi_{E}}{\textrm{d}t}$

  

### Waves in free space
No charges or currents present. Gauss' law for electrostatics and the Ampère-Maxwell law simplify to: 
$$
\boldsymbol{\nabla}\cdot\textbf{E}=0
$$
$$
\boldsymbol{\nabla}\times\textbf{B}=\epsilon_{0}\mu_{0}\dfrac{\partial\textbf{E}}{\partial t}
$$
From which the wave equations for electromagnetic waves can be derived. 
$$
\nabla^{2}\textbf{E}=\mu_{0}\epsilon_{0}\dfrac{\partial^{2}\textbf{E}}{\partial t^{2}}
$$
$$
\nabla^{2}\textbf{B}=\mu_{0}\epsilon_{0}\dfrac{\partial^{2}\textbf{B}}{\partial t^{2}}
$$
which have speed 
$$
c=\dfrac{1}{\sqrt{\mu_{0}\epsilon_{0}}}
$$
