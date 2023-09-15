# Numerical Methods Calculator

A calculator which implements various numerical methods and includes support for many special functions.
___
## About The Project

Numerical methods, also referred to as numerical analysis, is a branch of mathematical analysis which studies methods of approximating solutions, and deriving error bounds, to problems which are either too difficult or even impossible to solve exactly. It has applications to many disciplines in STEM and business including, but not limited to computational physics, computational chemistry, engineering, computational finance, and actuarial science.

Much of mathematics is based on the idea of functions. This project implements support for many of the functions taught in grade school including polynomials, exponentials, logarithms, trigonometric, and hyperbolic functions. Also included is support for many of the special functions used in more specialized areas of mathematics including mathematical physics, probability, real analysis, complex analysis, analytic number theory, ordinary differential equations, and partial differential equations. The gamma function, error function, and Bessel functions are just a few of the special functions which are supported.

See [Instructions](#Instructions) for more information regarding the functions and numerical algorithms that are implemented.
___
## Installation

This project runs in Jupyter Notebook. To use Jupyter Notebook it is necessary to download and install [Anaconda](https://www.anaconda.com/download). Once installed, Jupyter Notebook can be accessed through the Anaconda Navigator.

To run the code, the following packages must be installed:
- math
- mpmath
- numpy
- tkinter
- ttk

These packages can be installed by opening a new terminal in Jupyter Notebook and using the following command:

```pip install [Insert package name here.]```

Where the brackets should be replaced with the package name. For example, to install mpmath enter the command:

```pip install mpmath```

___
## Instructions

### Supported Constants and Functions

#### Constants

| Mathematical Constant | Mathematical Notation | Implementation | Python Function |
| --- | --- | --- | --- |
| Pi | &pi; | | math.pi |
| Euler's Number | e | | |
| Golden Ratio | &phi; | | mpmath.phi |
| Euler-Mascheroni Constant | &gamma; | | mpmath.euler |
| Glaisher-kinkelin Constant | A | | mpmath.glaisher |
| Catalan's Constant | G | | |
| Infinity | $\infty$ | | math.inf |

#### Functions

| Mathematical Function | Mathematical Notation | Implementation | Python Function |
| --- | --- | --- | --- |
| Absolute Value | &#124; x &#124; | &#124; x &#124; | math.fabs(x) |
| Exponential | e<sup>x</sup> | e^(x) | math.exp(x) |
| Natural Logarith | lnx | ln(x) | math.log(x) |
| Common Logarithm | logx | log(x) | math.log(x,10) |
| General Logarithm | log<sub>a</sub>x | log(x,a) | math.log(x,a) |
| Square Root | $\sqrt{x}$ | sqrt(x) | math.sqrt(x) |
| Cube Root | $\sqrt[3]{x}$ | cbrt(x) | mpmath.cbrt(x) |
| N-th Root | $\sqrt[n]{x}$ | root(x,n) | mpmath.root(x,n) |
| Lambert W Function | W(x) | W(x) | mpmath.lambertw(x) |
| Sine | sinx | sin(x) | math.sin(x) |
| Inverse Sine | arcsinx | arcsin(x) | math.asin(x) |
| Hyperbolic Sine | sinhx | sinh(x) | math.sinh(x) |
| Inverse Hyperbolic Sine | arsinhx | arsinh(x) | math.asinh(x) |
| Cosine | cosx | cos(x) | math.cos(x) |
| Inverse Cosine | arccosx | arccos(x) | math.acos(x) |
| Hyperbolic Cosine | coshx | cosh(x) | math.cosh(x) |
| Inverse Hyperbolic Cosine | arcoshx | arcosh(x) | math.acosh(x) |
| Tangent | tanx | tan(x) | math.tan(x) |
| Inverse Tangent | arctanx | arctan(x) | math.atan(x) |
| Hyperbolic Tangent | tanhx | tanh(x) | math.tanh(x) |
| Inverse Hyperbolic Tangent | artanhx | artanh(x) | math.atanh(x) |
| Secant | secx | sec(x) | mpmath.sec(x) |
| Inverse Secant | arcsecx | arcsec(x) | mpmath.asec(x) |
| Hyperbolic Secant | sechx | sech(x) | mpmath.sech(x) |
| Inverse Hyperbolic Secant | arsechx | arsech(x) | mpmath.asech(x) |
| Cosecant | cscx | csc(x) | mpmath.csc(x) |
| Inverse Cosecant | arccscx | arccsc(x) | mpmath.acsc(x) |
| Hyperbolic Cosecant | cschx | csch(x) | mpmath.csch(x) |
| Inverse Hyperbolic Cosecant | arcschx | arcsch(x) | mpmath.acsch(x) |
| Cotangent | cotx | cot(x) | mpmath.cot(x) |
| Inverse Cotangent | arccotx | arccot(x) | mpmath.acot(x) |
| Hyperbolic Cotangent | cothx | coth(x) | mpmath.coth(x) |
| Inverse Hyperbolic Cotangent | arcothx | arcoth(x) | mpmath.acoth(x) |
| Gamma Function | &Gamma;(x) | Gamma(x) | math.gamma(x) |
| Generalized Incomplete Gamma Function | &Gamma;(x,a,b) | Gamma(x,a,b) | mpmath.gammainc(x,a,b) |
| Digamma Function | &psi;(x) | psi(x) | mpmath.digamma(x) |
| Polygamma Function | &psi;<sub>n</sub>(x) | psi(n,x) | mpmath.psi(n,x) |
| Barnes G Function | G(x) | G(x) | mpmath.barnesg(x) |
| Exponential Integral Function | Ei(x) | Ei(x) | mpmath.ei(x) |
| Generalized Exponential Integral Function | E<sub>n</sub>(x) | En(n,x) | mpmath.expint(n,x) |
| Logarithmic Integral Function | li(x) | li(x) | mpmath.li(x) |
| Cosine Integral Function | Ci(x) | Ci(x) | mpmath.ci(x) |
| Hyperbolic Cosine Integral Function | Chi(x) | Chi(x) | mpmath.chi(x) |
| Sine Integral Function | Si(x) | Si(x) | mpmath.si(x) |
| Hyperbolic Sine Integral Function | Shi(x) | Shi(x) | mpmath.shi(x) |
| Error Function | erf(x) | erf(x) | math.erf(x) |
| Complementary Error Function | erfc(x) | erfc(x) | math.erfc(x) |
| Imaginary Error Function | erfi(x) | erfi(x) | mpmath.erfi(x) |
| Fresnel Sine Integral Function | S(x) | S(x) | mpmath.fresnels(x) |
| Fresnel Cosine Integral Function | C(x) | C(x) | mpmath.fresnelc(x) |
| Bessel Function of the First Kind | J<sub>n</sub>(x) | J(n,x) | mpmath.besselj(n,x) |
| Bessel Function of the Second Kind | Y<sub>n</sub>(x) | Y(n,x) | mpmath.bessely(n,x) |
| Modified Bessel Function of the First Kind | I<sub>n</sub>(x) | I(n,x) | mpmath.besseli(n,x) |
| Modified Bessel Function of the Second Kind | K<sub>n</sub>(x) | K(n,x) | mpmath.besselk(n,x) |
| Struve Function | H<sub>n</sub>(x) | H(n,x) | mpmath.struveh(n,x) |
| Modified Struve Function | L<sub>n</sub>(x) | L(n,x) | mpmath.struvel(n,x) |
| Weber Function | E<sub>&nu;</sub>(x) | E(&nu;,x) | mpmath.webere(&nu;,x)
| Lommel Function | s<sub>&mu;,&nu;</sub>(x) | s(&mu;,&nu;,x) | mpmath.lommels1(&mu;,&nu;,x)
| Airy Ai Function | Ai(x) | Ai(x) | mpmath.airyai(x) |
| Airy Bi Function | Bi(x) | Bi(x) | mpmath.airybi(x) |
| Scorer Gi Function | Gi(x) | Gi(x) | mpmath.scorergi(x) |
| Scorer Hi Function | Hi(x) | Hi(x) | mpmath.scorerhi(x) |
| Generalized Hypergeometric Function | <sub>p</sub>F<sub>q</sub>(a<sub>1</sub>,...,a<sub>p</sub>;b<sub>1</sub>,...,b<sub>q</sub>;x) | pFq([a<sub>1</sub>,...,a<sub>p</sub>],[b<sub>1</sub>,...,b<sub>q</sub>],x) | mpmath.hyper([a<sub>1</sub>,...,a<sub>p</sub>],[b<sub>1</sub>,...,b<sub>q</sub>],x) |
| Bilateral Hypergeometric Function | <sub>A</sub>H<sub>B</sub>(a<sub>1</sub>,...,a<sub>A</sub>;b<sub>1</sub>,...,b<sub>B</sub>;x) | AHB([a<sub>1</sub>,...,a<sub>A</sub>],[b<sub>1</sub>,...,b<sub>B</sub>],x) | mpmath.bihyper([a<sub>1</sub>,...,a<sub>A</sub>],[b<sub>1</sub>,...,b<sub>B</sub>],x) |
| Dirichlet Eta Function | &eta;(x) | eta(x) | mpmath.altzeta(x) |
| Jacobi Theta Function | &theta;<sub>n</sub>(x,q) | theta(n,x,q) | mpmath.jtheta(n,x,q) |
| Riemann Zeta Function | &zeta;(x) | zeta(x) | mpmath.zeta(x) |
| Hurwitz Zeta Function | &zeta;(x,a) | zeta(x,a) | mpmath.zeta(x,a) |
| Lerch Transcendent Function | &Phi;(x,s,a) | Phi(x,s,a) | mpmath.lerchphi(x,s,a) |
| Polylogarithm | Li<sub>s</sub>(x) | Li(s,x) | mpmath.polylog(s,x) |

### Numerical Algorithms

#### Root Finder

##### Bisection Method

##### Fixed-Point Iteration

##### Newton's Method

##### Secant Method

##### Method of False Position

##### Modified Newton's Method

##### Steffensen's Method

##### Muller's Method

#### Interpolation Calculator

##### Lagrange Interpolating Polynomials

##### Neville's Method

##### Newton's Divided Difference Method

##### Hermite Interpolation

##### Natural Cubic Spline

##### Clamped Cubic Spline

#### Numerical Differentiator

##### Forward Difference

##### Backward Difference

##### Central Difference

##### Three-Point Midpoint Formula

##### Three-Point Endpoint Formula

##### Five-Point Midpoint Formula

##### Five-Point Endpoint Formula

#### Numerical Integrator

##### Midpoint Rule

##### Trapezoid Rule

##### Simpson's Rule

##### Romberg Integration

##### Adaptive Quadrature

##### Gaussian Quadrature

#### Numerical Solver

##### Euler's Method

##### Midpoint Method

##### Modified Euler Method

##### Heun's Method

##### Runge-Kutta Method

##### Runge-Kutta-Fehlberg Method

##### Adams-Bashforth Technique

##### Milue's Method

##### Extrapolation

Note: To view this information in the app click the "Help" button in the lower left.

___
## Future Work

When I began writing the code to evaluate mathematical expressions I did so with the intention of using the _eval_ function, but upon learning that _eval_ is insecure I decided to take a different approach. As a result, some of the code I wrote previously is not necessary. A future update will clean up this code.

The current version of this project displays the numerical solution, but has no way to visualize this solution. In future versions I will add plots as part of the outputs for the various numerical techniques that have been implemented.

This project implements various commonly used numerical methods, but there is much more that can be added including techniques of numerical linear algebra, numerical optimization and numerical partial differential equation. I eventually want to implement methods from all these areas of numerical analysis.

Some of the algorithms can take a very long time to run depending on the inputs, as a result this can cause the program to crash. To mitigate this, I will add a settings menu in a future update that will include the option to set the maximum number of iterations before the algorithm terminates.

Some of the techniques implemented make use of a base method prior to running the main method. For example, the current implementation of Romberg integration uses the trapezoid rule as a base method, before extrapolating to produce a refined approximation. Future versions will allow the user to choose which base methods the program uses.
___
## Acknowledgements

I acknowledge the extensive use of the math and mpmath Python modules in this project and am grateful for the work done by the creators of these packages. Without these libraries this project would have been much harder.

The book Numerical Analysis by Burden & Faires, 9th edition was used as a reference over the course of the project, and I thank the authors of this book which served as a valuable resource.

Furthermore, Wolfram MathWorld allowed me to learn about the various special functions I did not know about prior to this project. I thank the creators of this website, for the material I referred to during this project. As well as serving as a great resource for nearly every area of mathematics.

I thank the owner of the YouTube channel Clear Code. His tkinter tutorial helped me learn how to create user interfaces in Python. Including the one for this project.

I thank Liu Zuo Lin for his [Medium article](https://medium.com/codex/another-python-question-that-took-me-days-to-solve-as-a-beginner-37b5e144ecc) on how to evaluate Python strings as mathematical expressions. This helped me avoid the use of the _eval_ and _exec_ functions, which have been shown to be insecure.

Note: To view this information in the app click the "Acknowledgements" button in the lower right.

___
## Disclaimer

This project was originally created by Joseph W Barnett. As long as credit is given to the original author, it can be altered and distributed for noncommercial use.
