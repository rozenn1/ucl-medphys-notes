---
id: 7p6y1ynwrgmnxpv5fe80j0i
title: PHAS0022
desc: ''
updated: 1679912359016
created: 1679910845021
---

# Quantum Physics
_last updated on 13/12/2022_

* * *

### CONTENTS:

*   **Section 1** : Recap of key concepts
*   **Section 2** : Steps towards wave mechanics
*   **Section 3** : Postulates of quantum mechanics
    *   Postulate 1: The wavefunction
    *   Postulate 2: Operators
    *   Postulate 3: Constructing operators
    *   Postulate 4: Probability
    *   Postulate 5: Time evolution of the wavefunction
*   **Section 4** : One-dimensional time-independent problems
    *   4.1 The infinite square well
    *   4.2 The finite square well
    *   4.3 The potential step and particle flux
    *   4.4 Quantum tunnelling
    *   4.5 The Harmonic oscillator
*   **Section 5** : Periodic potentials
*   **Section 6** : Commutation and Perturbation theory
    *   6.1 Compatible operators
    *   6.2 Perturbation theory
*   **Section 7** : Angular Momentum
    *   7.1 Angular momentum operators
    *   7.2 Spherical Harmonics
*   **Section 8** : Three dimensional problems and the Hydrogenic atom
    *   8.1 The Schrödinger equation in 3D
    *   8.2 The three-dimensional box
    *   8.3 The hydrogenic atom
*   **Section 9** : Electron spin and total angular momentum
    *   9.1 Orbital Magnetic Momentum
    *   9.2 The Stern-Gerlach experiment
    *   9.3 Operators for spin

  

* * *

  

Section 1 : Recap of key concepts
---------------------------------

#### The photoelectric effect

The photoelectric effect demonstrated that electromagnetic radiation acted as wave-particle dualities. Materials sometimes emit photo-electrons when irradiated with light. Only light above a certain frequency ($\propto$ Energy) caused this effect. This cannot be explained by classical physics alone. 
$$
E=hf\qquad E_{K max}=hf-\phi
$$
The quantisation of light involves the Planck constant, a fundamental constant of physics. 
$$
\hbar=\dfrac{h}{2\pi}\qquad E=hf=\hbar\omega
$$

$$
h=6.6261\times 10^{-34} Js = 4.1357 \times 10^{-15} eV s
$$

$$
\hbar=1.0546\times 10^{-34} Js = 6.5821 \times 10^{-16} eV s
$$

  

#### Compton scattering

Compton scattering is the scattering of high energy x-rays from free electrons. Experiments show that scattered x-rays have longer wavelengths, whereas classical physics predictes no wavelength shift. The process must be treated relativistically.

![Before: Incoming photon has energy E0 and momentum p0, and is about to collide with an electron of energy m e, c squared. After: Photon has scattered at angle theta with energy E1 momentum p1, electron scattered at angle phi with energy E e momentum p e.](https://i.postimg.cc/LsDq27t4/Screenshot-20221116-083937.png "Compton scattering schematic. [B&M Sect. 2.7]"){max-width: 400px, display: block, margin: 0 auto}

Compton scattering schematic.

Consider this an elastic scattering problem, and use conservation of energy and momentum.

*   Conservation of momentum: $p_{0}+0=p_{1}+p_{e}$
*   Conservation of energy: $E_{0}+m_{e}c^{2}=E_{1}+E_{e}$
*   Relativity: $E=\sqrt{m^{2}c^{4}+p^{2}c^{2}}$ (electron; particle with mass)
*   Relativity: $E=pc$ (photon; massless particle)
*   Quantum: $E=hf$

There is a shifted wavelength due to scattering of a photon from a free electron, and an unshifted peak due to scattering off of nucleus or bound electron. 
$$
\Delta\lambda=\lambda_{C}(1-\cos{\theta})
$$

$$
\lambda_C\equiv\dfrac{h}{m_{e}c}
$$

  

#### Matter waves

Define wave number $k$ as 
$$
k=\dfrac{2\pi}{\lambda}
$$
so we can write 
$$
p=\hbar k
$$
Or using general vector quantities momentum and wave vector 
$$
\textbf{p}=\hbar\textbf{k}
$$
Applying these concepts to matter instead of photons, de Broglie postulated that any object having momentum has an associated wavelength, and 
$$
E=\hbar\omega
$$

$$
p=\hbar k
$$

  

#### The double slit experiment

Coherent waves pass throgh two slits and form interference fringes. They are observed even if only one particle goes through the slits at a time.

  

#### The Heisenberg Uncertainty Principle

Position and momentum cannot be known with absolute precision at the same time. 
$$
\Delta x\Delta p_{x}\geq\dfrac{\hbar}{2}
$$

  

* * *

  

Section 2 : Steps towards wave mechanics
----------------------------------------

The wave equation for electromagnetic waves does not work for matter waves. In order to satisfy $E=\hbar\omega$ and $E=p^{2}/2m$, frequency must be $\omega\propto k^{2}$. This motivates the existence of the **Time-dependent Schrödinger equation**. 
$$
i\hbar\dfrac{\partial\Psi}{\partial t}=\dfrac{-\hbar^{2}}{2m}\dfrac{\partial^{2}\Psi}{\partial x^{2}}+V\Psi
$$
where $\Psi\equiv\Psi(x,t)$, and $V\equiv V(x,t)$. The wave solution to the time dependent Schrödinger equation is the complex wavefunction $\Psi=\Psi(x,t)$, or $\Psi=(\textbf{r},t)$ in three dimensions.

When $V(x,t)\equiv V(x)$, separation of variables $\Psi(x,t)=\psi(x)T(t)$ can be used to find 
$$
T(t)=\exp\left(\dfrac{-iEt}{\hbar}\right)
$$
and the **Time-independent Schrödinger equation** 
$$
\dfrac{-\hbar^{2}}{2m}\dfrac{\textrm{d}^{2}\psi(x)}{\textrm{d}x^{2}}+V(x)\psi(x)=E\psi(x)
$$
which depends on the form of the potential.

  

* * *

  

Section 3 : Postulates of quantum mechanics
-------------------------------------------

### Postulate 1: The wavefunction

*   The wavefunction exists and contains all information about the physical properties of the system.
*   It is a continuous, square-integrable, single valued, complex function of the parameters of all the partcles and of time.

The Born rule 
$$
P(a\leq x\leq b)=\int_{a}^{b}{\left|\Phi(x,t)\right|^{2}}dx
$$
The wavefunction is normalised such that total probability = 1.

  

### Postulate 2: Operators

*   Each observable is associated with a linear Hermitian operator. Hermitian, so that the eigenvalues are real.
*   Eigenvalues of the operator are the possible results of measurements.
*   Immediately after making a measurement, the wavefunction $\psi$ collapses to the eigenfunction $\phi$ corresponding to the result of the measurement.

Eigenvalue equation 
$$
\hat{Q}\phi_{n}=q_{n}\phi{n}
$$
Hermitian operator 
$$
\int f^{*}(\tau)\hat{Q}g(\tau)\;d\tau=\int\left(\hat{Q}f(\tau)\right)^{*}g(\tau)\;d\tau
$$
Linear operator 
$$
\hat{Q}(c_{1}f_{1}+c_{2}f_{2})=c_{1}\hat{Q}(f_{1})+c_{2}\hat{Q}(f_{2})
$$

Eigenfunctions are orthogonal, and can be normalised to form an **orthonormal** system. This results in the completeness condition - that any function can always be expressed as an expansion in terms of eigenfunctions. 
$$
\int\phi_{n}^{*}\,\phi_{m}\;d\tau=\delta_{nm}=\left\{\begin{array}{l}1\quad\textrm{if }m=n\\0\quad\textrm{if }m\neq n\\\end{array} \right.
$$

$$
\psi=\sum_{n}a_{n}\phi_{n}\qquad a_{n}\in\mathbb{C}
$$

$$
a_{n}=\int \phi_{n}^{*}\,\psi\;d\tau
$$

  

### Postulate 3: Constructing operators

*   The operators representing the position and momentum of a particle are: 
$$
\textrm{In 1D:}\qquad\hat{X}=x;\qquad\hat{P}=-i\hbar\dfrac{\textrm{d}}{\textrm{d}x}
$$

$$
\textrm{In 3D:}\qquad\hat{\textbf{R}}=\textbf{r};\qquad\hat{\textbf{P}}=-i\hbar\boldsymbol{\nabla}
$$
*   Operators representing other dynamical quantities have the same functional relation to these as in classical physics.

Immediately after a position measurement is made, the wavefunction is given by the Delta Dirac function. 
$$
\delta(x-x_{0})=\left\{ \begin{array}{l}+\infty\quad\textrm{if }x=x_{0}\\0\qquad\textrm{otherwise,}\end{array}\right.
$$
and 
$$
\int_{-\infty}^{\infty}{f(x)\delta(x-x_{0})}dx=f(x_{0})
$$

$$
\int_{-\infty}^{\infty}{\delta(x-x_{0})}dx=1
$$

  

### Postulate 4: Probability

When a measurement is carried out on a wavefunction $\psi$, the probability of the result being equal to a particular eigenvalue $q_{m}$ is 
$$
\left|a_{m}\right|^{2},\quad\textrm{where}
$$

$$
\psi=\sum_{n}a_{n}\phi_{n}
$$
So if a system is definitely in eigenstate $\phi_{n}$, the result of measuring $\hat{Q}$ is definitely $q_{n}$.

The average value over a set of repeated measurements is the expectation value. The expectation value of an observable represented by $\hat{Q}$ for a system in state $\psi$ is 
$$
\left\langle\hat{Q}\right\rangle=\int{\psi^{*}\hat{Q}\psi\;d\tau}
$$

$$
\left\langle\hat{Q}\right\rangle=\sum_{n}\left|a_{n}\right|^{2}q_{n}
$$

  

### Postulate 5: Time evolution of the wavefunction

Between measurements, the wavefunction evolves according to the time dependent Schrödinger equation 
$$
\hat{H}\Psi=i\hbar\dfrac{\partial\Psi}{\partial t}
$$

$$
\hat{H}=\dfrac{-\hbar^{2}}{2m}\nabla^{2}+V(\textbf{r},t)
$$
Thus, when $V(x,t)\equiv V(x)$, the stationary state solutions are 
$$
\Psi(x,t)=\phi(x)\exp\left(\dfrac{-iEt}{\hbar}\right)
$$
It is called a stationary state as only phase changes with time, not the probability distribution function.

In general, for a superposition of multiple states, time dependence of the wavefunction is 
$$
\Psi(x,t)=\sum_{n}a_{n}\phi_{n}(x)\exp\left(\dfrac{-iE_{n}t}{\hbar}\right)
$$

Rate of change of the expectation value, where $\left[\hat{Q},\hat{H}\right]$ is the commutator $\hat{Q}\hat{H}-\hat{H}\hat{Q}$ 
$$
\dfrac{\text{d}}{\text{d}t}\left\langle\hat{Q}\right\rangle=\left\langle\dfrac{\partial\hat{Q}}{\partial t}\right\rangle+ \dfrac{1}{i\hbar}\left\langle\left[\hat{Q},\hat{H}\right]\right\rangle
$$

  

* * *

  

Section 4 : One-dimensional time-independent problems
-----------------------------------------------------

### 4.1 The infinite square well

![When x is less than -a or more than +a, potential V(x) is infinite. When x is between -a and +a, potential V(x) is 0.](https://i.postimg.cc/nz7GPp0P/Screenshot-20221119-110525.png "The infinite square well in 1D"){max-width: 400px, display: block, margin: 0 auto}

The infinite square well

The wavefunction cannot exist in the infinite potential regions, but can take a free particle form in the zero potential regions. Using continuity boundary conditions and the time-independent Schrödinger equation, the solution is 
$$
\psi_{n}(x)=\left\{\begin{array}{l} \dfrac{1}{\sqrt{a}}\cos{\left(\dfrac{n\pi}{2a}x\right)} & \textrm{for}\quad n=1,3,5,\dots \\ \dfrac{1}{\sqrt{a}}\sin{\left(\dfrac{n\pi}{2a}x\right)} & \textrm{for}\quad n=2,4,6,\dots \\ \end{array}\right.
$$
where 
$$
E_{n}=\dfrac{\hbar^{2}\pi^{2}}{8ma^{2}}n^{2}
$$
$n$ is the quantum number for this system.

![Energy increases with n squared. Wavefunction alternates between sinusoidal and cosinusoidal solutions between energy levels. As energy level increases, the period of the solutions decreases. Probability density is proportional to wavefunction squared.](https://i.postimg.cc/SsytCXyG/Screenshot-20221119-111756.png "Solutions to the infinite square well"){max-width: 400px, display: block, margin: 0 auto}

The first four solutions to the infinite square well. The energy  
levels are $E_{n}\propto n^{2}$. $E_{1}$ is the ground state of the system.

  

### 4.2 The finite square well

![When x is less than -a or more than +a, potential V(x) is a constant V0. When x is between -a and +a, potential V(x) is 0.](https://i.postimg.cc/wTgqb2wq/Screenshot-20221119-113022.png "The finite square well in 1D"){max-width: 400px, display: block, margin: 0 auto}

The finite square well

The wavefunction must not diverge at $\pm\infty$, and continuity boundary conditions apply at $x=\pm a$. The solution is a free particle for the zero potential region and an exponential decay for the finite potential region.

![Similar to infinite square well solutions, except that the wavefunction penetrates into the classically forbidden region as an exponential decay.](https://i.postimg.cc/4xHyt5wX/Screenshot-20221119-114733.png "Solutions to the finite square well."){max-width: 400px, display: block, margin: 0 auto}

First four solutions to the finite square well.

![Similar to infinite square well probability densities, except that the wavefunction has finite probability of existing in the classically forbidden region as an exponential decay.](https://i.postimg.cc/s2crZGFV/Screenshot-20221119-114825.png "Solutions to the finite square well."){max-width: 400px, display: block, margin: 0 auto}

Their corresponding probability density functions.

  

### 4.3 The potential step and particle flux

Travelling waves are not square integrable over all space. This issue is resolved by considering a plane wave as a beam of particles. This introduces the concept of particle flux, which in 1D represents the number of particles passing a point per second. 
$$
\Gamma(x)=\dfrac{-i\hbar}{2m}\left(\Psi^{*}\dfrac{\partial\Psi}{\partial x}-\Psi\dfrac{\partial\Psi^{*}}{\partial x}\right)
$$

Consider a potential step. When $E\lt V_{0}$, there is some penetration of particles into the classically forbidden region, but there is eventually 100% reflection. When $E\gt V_{0}$, reflection probability does not immediately fall to zero, but instead interferes with the incident wave, although it decays to 0 for very large $E$. 
$$
R=\left|\dfrac{\textrm{reflected flux}}{\textrm{incident flux}}\right|;\qquad T=\left|\dfrac{\textrm{transmitted flux}} {\textrm{incident flux}}\right|
$$
where $R+T=1$.

  

### 4.4 Quantum tunnelling

![Potential V(x) is constant V0 for x between 0 and a, and is 0 otherwise. Energy of the particle beam E is between 0 and V0.](https://i.postimg.cc/gjMd0mkk/Screenshot-20221119-014235.png "The potential barrier in 1D"){max-width: 400px, display: block, margin: 0 auto}

The potential barrier

Consider a potential barrier. Transmission probability is dependent on the width of the barrier.  
Small $E$ approximation 
$$
T=\dfrac{16E(V_{0}-E)}{V_{0}^{2}}e^{-2\kappa a}
$$
For all $E$, quantum mechanics predicts oscillations in transmission probability as a function of energy.

![As energy approaches the height of the barrier, transmission probability grows exponentially until 1. For larger energies, Transmission probability oscillates, only reaching 1 for discrete values of E.](https://i.postimg.cc/gk6BjG0S/Screenshot-20221119-014344.png "Transmission probability at different Energy values for the barrier potential"){max-width: 600px, display: block, margin: 0 auto}

Transmission probability v. Energy of particle beam

  

### 4.5 The Harmonic oscillator

Consider a quantum harmonic oscillator in a potential $V(x)=\dfrac{1}{2}\omega_{0}^{2}m x^{2}$. Changing variables, 
$$
\psi''(y)+(\alpha-y^{2})\psi(y)=0
$$
where 
$$
y=\sqrt{\dfrac{m\omega_{0}}{\hbar}}x\quad\textrm{and}\quad\alpha=\dfrac{2E}{\hbar\omega_{0}}
$$
Considering the asymptotic behaviour of the wavefunction 
$$
H''(y)-2yH'(y)+(\alpha-1)H(y)=0
$$

$$
\psi(y)=H(y)e^{y^{2}/2}
$$
where $H(y)$ are the Hermite polynomials. 
$$
\phi_{n}(x)=A_{n}H_{n}\left(\sqrt{\dfrac{m\omega_{0}}{\hbar}}x\right)\exp{\left(-\dfrac{m\omega_{0}x^{2}}{2\hbar}\right)}, \:n=0,1,2,3,...
$$

$$
E=\hbar\omega_{0}\left(n+\dfrac{1}{2}\right),\:n=0,1,2,3,...
$$

  

* * *

  

Section 5 : Periodic potentials
-------------------------------

Consider the Schrödinger equation for an electron in a crystal lattice, while making the following approximations:

*   Born-Oppenheimer approximation: nuclei are in fixed positions.
*   Independent electron approximation: no electron-electron interactions.
*   One dimention: only consider one spatial dimension.

For a completely free electron ($V(x)=0$): $E(k)=\dfrac{\hbar^{2}k^{2}}{2m}$. Thus the dispersion relation is

![Dispersion relation E(k) vs k is a quadratic parabola](https://i.postimg.cc/G202nb90/Screenshot-20221120-112803.png "Dispersion relation for free particle"){max-width: 400px, display: block, margin: 0 auto}

Dispersion relation for a free electron

Consider confining this electron such that it can only exist within some macroscopic length L. The dispersion relation becomes $E_{n}=\dfrac{\hbar^{2}\pi^{2}n^{2}}{2mL^{2}}$ (quantised)

![Quadratic relation, but only discrete energies are allowed.](/assets/images/2023-03-27-11-06-57.png){max-width: 400px, display: block, margin: 0 auto}

Dispersion relation for a confined particle.

The Pauli exclusion principle states that no two electrons can have all quantum numbers identical. Since electrons can have spin $m_{s}=\pm 1/2$, $n_{F}=N/2$ is the topmost filled energy state (Fermi level) with Fermi energy 
$$
E_{F}=\dfrac{\hbar^{2}\pi^{2}n_{F}^{2}}{2mL^{2}}
$$

Crystal lattices have periodic potentials with periodic boundary conditions 
$$
V(x+na)=V(x)\quad n=1,2,3,...
$$

$$
\psi(x+Na)=\psi(x)
$$
Considering this, we find 
$$
\psi(x+a)=\psi(x)e^{ika}\:\textrm{where}\: k=\dfrac{2\pi n}{Na},\: n=0,\pm 1,\pm, 2,...
$$
Which is consistent with Bloch's Theorem 
$$
\psi(x)=u(x)e^{ikx}\:\textrm{where}\: u(x)=u(x+a)
$$
$k$ is crystal wave number and $\hbar k$ is crystal momentum.

  

#### The Kronig-Penney Model

![Square potential barrier is taken to the limit where width becomes zero and height becomes infinity.](https://i.postimg.cc/g0MVVSzt/Screenshot-20221120-121653.png "Kronig-Penney Model: Potentials become delta function barriers"){max-width: 200px, display: block, margin: 0 auto}

Taking the Dirac delta potentials limit

*   The Kronig-Penney model involves replacing finite potential barriers by $\delta$-function barriers.
*   Consider barriers of width $b$ and height $h$.
*   Take the limit $b\rightarrow 0$ while keeping the area fixed. 
$$
\int_{0}^{b} h\, dx=hb=V_{0}
$$
*   This results in Dirac delta function potentials, thus our periodic potential becomes 
$$
V(x)=V_{0}\sum_{n}\delta(x-na)
$$
Note that this causes discontinuity in the gradient of the wavefunction. 
$$
\left.\dfrac{\textrm{d}\psi}{\textrm{d}x}\right|_{\epsilon}-\left.\dfrac{\textrm{d}\psi}{\textrm{d}x}\right|_{-\epsilon}= \dfrac{2mV_{0}}{\hbar^{2}}\psi(0)
$$

Using continuity of the wavefunction and discontinuity of the gradient of the wavefunction as boundary conditions, a coefficients matrix can be found 
$$
\left(\begin{array}{c} e^{i\alpha a}-e^{ika} & e^{-i\alpha a}-e^{ika} \\ -i\alpha\left(e^{i\alpha a}-e^{ika}\right)-\dfrac{2mV_{0}}{\hbar^{2}}e^{ika} & i\alpha\left(e^{-i\alpha a}-e^{ika}\right)- \dfrac{2mV_{0}}{\hbar^{2}}e^{ika} \\ \end{array}\right) \left(\begin{array}{l}A\\B\\\end{array}\right) =\left(\begin{array}{l}0\\0\\\end{array}\right)
$$
For a wavefunction $\psi(x)=Ae^{i\alpha x}+Be^{-i\alpha x}\quad(0\lt x\lt a)$. This yields the Kronig-Penney result for the $\delta$ function periodic potential 
$$
\dfrac{mV_{0}}{\alpha\hbar^{2}}\sin{(\alpha a)}+\cos{(\alpha a)}=\cos{(ka)}
$$
The $\cos{(ka)}$ term on the right hand side can only take certain values, so this results in allowed energy bands. The zone edges of the band gaps develop at $ka=n\pi$.

![Dispersion relation has approximately quadratic shape but only exists in certain allowed energy bands.](https://i.postimg.cc/vZ1J2F7R/Screenshot-20221120-032758.png "Solution to periodic potential using Kronig-Penney model"){max-width: 400px, display: block, margin: 0 auto}

Solution to finite periodic potential

  

* * *

  

Section 6 : Commutation and Perturbation theory
-----------------------------------------------

### 6.1 Compatible operators

*   We define the commutator of two operators as 
$$
\left[\hat{A},\hat{B}\right]\equiv\hat{A}\hat{B}-\hat{B}\hat{A}
$$
*   Two operators are said to commute if 
$$
\left[\hat{A},\hat{B}\right]=0
$$


$$
\left[\hat{A},\hat{A}\right]=0,\qquad\left[\hat{A},\hat{B}\right]=-\left[\hat{B},\hat{A}\right]
$$

$$
\left[\hat{X}_{i},\hat{X}_{j}\right]=0,\qquad\left[\hat{P}_{i},\hat{P}_{j}\right]=0
$$

$$
\left[\hat{P}_{i},\hat{X}_{j}\right]=-i\hbar\delta_{ij}\qquad i,j\in\{1,2,3\}
$$

Two physical observables are **compatible** if their operators have a common set of eigenfunctions. We assume eigenfunctions are non-degenerate: that they do not share the same eigenvalue.

Compatible operators commute. Commuting operators are compatible in the non-degenerate case.

  

### 6.2 Perturbation theory

Suppose we have a simple potential, to which we add a small perturbation such that 
$$
\hat{H}=\hat{H}^{(0)}+\lambda\hat{H}'
$$
where $\lambda$ is a parameter $0\lt\lambda\lt 1$. We assume that we can expand the eigenfunctions and eigen energies of the full Hamiltonian as a power series in $\lambda$. First order energy correction is 
$$
E_{n}^{(1)}=\left\langle\hat{H}'\right\rangle
$$

  

* * *

  

Section 7 : Angular Momentum
----------------------------

### 7.1 Angular momentum operators


$$
\boldsymbol{\hat{L}}=\boldsymbol{\hat{R}}\times\boldsymbol{\hat{P}}=-i\hbar\boldsymbol{r}\times\boldsymbol{\nabla}\quad \Rightarrow\quad\hat{L}_{i}=\epsilon_{ijk}\hat{R}_{j}\hat{P}_{k}
$$
If $i,j,k$ are taken to be summed over cartesian coordinates $x,y,z$.

The following commutation relations apply: 
$$
\left[\hat{L}_{i},\hat{L}_{j}\right]=i\hbar\,\epsilon_{ijk}\hat{L}_{k}
$$

$$
\left[A^{2},B\right]=A[A,B]+[A,B]A\quad\Rightarrow\quad\therefore\left[\hat{L}^{2},\hat{L}_{i}\right]=0\quad\forall i\in\{1,2,3\}
$$

$$
\textrm{where }\hat{L}^{2}=\sum_{i=1}^{3}\hat{L}_{i}^{2}
$$

This means we cannot know all components of angular momentum at the same time, but we **can** know $\hat{L}^{2}$ and $\hat{L}_{z}$ at the same time, where $z$ is, by convention, the quantisation axis. Derive expressions for angular momentum in polar coordinates: 
$$
\begin{array}{l} x=r\sin\theta\cos\phi &&& r\geq 0 \\ y=r\sin\theta\sin\phi &&& 0\leq\theta\leq\pi \\ z=r\cos\theta &&& 0\leq\phi\leq 2\pi \\ \end{array}
$$

$$
\hat{\textbf{e}}_{\textbf{r}}=\left(\begin{array}{c}\sin\theta\cos\phi\\\sin\theta\sin\phi\\\cos\theta\end{array}\right)\quad \hat{\textbf{e}}_{\theta}=\left(\begin{array}{c}\cos\theta\cos\phi\\\cos\theta\sin\phi\\-\sin\theta\end{array}\right)\quad \hat{\textbf{e}}_{\phi}=\left(\begin{array}{c}-\sin\phi\\\cos\phi\\0\end{array}\right)
$$

$$
\boldsymbol{\hat{L}}=-i\hbar\left(\hat{\textbf{e}}_{\phi}\dfrac{\partial}{\partial\theta}-\hat{\textbf{e}}_{\theta} \dfrac{1}{\sin\theta}\dfrac{\partial}{\partial\phi}\right)
$$

$$
\because\boldsymbol{\nabla}=\hat{\textbf{e}}_{\textbf{r}}\dfrac{\partial}{\partial r}+\hat{\textbf{e}}_{\theta}\dfrac{1}{r} \dfrac{\partial}{\partial\theta}+\hat{\textbf{e}}_{\phi}\dfrac{1}{r\sin\theta}\dfrac{\partial}{\partial\phi}
$$
So 
$$
\hat{L}_{z}=\hat{\textbf{e}}_{k}\cdot\boldsymbol{\hat{L}}=-i\hbar\dfrac{\partial}{\partial\phi}
$$

$$
\because\hat{\textbf{e}}_{k}=\hat{\textbf{e}}_{r}\cos\theta-\hat{\textbf{e}}_{\theta}\sin\theta
$$
and 
$$
\hat{L}^{2}=-\hbar^{2}\left(\dfrac{1}{\sin\theta}\dfrac{\partial}{\partial\theta}\left(\sin\theta\dfrac{\partial}{\partial\theta} \right)+\dfrac{1}{\sin^{2}\theta}\dfrac{\partial^{2}}{\partial\phi^{2}}\right)
$$

  

### 7.2 Spherical Harmonics

Find eigenvalues and eigenfunctions of angular momentum. 
$$
\begin{array}{c}\hat{L}_{z}\Phi(\phi)=\lambda\Phi(\phi)\\-i\dfrac{\textrm{d}}{\textrm{d}\phi}\Phi(\phi)=\lambda\Phi(\phi)\\ \end{array}\quad\Rightarrow\quad\Phi(\phi)=\dfrac{1}{\sqrt{2\pi}}e^{im\phi}
$$
where $m$ is an integer and $\lambda=m\hbar$ are the eigenvalues of $\hat{L}_{z}$. 
$$
\hat{L}^{2}Y(\theta,\phi)=\beta\hbar^{2}Y(\theta,\phi)\qquad(-l\leq m\leq l)
$$
where $\beta\hbar^{2}=l(l+1)\hbar^{2}$ and $Y(\theta,\phi)=\Theta(\theta)\Phi(\phi)$ are the **Spherical Harmonics**. 
$$
-\dfrac{1}{\sin\theta}\dfrac{\partial}{\partial\theta}\left(\sin\theta\dfrac{\partial\Theta}{\partial\theta}\right)+ \dfrac{m^{2}}{\sin^{2}\theta}\Theta=\beta\Theta
$$
is the Legendre equation.

  


$$
\begin{array}{l}Y_{lm}(\theta,\phi)=\Theta_{l}(\theta)\Phi_{m}(\phi)\\ \qquad=(-1)^{m}\left[\dfrac{(2l+1)}{4\pi}\dfrac{(l-|m|)!}{(l+|m|)!}\right]^{1/2}P_{l}^{m}(\cos\theta)e^{im\phi}\\\end{array}
$$
Where $P_{l}^{m}$ are the associated Legendre functions 
$$
P_{l}^{m}(\mu)\equiv\left(1-\mu^{2}\right)^{|m|/2}\left(\dfrac{\textrm{d}}{\textrm{d}\mu}\right)^{|m|}P_{l}(\mu)
$$
and $P_{l}$ are the Legendre Polynomials 
$$
P_{l}(\mu)\equiv\dfrac{1}{2^{l}l!}\left(\dfrac{\textrm{d}}{\textrm{d}\mu}\right)^{l}\left(\mu^{2}-1\right)^{l}
$$

  

The eigenvalues of $\hat{L}^{2}$ are 
$$
l(l+1)\hbar^{2}\quad\textrm{with}\quad l=0,1,2,3,\dots
$$
$l$ is orbital angular momentum quantum number (or azimuthal quantum number); it determines the magnitude of angular momentum.

The eigenvalues of $\hat{L}_{z}$ are 
$$
m\hbar\quad\textrm{with}\quad m=-l,\dots,-1,0,1,\dots,l
$$
$m$ is magnetic quantum number; it determines the component of angular momentum along the quantisation axis.

  

* * *

  

Section 8 : Three dimensional problems and the Hydrogenic atom
--------------------------------------------------------------

### 8.1 The Schrödinger equation in 3D

The time-dependent Schrödinger equation in three dimensions is 
$$
i\hbar\dfrac{\partial\Psi}{\partial t}=\left(-\dfrac{\hbar}{2m}\nabla^{2}+V(\textbf{r})\right)\Psi
$$
and the time-independent Schrödinger equation is 
$$
\left(-\dfrac{\hbar}{2m}\nabla^{2}+V(\textbf{r})\right)\psi=E\psi
$$

Consider the case where the potential $V(\textbf{r})$ can be written 
$$
V(\textbf{r})=V_{1}(x)+V_{2}(y)+V_{3}(z)
$$
such that 
$$
\psi(\textbf{r})=X(x)Y(y)Z(z)
$$
This results in three variable-separated equations 
$$
\left.\begin{array}{l} -\dfrac{\hbar^{2}}{2m}\dfrac{\textrm{d}^{2}X}{\textrm{d}x^{2}}+V_{1}X=E_{x}X \\ -\dfrac{\hbar^{2}}{2m}\dfrac{\textrm{d}^{2}Y}{\textrm{d}y^{2}}+V_{1}Y=E_{y}Y \\ -\dfrac{\hbar^{2}}{2m}\dfrac{\textrm{d}^{2}Z}{\textrm{d}z^{2}}+V_{1}Z=E_{z}Z \\ \end{array}\right\}E_{x}+E_{y}+E_{z}=E
$$

  

### 8.2 The three-dimensional box

Consider a three-dimensional equivalent to the infinite square well, such that a particle is only allowed to exist within a square box of side length $2a$. 
$$
V(\textbf{r})=\left\{\begin{array}{l} 0 & \textrm{if } -a\leq x,y,z \leq a \\ \infty & \textrm{otherwise.} \\ \end{array}\right.
$$
In each direction, the solution is of the form 
$$
E_{x}=\dfrac{\hbar^{2}\pi^{2}}{8ma^{2}}n_{x}^{2},\quad n_{x}=1,2,3,\dots
$$
such that total energy is 
$$
E_{n_{x}n_{y}n_{z}}=\dfrac{\hbar^{2}\pi^{2}}{8ma^{2}}\left(n_{x}^{2}+n_{y}^{2}+n_{z}^{2}\right)
$$
Note that three quantum numbers are needed to specify a three-dimensional state, and that the eigen energies are degenerate.

The eigenfunction bound state solutions in each direction are 
$$
\phi_{n}(x)=a^{-1/2}\left\{\begin{array}{l}\cos\\\sin\\\end{array}\right\}\left(\dfrac{n\pi x}{2a}\right)\quad\textrm{for}\:-a\leq x\leq a
$$
cosine if $n$ is odd, sine if $n$ is even. Total wavefunction within three-dimensional box is 
$$
\phi_{n_{x}n_{y}n_{z}}=a^{-3/2}\left\{\begin{array}{l}\cos\\\sin\\\end{array}\right\}\left(\dfrac{n_{x}\pi x}{2a}\right)\left\{\begin{array}{l}\cos\\\sin\\\end{array}\right\}\left(\dfrac{n_{y}\pi y}{2a}\right)\left\{\begin{array}{l}\cos\\\sin\\\end{array}\right\}\left(\dfrac{n_{z}\pi z}{2a}\right)
$$

  

### 8.3 The hydrogenic atom

The potential energy function for a hydrogenic atom is the Coulomb potential 
$$
V(r)=\dfrac{-Ze^{2}}{4\pi\epsilon_{0}}\dfrac{1}{r}
$$
Note that it is spherically symmetrical. The Hamiltonian becomes 
$$
\hat{H}=-\dfrac{\hbar^{2}}{2m_{e}}\nabla^{2}-\dfrac{Ze^{2}}{4\pi\epsilon_{0}}\dfrac{1}{r}
$$
where the Laplacian in spherical coordinates is 
$$
\nabla^{2}=\dfrac{1}{r^{2}}\dfrac{\partial}{\partial r}\left(r^{2}\dfrac{\partial}{\partial r}\right)+\dfrac{1}{r^{2}\sin\theta}\dfrac{\partial}{\partial\theta}\left(\sin\theta\dfrac{\partial}{\partial\theta}\right)+\dfrac{1}{r^{2}\sin^{2}\theta}\dfrac{\partial^{2}}{\partial\phi^{2}}
$$
Noting the form of $\hat{L}^{2}$, 
$$
\hat{H}=-\dfrac{\hbar^{2}}{2m_{e}}\dfrac{1}{r^{2}}\dfrac{\partial}{\partial r}\left(r^{2}\dfrac{\partial}{\partial r}\right)+\dfrac{\hat{L}^{2}}{2m_{e}r^{2}}-\dfrac{Ze^{2}}{4\pi\epsilon_{0}}\dfrac{1}{r}
$$
So our Hamiltonian depends only on $r$ and $\hat{L}^{2}$. Knowing that $\hat{L}^{2}$ and $\hat{L}_{z}$ are independent of $r$, the Hamiltonian commutes with them both. They are also all compatible operators.

We look for solutions of the form 
$$
\psi(r,\theta,\phi)=R(r)Y(\theta,\phi)
$$
Using separation of variables, we find an angular equation 
$$
\hat{L}^{2}Y_{lm}(\theta,\phi)=2m_{e}\lambda Y_{lm}(\theta,\phi)
$$
where $Y_{lm}(\theta,\phi)$ are the spherical harmonics, and $\lambda=\hbar^{2}l(l+1)/2m_{e}$. It does not depend on $r$ and is the same for all spherically symmetric potentials.

Define a new function $\chi(r)=rR(r)$, such that the radial equation becomes 
$$
-\dfrac{\hbar^{2}}{2m_{e}}\dfrac{\textrm{d}^{2}\chi}{\textrm{d}r^{2}}+\underbrace{\left(\dfrac{\hbar^{2}}{2m_{e}}\dfrac{l(l+1)}{r^{2}}-\dfrac{Ze^{2}}{4\pi\epsilon_{0}}\dfrac{1}{r}\right)}_{=V_{\textrm{eff}}(r)}\chi=E\chi
$$
which is identical to the 1D TISE, with an effective potential $V_{\textrm{eff}}(r)$. The first term of $V_{\textrm{eff}}(r)$ is analogous to centrifugal (pseudo) force, and the second term is the Coulomb potential energy.

Using atomic units, $\hbar$, $m_{e}$, $e$, and $1/4\pi\epsilon_{0}$ are set to unity. As a result:

*   Length is measured in terms of Bohr radius 
$$
a_{0}=\dfrac{4\pi\epsilon_{0}\hbar^{2}}{m_{e}e^{2}}=5.29\times 10^{-11}\textrm{m}
$$
*   The unit of energy becomes the Hartree 
$$
E_{H}=\dfrac{\hbar^{2}}{m_{e}a_{0}^{2}}=4.36\times 10^{-18}\textrm{J}=27.21\,\textrm{eV}
$$
*   The radial equation becomes 
$$
-\dfrac{1}{2}\dfrac{\textrm{d}^{2}\chi}{\textrm{d}r^{2}}+\underbrace{\left(\dfrac{1}{2}\dfrac{l(l+1)}{r^{2}}-\dfrac{Z}{r}\right)}_{=V_{\textrm{eff}}(r)}\chi=E\chi
$$

Considering asymptotic ($e^{-\kappa r}$) and small $r$ ($r^{l+1}$) solutions, the general solution must be of the form 
$$
\chi(r)=F(r)e^{-\kappa r}
$$
where $F(r)$ is a power series solution with recurrence relation 
$$
\dfrac{c_{p}}{c_{p-1}}=\dfrac{2(\kappa(p+l)-Z)}{(p+l+1)(p+l)-l(l+1)}
$$
where $E=-\kappa^{2}/2$, where 
$$
E=-\dfrac{\kappa^{2}}{2}=-\dfrac{Z^{2}}{2(N+l)^{2}}
$$
for series to terminate at $N$th term. Define principle quantum number $n=N+l$ 
$$
E_{n}=-\dfrac{Z^{2}}{2n^{2}}\quad n=1,2,3,\dots\quad\textrm{(a.u.)}
$$
$N\geq 1$ and $l\geq 0$ gives 
$$
n\geq 1,\quad l\leq n-1
$$

So the stationary states of the hydrogenic atoms have quantum numbers $n$, $l$, and $m$, which specify the compatible operators $\hat{H}$, $\hat{L}^{2}$, and $\hat{L}_{z}$, respectively. 
$$
\begin{array}{l} n=1,2,3,\dots \\ l=0,1,2,\dots,(n-1) \\ m=-l,\dots,-1,0,1,\dots,l \\ \end{array}
$$

$$
E_{n}=-\dfrac{Z^{2}}{2n^{2}}E_{H}=-\dfrac{m_{e}Z^{2}e^{4}}{2(4\pi\epsilon_{0})^{2}\hbar^{2}}\dfrac{1}{n^{2}}\quad n=1,2,3,\dots
$$

In summary, the radial wavefunction can be found using 
$$
R(r)=\dfrac{\chi(r)}{r}=\dfrac{1}{r}F(r)e^{-\kappa r}
$$

$$
F(r)=\sum_{p=0}c_{p}r^{p+l+1}
$$

$$
\dfrac{c_{p}}{c_{p-1}}=\dfrac{2((Z/n)(p+l)-Z)}{(p+l+1)(p+l)-l(l+1)}
$$
where $\kappa=\sqrt{-2E}=Z/n$

Normalisation condition for radial wavefunction 
$$
\int_{0}^{\infty}|R_{nl}(r)|^{2}r^{2}\;\textrm{d}r=1
$$

Approximations: reduced mass, relativistic treatment, and spin have so far been neglected. Spin gives rise to Fine structure (interaction of orbital motion with its spin) and Hyperfine structure (interaction of electron spin and nucleus spin).

  

* * *

  

Section 9 : Electron spin and total angular momentum
----------------------------------------------------

### 9.1 Orbital Magnetic Momentum

![An electron in a circular orbit produces a current loop.](https://i.postimg.cc/3NwRt3zG/Screenshot-2022-12-13-121911.png "Semiclassical picture of an orbiting electron"){max-width: 400px, display: block, margin: 0 auto}

Using a semi-classical approach, an orbiting electron behaves like a current loop with 
$$
I_{\textrm{loop}}=\dfrac{-ev}{2\pi r}
$$
and magnetic moment 
$$
\mu=IA=\dfrac{-ev}{2\pi r}\times\pi r^{2}
$$

$$
\boldsymbol{\mu}=\dfrac{-\mu_{B}}{\hbar}\textbf{L}
$$
where $\mu_{B}=e\hbar/2m_{e}$ is the **Bohr magneton**.

A magnetic dipole moment in an external field $\textbf{B}$ possesses a magnetic potential energy 
$$
U_{\textrm{magnetic}}=-\boldsymbol{\mu}\cdot\textbf{B}
$$
So quantum magnetic interaction energy has operator 
$$
\hat{H}_{\textrm{magnetic}}=-\boldsymbol{\hat{\mu}}\cdot\textbf{B}=\dfrac{\mu_{B}}{\hbar}\boldsymbol{\hat{L}}\cdot\textbf{B}
$$
Suppose $\textbf{B}$ is only in $z$ direction 
$$
\textbf{B}=B_{z}\hat{\textbf{e}}_{z}
$$
Then the potential energy 
$$
\hat{H}_{\textrm{magnetic}}=\dfrac{\mu_{B}}{\hbar}B_{z}\hat{L}_{z}
$$
can be treated as a small perturbation to the hydrogenic atom Hamiltonian. 
$$
\begin{array}{l} \hat{H}\psi_{nlm} & =\biggl(\hat{H}^{(0)}+\underbrace{\dfrac{\mu_{B}}{\hbar}B_{z}\hat{L}_{z}}_{\textrm{Zeeman term}}\biggr)\psi_{nlm} \\ & =\underbrace{(E_{n}^{(0)}+m\mu_{B}B_{z})}_{\textrm{New energy eigenvalue}}\psi_{nlm} \\ \end{array}
$$
Remembering that $m$ takes integer values between $\pm l$, the magnetic field splits energy levels by 
$$
\Delta E=m\mu_{B}B_{z}
$$
The magnetic field-induced energy level splitting is known as the **Zeeman effect**. This phenomenon is why $m$ is called the magnetic quantum number.

  

### 9.2 The Stern-Gerlach experiment

![Beam of silver atoms within inhomogeneous magnetic field in z-direction.](https://i.postimg.cc/CMtmT7s3/Screenshot-2022-12-13-125521.png "The Stern-Gerlack experiment."){max-width: 400px, display: block, margin: 0 auto}


$$
F=-\dfrac{\partial V}{\partial z}=\mu_{z}\dfrac{\partial B}{\partial z}
$$
If magnetic field has a uniform gradient, the beam should be deflected in proportion to $\mu_{z}$. Classically, this can take any value and a continuous distibution is expected. Or, considering orbital angular momentum, we would expect quantisation according to allowed values of $m$, which are always odd. For a beam of s-state atoms, we would expect no deflection since $m=0$, but the Stern-Gerlach experiment gives two groups of atoms with magnetic moments 
$$
\mu_{z}=\pm\mu_{B}
$$
So there must be an additional, intrinsic source of angular momentum: spin.

  

### 9.3 Operators for spin

The intrinsic angular momentum, or spin $\textbf{S}$ is defined in analogy to $\textbf{L}$:

$\boldsymbol{\hat{L}}$ | $\boldsymbol{\hat{S}}$
------|--------
$l$ | $s$
$m_{l}=-l,\dots,l$ | $m_{s}=-s,\dots,s$
$\hat{L}^{2}Y_{lm_{l}}=l(l+1)\hbar^{2}Y_{lm_{l}}$ | $\hat{S}^{2}\chi_{sm_{s}}=s(s+1)\hbar^{2}\chi_{sm_{s}}$
$\hat{L}_{z}Y_{lm_{l}}=m_{l}\hbar Y_{lm_{l}}$ | $\hat{S}_{z}\chi_{sm_{s}}=m_{s}\hbar\chi_{sm_{s}}$
$\left[\hat{L}_{i},\hat{L}_{j}\right]=i\hbar\,\epsilon_{ijk}\hat{L}_{k}$ | $\left[\hat{S}_{i},\hat{S}_{j}\right]=i\hbar\,\epsilon_{ijk}\hat{S}_{k}$
$\left[\hat{L}^{2},\hat{L}_{i}\right]=0\quad i\in\{1,2,3\}$ | $\left[\hat{S}^{2},\hat{S}_{i}\right]=0\quad i\in\{1,2,3\}$


Note that $\chi_{sm_{s}}$ do not depend on electron coordinates; they represent a purely internal degree of freedom. $\chi_{\frac{1}{2}\frac{1}{2}}$ is spin up, and $\chi_{\frac{1}{2}-\frac{1}{2}}$ is spin down.

$s$ is spin quantum number; $s=1/2$ for an electron. $m_{s}=-s,\dots,s$ is magnetic spin quantum number.

The general formula for magnetic moment is 
$$
\boldsymbol{\mu}_{X}=g_{X}\dfrac{Q}{2M}\textbf{X}
$$
where $g_{X}$ is gyromagnetic factor. From this, spin g-factor $g_{s}=2$ for an electron can be derived, and the two allowed values $m_{s}=\pm1/2$.

The general interaction of the hydrogenic atom witha magnetic field must take into account both orbital and intrinsic angular momenta 
$$
\hat{H}=\hat{H}^{(0)}+\dfrac{\mu_{B}}{\hbar}\textbf{B}\cdot\left(\boldsymbol{\hat{L}}+2\boldsymbol{\hat{S}}\right)
$$
With eigenfunction 
$$
\psi_{n,l,m_{l},s,m_{s}}(r,\theta,\phi)=\underbrace{R_{n,l}(r)Y_{l,m_{l}}(\theta,\phi)}_{\textrm{continuous}}\overbrace{\chi_{s,m_{s}}}^{discrete}
$$
Note that $n,l,m_{l},s,m_{s}$ form a **complete set** of quantum numbers.

The eigenvalues of $(\hat{L}_{z}+2\hat{S}_{z})$ when applied to $\psi_{n,l,m_{l},s,m_{s}}$ in a constant magnetic field in $z$-direction are 
$$
(m_{l}+g_{s}m_{s})\hbar
$$

#### Total angular momentum
$$
\boldsymbol{\hat{J}}=\boldsymbol{\hat{L}}+\boldsymbol{\hat{S}}
$$
$$
|l-s|\leq j\leq |l+s|
$$
$$
m_{j}=-j,\dots,+j
$$
Values of $m_{j}$ differ by integer steps. For an electron, 
$$
j=\left|l-\dfrac{1}{2}\right|,l+\dfrac{1}{2}
$$