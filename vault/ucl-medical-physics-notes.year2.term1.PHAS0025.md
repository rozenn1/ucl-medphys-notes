---
id: yaliiiyfi9adlwhu56uyulz
title: PHAS0025
desc: ''
updated: 1679913085353
created: 1679912381687
---

Mathematical Methods III
============================================
_last updated on 24/01/2023_

* * *

### CONTENTS:

*   **1** Partial Differential Equations
    *   1.1 Terminology
    *   1.2 Separation of Variables Method
*   **2** Series Solutions to Differential Equations
    *   2.1 Series Solutions Flowchart
    *   2.2 Frobenius' Method
    *   2.3 Special Points and Fuchs' theorem
    *   2.4 Quantum Harmonic Oscillator
*   **3** Legendre Polynomials
    *   3.1 Laplace's equation in spherical polar coordinates
    *   3.2 The Generating Function
    *   3.3 Orthogonality and Normalisation
    *   3.4 Expansion of a function in terms of Legendre polynomials
    *   3.5 Spherical Harmonics
*   **4** Lagrangian and Hamiltonian Mechanics
    *   4.1 The Euler-Lagrange equation
    *   4.2 Lagrangian meachanics
    *   4.3 Hamiltonian mechanics
*   **5** Fourier Analysis
    *   5.1 Fourier Series
    *   5.2 Fourier Transforms
*   **6** Special Relativity
    *   6.1 The speed of light and Einstein's postulates
    *   6.2 The Lorentz transformation and four-vectors
    *   6.3 Consequences of the Lorentz transformation
    *   6.4 Mass, Energy, and Momentum
  

* * *

  

1 Partial Differential Equations
--------------------------------

### 1.1 Terminology

The **Order** of a differential equation is equal to the order of the highest-order derivative it contains.

A differential equation is **Linear** if the $y$ or $\dfrac{d^{n}y}{dx^{n}}$ terms are to the first power at most.

A linear differential equation is **Homogeneous** if every term contains a factor of $y$ or $\dfrac{d^{n}y}{dx^{n}}$.

The **Degree** of a differential equation is equal to the exponent (power) that the highest-order derivative is raised to. It can only take an integer value, and can be undefined if the highest-order derivative is within a function such as cosine.

**Solutions of a differential equation**  
There is a region $a\lt x\lt b$ for which a differential equation is defined. The solution $y(x)=u(x)$ satisfies the original differential equation by definition.

**Uniqueness**  
For an $n^{th}$ order differential equation, there are usually $n$ independent solutions. $n$ boundary conditions are required to determine unknown constants.

**Existence**  
There is no guarantee that a differential equation will have a solution of the form $y=u(x)$.

**Superposition principle**  
If $y_{1}(x)$ and $y_{2}(x)$ are solutions to a linear homogeneous differential equation, then $y=Cy_{1}(x)+Dy_{2}(x)$ is also a solution.

  

### 1.2 Separation of Variables Method

The aim is to transform a partial differential equation in $n$ variables into $n$ separate ordinary differential equations. Use the following procedure:

1.  Assume the solution can be written $u(x,y)=X(x)\cdot Y(y)$.
2.  Substitute into original differential equation and change partial derivatives into ordinary derivatives.
3.  Divide whole equation by $u(x,y)$.
4.  The resulting equation should be separable, provided that the factors in front of the derivatives can be expressed in terms of only one variable.
5.  We now have $f(x)=g(y)$. Since $x$ and $y$ are independent variables, each side of the equation can be equated to an arbitrary constant $c$.

This yields two ordinary differential equations which can be solved by considering different possible values of $c$. E.g.: Consider $c=0$, $c=-\lambda^{2}$, and $c=+\lambda^{2}$ for second order ordinary differential equations. Then apply boundary conditions for specific solution, or alternatively, sum over range of allowed solutions.

  

* * *

  

2 Series Solutions to Differential Equations
--------------------------------------------

### 2.1 Series Solutions Flowchart

Consider an ordinary differential equation in the form: 
$$
\dfrac{d^{2}y}{dx^{2}}+p(x)\dfrac{dy}{dx}+q(x)y=0\quad{at}\quad{x=x_{0}}
$$
Analytic means that the function can be written as a Taylor expansion at that point $x_{0}$, or that it tends to a finite constant within the limit $x\rightarrow x_{0}$. 
$$
p_{0}=\lim_{x\rightarrow{x_{0}}}{x\,p(x)}\qquad{and}\qquad{q_{0}}=\lim_{x\rightarrow{x_{0}}}{x^{2}\,q(x)}
$$
Use the flowchart below to determine the nature of the point $x_{0}$ and the method that should be used to solve the differential equation.

![Flowchart. Start. Are both p(x) AND q(x) analytic at x0? If yes, x0 is an ordinary point, so use power series solutions method. If no, go to next question. Are both p0 and q0 analytic at x0? If yes, x0 is a regular singular point, so Frobenius Method should be used. If no, x0 is an essential singular point. End.](https://i.postimg.cc/TPFy1ShZ/Screenshot-2022-11-02-202045.jpg "Flowchart for deciding which method of series solution to use for a point x0"){max-width: 500px, display: block, margin: 0 auto}

For power series solution method, use the assumed solution: 
$$
y=\sum_{n=0}^{\infty}a_{n}x^{n}
$$

  

### 2.2 Frobenius' Method

For a general second order linear homogeneous differential equation of the form 
$$
\dfrac{d^{2}y}{dx^{2}}+p(x)\dfrac{dy}{dx}+q(x)y=0
$$

1.  Choose a regular singular point $x_{0}$ where the series solution will be centered.
2.  Assume a solution of the form: 
$$
y(x)=\sum_{j=0}^{\infty}{a_{j}(x-x_{0})^{k+j}}\quad{where}\quad{a_{0}\neq{0}}
$$
3.  Derive **indicial equation** for the parameter $k$: 
$$
k(k-1)+p_{0}k+q_{0}=0
$$
Note that if the possible values of $k$ differ by an integer (or if they are a repeated solution) only one independent solution of the assumed form is guaranteed, and it is given by the largest $k$.
4.  Insert the assumed expression for $y(x)$ and its differentials into ordinary differential equation.
5.  For each value of $k$, derive a condition for successive $a_{j}$ called the **recurrence relation**. Use dummy variable change in summations if needed, remembering that different powers of $x$ are linearly independent. In some cases, a series solution may terminate after a certain $j$ value.

  

### 2.3 Special Points and Fuchs' theorem

Use the flowchart from 2.1 to determine the nature of a point $x_{0}$.

**Fuchs' Theorem**  
Given a linear, homogeneous differential equation of the second order, at least one series solution exists if the expansion point is an ordinary or regular singular point (NOT an essential singular point).

**Wronskian test**  
Given two solutions $y_{1}(x)$ and $y_{2}(x)$, they are linearly independent if and only if: 
$$
\left|\begin{array}{l} y_{1} & y_{2}\\ y_{1}' & y_{2}'\\ \end{array}\right|\neq0
$$

**D'Alembert ratio test**  
To test convergence of a series, consider two successive terms $u_{k}$ and $u_{k+1}$ 
$$
\rho=\lim_{k\rightarrow{\infty}}{\left|{\dfrac{u_{k+1}}{u_{k}}}\right|}\lt{1}\qquad{for\;convergence}
$$
Use this to find a radius of convergence $-a\lt{x}\lt{a}$.

  

### 2.4 Quantum Harmonic Oscillator

The solution of the quantum harmonic oscillator can be separated into a polynomial and an asymptotic part as follows 
$$
\psi(y)=H(y)\exp{\left(-\dfrac{y^{2}}{2}\right)}
$$
where the solutions for $H(y)$ are given by the **Hermite polynomials**.  
(Normalisation condition: highest power term in $a_{j}=2^{j}$) 
$$
H_{0}(y)=1
$$

$$
H_{1}(y)=2y
$$

$$
H_{2}(y)=4y^{2}-2
$$

$$
H_{3}(y)=8y^{3}-12y
$$

$$
\vdots
$$

  

* * *

  

3 Legendre Polynomials
----------------------

### 3.1 Laplace's equation in spherical polar coordinates


$$
\textrm{Laplace's Equation:}\quad\nabla^{2}V=0
$$

$$
\dfrac{1}{r^{2}}\dfrac{\partial}{\partial{r}}\left({r^{2}\dfrac{\partial{V}}{\partial{r}}}\right)+\dfrac{1}{r^{2}\sin{\theta}}\dfrac{\partial}{\partial{\theta}}\left({\sin{\theta}\dfrac{\partial{V}}{\partial{\theta}}}\right)+\dfrac{1}{r^{2}\sin^{2}{\theta}}\dfrac{\partial^{2}V}{\partial{\phi}^{2}}=0
$$
Using partial differential equations separation of variables method: 
$$
V(r,\theta,\phi)=R(r)\Theta(\theta)\Phi(\phi)
$$

$$
\Phi(\phi)=Ae^{\mp{im}\phi},\quad{R(r)}=Ar^{l}+\dfrac{B}{r^{l+1}}
$$
Angular part of Laplace equation leads to **Legendre equation**: 
$$
\dfrac{d}{d\mu}\left({(1-\mu^{2})\dfrac{d\theta}{d\mu}}\right)+\left({l(l+1)-\dfrac{m^{2}}{1-\mu^{2}}}\right)\Theta=0\qquad\mu=\cos{\theta}
$$
Rearrange with $x=\cos{\theta}\:$ and $\:\Theta\Rightarrow{y(x)}\:$ with $m=0\:$ (cylindrical symmetry): 
$$
y''-\dfrac{2x}{1-x^{2}}y'+\dfrac{\lambda}{1-x^{2}}=0
$$
Series solution results in the **Legendre polynomials**:

![The Legendre polynomials for n=0,1,2,3,4. Note that every curve coincides at point (1,1). Graph.](https://www.researchgate.net/profile/Benaoumeur-Bakhti/publication/345642097/figure/fig5/AS:956076245655552@1604957748168/Polynomes-de-Legendre-pour-n-0-1-2-3-4.png "Graph of first few normalised Legendre polynomials"){max-width: 400px, display: block, margin: 0 auto}


$$
P_{0}(x)=1
$$

$$
P_{1}(x)=x
$$

$$
P_{2}(x)=\dfrac{1}{2}(3x^{2}-1)
$$

$$
P_{3}(x)=\dfrac{1}{2}(5x^{3}-3x)
$$

$$
\vdots
$$

The series solution converges for $|x|\lt1$, i.e. $0°\lt\theta\lt{180°}$. Series terminates when $n=l$. Notice that Legendre polynomials are normalised such that $P_{n}(x=1)=1$. 
$$
\therefore{V(r,\theta,\phi)}=\sum_{l=0}^{\infty}\sum_{m=-l}^{+l}\left({C_{l}r^l+\dfrac{D_{l}}{r^{l+1}}}\right)P_{l}(\cos{\theta})A_{m}e^{-im\phi}
$$

  

### 3.2 The Generating Function

The function $g(t,\mu)$ is the **Generating function** of Legendre polynomials. 
$$
g(t,\mu)=\dfrac{1}{\sqrt{1+t^{2}-2t\mu}}=\sum_{l=0}^{\infty}t^{l}\:P_{l}(\mu)
$$

**Multipole expansion**  
An "$(l+1)$-pole" can be found, using the corresponding $l$ term of the charge distribution from which the field originates. 
$$
V(r,\theta)=\sum_{l=0}^{\infty}\dfrac{D_{l}}{r^{l+1}}P_{l}(\cos{\theta})
$$

  

### 3.3 Orthogonality and Normalisation

Different Legendre polynomials are orthogonal to one another, and obey the following orthonormality condition: 
$$
\int_{-1}^{1}P_{l}(x)P_{n}(x)\:{dx}=\dfrac{2}{2l+1}\delta_{ln}
$$

$$
\delta_{ln}=\left\{\begin{array}{l} 1\quad{for\;l=n}\\ 0\quad{for\;l\neq{n}}\\ \end{array}\right.
$$

### 3.4 Expansion of a function in terms of Legendre polynomials

Any reasonable, continuous function in range $|x|\lt{1}$ can be expanded in terms of Legendre polynomials as follows: 
$$
f(x)=\sum_{l=0}^{\infty}c_{l}P_{l}(x)
$$

$$
c_{m}=\dfrac{2m+1}{2}\int_{-1}^{1}f(x)\,P_{m}(x)\:dx
$$
Legendre expansions may be better approximations than Taylor expansions at different values of $x_{0}$.

### 3.5 Spherical Harmonics

Well-behaved, physical solutions of Legendre's equation are possible for $l$ being a non-negative integer, and $m$ being in the range $-l\lt{m}\lt{l}$. For $m\gt{0}$, the **associated Legendre polynomials** can be derived using: 
$$
P_{l}^{m}(x)=(1-x^{2})^{m/2}\dfrac{d^{m}}{dx^{m}}P_{l}(x)
$$

$$
\int_{-1}^{1}P_{l}^{m}(x)P_{n}^{m}(x)\:dx=\dfrac{2}{2l+1}\dfrac{(l+m)!}{(l-m)!}\:\delta_{ln}
$$
And for $m\lt{0}$: 
$$
P_{n}^{-m}(x)=(-1)^{m}\dfrac{(n-m)!}{(n+m)!}P_{n}^{m}(x)
$$
Orthogonality for different $m$: 
$$
\int_{-1}^{1}P_{n}^{m}(x)P_{n}^{k}(x)\dfrac{dx}{1-x^{2}}=\dfrac{(n+m)!}{m(n-m)!}\,\delta_{mk}
$$
In Quantum mechanics, we write **spherical harmonics**: 
$$
Y_{l}^{m}(\theta,\phi)=c_{l,m}\,P_{l}^{m}(\cos{\theta})\,e^{im\phi}
$$

$$
\int_{-1}^{1}d(\cos{\theta})\int_{0}^{2\pi}d\phi\;{Y_{l}^{m}}^{*}\;{Y_{l'}^{m'}}=\delta_{ll'}-\delta_{mm'}
$$
where 
$$
c_{l,m}=(-1)^{m}\sqrt{\dfrac{(l-m)!\,(2l+1)}{4\pi(l+m)!}}
$$

  

* * *

  

4 Lagrangian and Hamiltonian mechanics
--------------------------------------

### 4.1 The Euler-Lagrange equation

Consider the integral 
$$
J=\int_{x_{1}}^{x_{2}}{f(y,y',x)}\;dx
$$
We choose a path through $x_{1}$ and $x_{2}$ which minimises the integral $J$, using the **Euler-Lagrange equation** 
$$
\dfrac{\partial f}{\partial y}-\dfrac{\textrm{d}}{\textrm{d}x}\dfrac{\partial f}{\partial y'}=0
$$
When the function contains no $y$ dependence, then $\dfrac{\partial f}{\partial y}=0$, so $\dfrac{\partial f}{\partial y'}=\textrm{constant}$

Another form is 
$$
\dfrac{\partial f}{\partial x}-\dfrac{\textrm{d}}{\textrm{d} x}\left({f-y'\dfrac{\partial f}{\partial y'}}\right)=0
$$
and if $f=f(y,y')$, with no explicit $x$ dependence, 
$$
\dfrac{\textrm{d}}{\textrm{d} x}\left({f-y'\dfrac{\partial f}{\partial y'}}\right)=0\quad\textrm{or}\quad{f-y'\dfrac{\partial f}{\partial y'}=\textrm{constant}}
$$

  

### 4.2 Lagrangian mechanics

Several dependent variables, $y_{n}(x)$, give a set of Euler-Lagrange equations for each dependent variables. 
$$
\dfrac{\partial f}{\partial y_{i}}-\dfrac{\textrm{d}}{\textrm{d} x}\left({\dfrac{\partial f}{\partial y_{i}'}}\right)=0,\quad{i=1,2,...,n}
$$
For several independent variables $x_{n}$, the Euler-Lagrange equation is 
$$
\dfrac{\partial f}{\partial y}-\sum_{i=1}^{n}{\dfrac{\partial}{\partial x_{i}}\left({\dfrac{\partial f}{\partial y_{x_{i}}}}\right)}=0\quad\textrm{where } y_{x_{i}}=\dfrac{\partial y}{\partial x_{i}}
$$
This can be expanded for multiple dependent and independent variables.

#### The Lagrangian

The Lagrangian $L$ is defined as the difference between the kinetic and potential energies. 
$$
L(x,\dot{x},t)=T(x,\dot{x},t)-V(x,t)
$$
Applying the Euler-Lagrange equation, we obtain **Lagrange's equations of motion**. 
$$
\dfrac{\textrm{d}}{\textrm{d} t}\left({\dfrac{\partial L}{\partial\dot{x_{i}}}}\right)-\dfrac{\partial L}{\partial x_{i}}=0
$$

  

### 4.3 Hamiltonian mechanics

The Hamiltonian formulation of meachanics describes systems in terms of generalised coordinates $q_{i}$ and generalised momenta $p_{i}$. We define the general momentum as 
$$
p_{i}=\dfrac{\partial L}{\partial\dot{q_{i}}};\quad\dot{p_{i}}=\dfrac{\partial L}{\partial q_{i}}
$$
From which we can derive the definition of the Hamiltonian 
$$
H=\sum_{i}p_{i}\dot{q_{i}}-L
$$
The **Hamilton equations of motion** are 
$$
-\dot{p_{i}}=\dfrac{\partial H}{\partial q_{i}}\quad\textrm{and}\quad\dot{q_{i}}=\dfrac{\partial H}{\partial p_{i}}
$$
and 
$$
\dfrac{\partial H}{\partial t}=-\dfrac{\partial L}{\partial t}
$$
We can also write the Hamiltonian in terms of kinetic and potential energy 
$$
H=T+V,\quad\textrm{where}\quad T=\dfrac{1}{2}\sum_{i}p_{i}\dot{q_{i}}
$$

  

* * *

  

5 Fourier Analysis
------------------

### 5.1 Fourier Series

Fourier analysis is the decomposition of complex signals into a sum of sine and cosine waves of different frequencies. For a signal of period $2L$, the Fourier series can be defined 
$$
f(x)=\dfrac{a_{0}}{2}+\sum_{n=1}^{\infty}\left[a_{n}\cos\left(\dfrac{n\pi}{L}x\right)+b_{n}\sin\left(\dfrac{n\pi}{L}x\right)\right]
$$
where 
$$
a_{n}=\dfrac{1}{L}\int_{-L}^{L}\cos\left(\dfrac{n\pi}{L}x\right)f(x)\:\textrm{d}x
$$

$$
b_{n}=\dfrac{1}{L}\int_{-L}^{L}\sin\left(\dfrac{n\pi}{L}x\right)f(x)\:\textrm{d}x
$$

In this system, the scalar product is defined 
$$
f(x)\cdot g(x):=\int_{-L}^{L}f(x)g(x)\:\textrm{d}x
$$
such that the sine and cosine form an **orthonormal basis** which can be used to express any periodic function as a Fourier series. The orthonormality relations are 
$$
\sin\left(\dfrac{m\pi}{L}x\right)\cdot\sin\left(\dfrac{n\pi}{L}x\right)=\left\{\begin{array}{l}L\delta_{mn}&\textrm{for}\:\max(m,n)\gt 0\\0&\textrm{for}\;m=n=0\end{array}\right.
$$

$$
\cos\left(\dfrac{m\pi}{L}x\right)\cdot\cos\left(\dfrac{n\pi}{L}x\right)=\left\{\begin{array}{l}L\delta_{mn}&\textrm{for}\:\max(m,n)\gt 0\\2L&\textrm{for}\;m=n=0\end{array}\right.
$$

$$
\sin\left(\dfrac{m\pi}{L}x\right)\cdot\cos\left(\dfrac{n\pi}{L}x\right)=0
$$

Use trignomometric identities 
$$
\sin\alpha\cos\beta=\dfrac{1}{2}\left[\sin\left(\alpha-\beta\right)+\sin\left(\alpha+\beta\right)\right]
$$

$$
\sin\alpha\sin\beta=\dfrac{1}{2}\left[\cos\left(\alpha-\beta\right)-\cos\left(\alpha+\beta\right)\right]
$$

$$
\cos\alpha\cos\beta=\dfrac{1}{2}\left[\cos\left(\alpha-\beta\right)+\cos\left(\alpha+\beta\right)\right]
$$

  

Note that

*   Even functions $f(x)=f(-x)$ can be expressed solely in $\cos$ terms
*   Odd functions $f(x)=-f(-x)$ can be expressed solely in $\sin$ terms

  

#### Parseval's Identity


$$
\dfrac{1}{2L}\int_{-L}^{L}\left[f(x)\right]^{2}\:\textrm{d}x=\left(\dfrac{a_{0}}{2}\right)^{2}+\dfrac{1}{2}\sum_{n=1}^{\infty}\left(a_{n}^{2}+b_{n}^{2}\right)
$$

  

#### Complex Fourier series

Considering Euler's formula, any complex function can be expressed as a complex Fourier series 
$$
f(x)=\sum_{n=-\infty}^{+\infty}c_{n}e^{i\frac{n\pi}{L}x}
$$

$$
c_{n}=\dfrac{1}{2L}\int_{-L}^{L}e^{-i\frac{n\pi}{L}x}f(x)\:\textrm{d}x
$$

The scalar product is now the "Hilbert-Schmidt" scalar product 
$$
f(x)\cdot g(x):=\int_{-L}^{L}f^{*}(x)g(x)\:\textrm{d}x
$$
where the new orthonormality relations take the form 
$$
e^{i\frac{m\pi}{L}x}\cdot e^{i\frac{n\pi}{L}x}=2L\delta_{mn}
$$

Parseval's identity is expressed as 
$$
\dfrac{1}{2L}\int_{-L}^{L}|f(x)|^{2}\:\textrm{d}x=\sum_{n=-\infty}^{+\infty}|c_{n}|^{2}
$$

  

### 5.2 Fourier Transforms

Consider a non-periodic function. It can be expressed as a Fourier series with infinite period. 
$$
f(x)=\dfrac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}e^{ikx}\tilde{f}(k)\:\textrm{d}k
$$

$$
\tilde{f}(k)=\dfrac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}e^{-ikx}f(x)\:\textrm{d}x
$$
where $k=n\pi/L$ and $\tilde{f}(k)$ is the **Fourier Transform** of $f(x)$.

*   $f(x)$ is odd $\rightarrow$ only $\sin$ terms.
*   $f(x)$ is even $\rightarrow$ only $\cos$ terms.


$$
\textrm{FT}[f'(x)]=ik\textrm{FT}[f(x)]=ik\tilde{f}(k)
$$

$$
\textrm{FT}[f(x+a)]=e^{ika}\textrm{FT}[f(x)]=e^{ika}\tilde{f}(k)
$$

  

#### The Dirac Delta function

It "filters out" the one value of $f(y)$ at $x$. 
$$
f(x)=\dfrac{1}{2\pi}\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}e^{ik(x-y)}f(y)\:\textrm{d}y\,\textrm{d}k
$$

$$
f(x)=\int_{-\infty}^{\infty}\delta(x-y)f(y)\:\textrm{d}y
$$
where 
$$
\delta(x-y):=\dfrac{1}{2\pi}\int_{-\infty}^{\infty}e^{ik(x-y)}\:\textrm{d}k
$$

  

#### Parseval's identity for Fourier Transforms


$$
\int_{-\infty}^{\infty}|f(x)|^{2}\:\textrm{d}x=\int_{-\infty}^{\infty}|\tilde{f}(k)|^{2}\:\textrm{d}k
$$

  

#### Convolution Theorem

For a physical quantity $f(x)$, measured using apparatus with resolution function $g(y)$, the convolution $h(z)$ is 
$$
h(z)=\dfrac{1}{\sqrt{2\pi}}\int_{-\infty}^{\infty}f(x)g(z-x)\:\textrm{d}x
$$
which is written formally as $h=f*g$. For an ideal instrument, $g(z-x)=\sqrt{2\pi}\delta(z-x)$.

Convolution theorem states that 
$$
\textrm{FT}[h]=\textrm{FT}[f]\times\textrm{FT}[g]
$$

  

* * *

  

6 Special Relativity
--------------------

### 6.1 The speed of light and Einstein's postulates

Before Einstein, Newton assumed that time flowed uniformly on, without regard to external factors.

We know that for waves travelling in a medium, wind to or away from the observer changes the received wavelength of the sound 
$$
n=\dfrac{d}{\lambda}=\dfrac{fd}{v_{0}\pm u}
$$
where $n$ is number of wavelengths in a distance $d$.

If light travelled in a medium, _'lumineferous aether'_, then its wavelength and speed should change like sound waves do.

  

#### The Michelson-Morley experiment

The Michelson-Morley experiment was designed to detect the effect of the 'aether wind' due to the Earth's orbit around the Sun.

![Laser from source hits beamsplitter at 45 degree angle. Each split beam is normal to a mirror, both at distance L. A detector analyses the interference pattern caused by both reflected and transmitted beams. Schematic.](/assets/images/2023-03-27-11-30-31.png){max-width: 400px, display: block, margin: 0 auto}

The 'aether wind' should cause the intergference fringes to shift when the apparatus is rotated, but **no effect has ever been detected**.

  

#### Inertial systems

Newton's first law can be stated in the form

> There are obsevers for whom all isolated bodies move with a uniform velocity.

Such observers are called **inertial observers**.

Here is the definition of an inertial coordinate system:

> An inertial coordinate system is a system of coordinates such that all isolated bodies move with uniform velocity in the coordinate system.

  

#### Einstein's postulates

Einstein postulated that the aether does not exist. This ensures that Maxwell's equations are equally valid for all observers, and that they all observe the same velocity of light.

Einstein's postulates are:

> The laws of physics have the same form in all inertial systems.

> The velocity of light in empty space is a universal constant, the same for all observers.

  

#### The relativity of simultaneity

Einstein's postulates completely destroy Newton's idea of absolute time. Events simultaneous in one frame, may not be simultaneous in another.

  

### 6.2 The Lorentz transformation and four-vectors

#### Events and Transformations

An event can be specified by its position and its time $(t,x,y,z)$. The same event can be observed in another frame $S'$: $(t',x',y',z')$. The relation between the two is given by a linear transformation.

  

#### The Galilean Transformation

Consider a frame $S'$ moving with velocity $v$ relative to $S$ along the $z$ direction. The systems are set so that at $t=t'=0$, the origins of the frames coincide.

The relation between both frames can be expressed as: 
$$
\left(\begin{array}{c} t' \\ x' \\ y' \\ z' \\ \end{array}\right)=\left(\begin{array}{c} 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ -v & 0 & 0 & 1 \\ \end{array}\right)\left(\begin{array}{c} t \\ x \\ y \\ z \\ \end{array}\right)
$$
It is not relativistic, and cannot be correct according to Einstein's postulates.

  

#### The Lorentz Transformation

Knowing Einstein's postulates, a linear transform respecting the symmetry of space can be derived - the Lorentz transform. 
$$
\left(\begin{array}{c} ct' \\ x' \\ y' \\ z' \\ \end{array}\right)=\left(\begin{array}{c} \gamma & 0 & 0 & -\gamma\beta \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ -\gamma\beta & 0 & 0 & \gamma \\ \end{array}\right)\left(\begin{array}{c} ct \\ x \\ y \\ z \\ \end{array}\right)
$$

$$
\gamma=\dfrac{1}{\sqrt{1-\beta^{2}}}\qquad\beta=\dfrac{v}{c}
$$

  

#### Four-vectors

> Four-vectors are objects which transform via the Lorentz matrices when boosted between inertial frames.

Four-vectors are introduced to keep the Lorentz matrix dimensionless. The scalar product of two four-vectors is 
$$
V\cdot W=V^{T}GW
$$
where $G$ is the metric of space-time, 
$$
G=\left(\begin{array}{c} 1 & 0 & 0 & 0 \\ 0 & -1 & 0 & 0 \\ 0 & 0 & -1 & 0 \\ 0 & 0 & 0 & -1 \\ \end{array}\right)
$$

  

### 6.3 Consequences of the Lorentz transformation

#### Length contraction

If a stick of rest length $L_{0}$ is observed moving with velocity $v$, it will contract in direction of movement 
$$
L=L_{0}\sqrt{1-\beta^{2}}
$$
For stick of orientation $\theta_{0}$ to direction of motion, stick is both contracted and rotated. 
$$
L=L_{0}\sqrt{1-\beta^{2}\cos^{2}\theta_{0}}
$$

$$
\theta=\tan^{-1}(\gamma\tan\theta_{0})
$$

  

#### Time dilation

An observer measure a longer time $\Delta t$ compared to time in the moving object's rest frame $\Delta t'$. 
$$
\Delta t=\gamma\Delta t'
$$
Use inverse Lorentz transformation to derive time dilation.

  

#### The relativity of simultaneity

The interval between two events $q$ is also a four-vector. The squared magnitude is 
$$
q^{2}=c^{2}\Delta t^{2}-\Delta x^{2}-\Delta y^{2}-\Delta z^{2}
$$
$q^{2}$ is called the spacetime interval. It is an invariant; the same in all inertial frames.

*   Time-like $q^{2}\gt0$ : A can cause B, there exists a frame where A happens before B at the same point in space. The events always occur in the same time-order in every inertial frame.
*   Light-like $q^{2}=0$ : Causation can only occur at speed of light.
*   Space-like $q^{2}\lt0$ : No causal relation possible. There exists a frame where events are simultaneous, but at different locations.

  

#### Addition of velocities

A frame $S'$ moves with velocity $v$ in $z$ direction compared to $S$. 
$$
u_{x}=\dfrac{1}{\gamma}\cdot\dfrac{u'_{x}}{1+u'_{z}v/c^{2}}
$$

$$
u_{y}=\dfrac{1}{\gamma}\cdot\dfrac{u'_{y}}{1+u'_{z}v/c^{2}}
$$

$$
u_{z}=\dfrac{u'_{z}+v}{1+u'_{z}v/c^{2}}
$$
For example, we want to find speed $\textbf{u}$ of a projectile relative to Earth $S$, knowing velocity of the projectile relative to a spaceship $S'$.

  

#### Relativistic Doppler effect

An emitter recedes with velocity $v$ directly away from an observer. 
$$
f=f_{0}\sqrt{\dfrac{1-v/c}{1+v/c}}
$$

$$
\lambda=\lambda_{0}\sqrt{\dfrac{1+v/c}{1-v/c}}
$$
If the source is moving perpendicularly to observer, there is still a shift due to time dilation. 
$$
f=f_{0}/\gamma
$$

  

### 6.4 Mass, Energy, and Momentum

Relativistic momentum is 
$$
\textbf{p}=\gamma m\textbf{u}
$$
Relativistic kinetic energy is 
$$
K=\gamma mc^{2}-mc^{2}
$$
Einstein proposed that total energy in a body is 
$$
E=\gamma mc^{2}
$$
which contains a "rest energy" even when stationary 
$$
E_{\textrm{rest}}=mc^{2}
$$
This energy exists due to an object's mass.

  

#### Energy in terms of momentum


$$
E=\sqrt{m^{2}c^{4}+\textbf{p}^{2}c^{2}}
$$
This leads to four-momentum 
$$
p=\left(\begin{array}{c} E/c \\ p_{x} \\ p_{y} \\ p_{z} \\ \end{array}\right)
$$
with $m^{2}c^{2}$ as the invariant 'length'. Four-momentum is boosted via the Lorentz transformation. Four-momentum is conserved component-by-component.

Four-momentum of a photon is 
$$
\left(\begin{array}{c} E/c \\ p_{x} \\ p_{y} \\ p_{z} \\ \end{array}\right)=\left(\begin{array}{c} h/\lambda \\ 0 \\ 0 \\ h/\lambda \\ \end{array}\right)
$$
