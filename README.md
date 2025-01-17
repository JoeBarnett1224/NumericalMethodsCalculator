# Numerical Methods Calculator

A calculator which implements various numerical methods and includes support for many special functions.
___

## About The Project

Numerical methods, also referred to as numerical analysis, is a branch of mathematical analysis which studies methods of approximating solutions, and deriving error bounds, to problems which are either too difficult or even impossible to solve exactly. It has applications to many disciplines in STEM and business including, but not limited to computational physics, computational chemistry, engineering, computational finance, and actuarial science.

Much of mathematics is based on the idea of functions. This project implements support for many of the functions taught in grade school including polynomials, exponentials, logarithms, trigonometric, and hyperbolic functions. Also included is support for many of the special functions used in more specialized areas of mathematics including mathematical physics, probability, real analysis, complex analysis, analytic number theory, ordinary differential equations, and partial differential equations. The gamma function, error function, and Bessel functions are just a few of the special functions which are supported.

See [Instructions](#Instructions) for more information regarding the functions and numerical algorithms that are implemented.
___

## Version History
__NumericalMethodsCalculator2__: This version features various code improvements including conversion from a function-based approach to a class-based approach. A couple of minor bugs were fixed.
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

Below are instructions on how to use this app, including supported functions and implemented numerical methods.

### Supported Constants and Functions

Many of the numerical methods implemented in this app require the user to input one or more functions, which are interpreted as Python strings.

The supported mathematical operations are addition (+), subtraction (-), multiplication (*), division (/), and exponentiation (^). The app follows the order of operations taught in grade school.

This app implements various mathematical constants and functions. See [Constants](#Constants) and [Functions](#Functions) to see which constants and functions are supported and how they are implemented. When using a mathematical function be sure to enclose the argument(s) in parenthesis. For example, use sin(x), not sinx.

#### Constants

| Mathematical Constant | Mathematical Notation | Implementation | Python Function |
| --- | --- | --- | --- |
| Pi | &pi; | pi | math.pi |
| Euler's Number | e | e^(1) | math.exp(1) |
| Golden Ratio | &phi; | phi | mpmath.phi |
| Euler-Mascheroni Constant | &gamma; | gamma | mpmath.euler |
| Glaisher-Kinkelin Constant | A | A | mpmath.glaisher |
| Catalan's Constant | G | (Phi(-1,2,1/2))/4 | (mpmath.lerchphi(-1,2,1/2))/4 |
| Infinity | $\infty$ | infinity | math.inf |

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

This app implements many of the most commonly used numerical methods. It includes a [root finder](#Root-Finder), an [interpolation calculator](#Interpolation-Calculator), a [numerical differentiator](#Numerical-Differentiator), a [numerical integrator](#Numerical-Integrator), and a [numerical solver](#Numerical-Solver). Below are instructions on how to use these tools.

#### Root Finder

Root finding is the process of finding solutions, also called roots or zeros, of the equation f(x) = 0. A similar procedure is determining fixed points of a function, or values of x which satisfy the equation f(x) = x. Some equations, such as x<sup>2</sup> - 7x + 12 = 0, can be easily solved analytically. However, equations like tanx = x cannot be solved analytically. In these cases, numerical techniques must be used to approximate a solution. The techniques include bracketing methods and iterative methods.

Bracketing methods start with a closed interval [a,b] such that the function is continuous over the interval and f(a) and f(b) have opposite signs. By the Intermediate Value Theorem, it is then known that a root exists between a and b. Bracketing methods shorten the size of this interval while still maintaining the conditions of the Intermediate Value Theorem, and proceeds until the interval is small enough to approximate the root within a given tolerance. Bracketing methods implemented in this app include the [bisection method](#Bisection-Method) and the [method of false position](#Method-of-False-Position).

Iterative methods begin with one or more initial approximations. These data are then used to derive a better approximation which is then used to derive an even better approximation. The process continues until a root is found within a given tolerance. [Fixed-point iteration](#Fixed-Point-Iteration), [Newton's method](#Newtons-Method), the [secant method](#Secant-Method), [modified Newton's method](#Modified-Newtons-Method), [Steffensen's method](#Steffensens-Method), and [Muller's method](#Mullers-Method) are the iterative methods implemented in this app.

##### Bisection Method

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): Left endpoint of interval. The function value at f(a) must have a different sign than at f(b).

- b (float): Right endpoint of interval. The function value at f(b) must have a different sign than at f(a).

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = 0 and estimated error derived via the bisection method, or message that the conditions of the Intermediate 
Value Theorem are not met. 

##### Fixed-Point Iteration

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x<sub>0</sub> (float): Initial approximation for fixed point.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = x and estimated error derived via fixed-point interation. 

##### Newton's Method

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- Derivative (string): Derivative of given function with respect to x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x<sub>0</sub> (float): Initial approximation for root.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = 0 and estimated error derived via Newton's method.

##### Secant Method

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x<sub>0</sub> (float): First initial approximation for root.

- x<sub>1</sub> (float): Second initial approximation for root.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = 0 and estimated error derived via the secant method.

##### Method of False Position

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): Left endpoint of interval. The function value at f(a) must have a different sign than at f(b).

- b (float): Right endpoint of interval. The function value at f(b) must have a different sign than at f(a).

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = 0 and estimated error derived via the method of false position, or message that the conditions of the Intermediate Value Theorem are not met. 

##### Modified Newton's Method

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- Derivative (string): First derivative of given function with respect to x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- Second Derivative (string): Second derivative of given function with respect to x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x<sub>0</sub> (float): Initial approximation for root.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = 0 and estimated error derived via modified Newton's method.

##### Steffensen's Method

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x<sub>0</sub> (float): Initial approximation for fixed point.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = x and estimated error derived via Steffensen's method. 

##### Muller's Method

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x<sub>0</sub> (float): First initial approximation for root.

- x<sub>1</sub> (float): Second initial approximation for root.

- x<sub>2</sub> (float): Third initial approximation for root.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of f(x) = 0 and estimated error derived via Muller's method.

#### Interpolation Calculator

Given any set of data there will be gaps in the data. As a result, there are often missing data points for which information needs to be determined. The process of estimating these missing data points based on given data is called interpolation. Included in the techniques of interpolation are polynomial interpolation and spline interpolation.

Polynomial interpolation is based on the idea that given n data points there is a unique polynomial of maximum degree n - 1 that agrees with the data. Polynomial interpolation determines this polynomial and evaluates it at the point(s) to be determined. Four methods of polynomial interpolation implemented in this app include the use of [Lagrange interpolating polynomials](#Lagrange-Interpolating-Polynomials), [Neville's method](#Nevilles-Method), [Newton's divided difference method](#Newtons-Divided-Difference-Method), and [Hermite Interpolation](#Hermite-Interpolation).

Given n data points, spline interpolation fits a polynomial to the data in each of the n - 1 subintervals. This app uses cubic splines, meaning each subinterval approximates the data using a cubic polynomial. These polynomials agree at each of the data points and have continuous first and second order derivatives at the interior data points. In order to obtain a unique solution, conditions must be given at the two boundary points which are called boundary conditions. For a natural cubic spline, the second derivative is equal to zero at the boundary points. In a clamped cubic spline, the value of the first derivative is specified at each boundary point. [Natural cubic splines](#Natural-Cubic-Spline) and [clamped cubic splines](#Clamped-Cubic-Spline) are implemented in this app.

##### Lagrange Interpolating Polynomials

Inputs:

- x-values (string): x-coordinates of data set entered as floats separated by commas.

- y-values (string): y-coordinates of data set entered as floats separated by commas.

- x (float): Interpolation point.

Output:

- Estimated value of y-coordinate at interpolation point derived via Lagrange interpolating polynomial.

##### Neville's Method

Inputs:

- x-values (string): x-coordinates of data set entered as floats separated by commas.

- y-values (string): y-coordinates of data set entered as floats separated by commas.

- x (float): Interpolation point.

Output:

- Estimated value of y-coordinate at interpolation point derived via Neville's method.

##### Newton's Divided Difference Method

Inputs:

- x-values (string): x-coordinates of data set entered as floats separated by commas.

- y-values (string): y-coordinates of data set entered as floats separated by commas.

- x (float): Interpolation point.

Output:

- Estimated value of y-coordinate at interpolation point derived via Newton's divided difference method.

##### Hermite Interpolation

Inputs:

- x-values (string): x-coordinates of data set entered as floats separated by commas.

- y-values (string): y-coordinates of data set entered as floats separated by commas.

- y'-values (string): Derivative values at the x-coordinates of data set entered as floats separated by commas.

- x (float): Interpolation point.

Output:

- Estimated value of y-coordinate at interpolation point derived via Hermite interpolation.

##### Natural Cubic Spline

Inputs:

- x-values (string): x-coordinates of data set entered as floats separated by commas.

- y-values (string): y-coordinates of data set entered as floats separated by commas.

- x (float): Interpolation point.

Output:

- Estimated value of y-coordinate at interpolation point derived via natural cubic spline.

##### Clamped Cubic Spline

Inputs:

- x-values (string): x-coordinates of data set entered as floats separated by commas.

- y-values (string): y-coordinates of data set entered as floats separated by commas.

- f'(a) (float): Value of first derivative at the minimum x-value.

- f'(b) (float): Value of first derivative at the maximum x-value.

- x (float): Interpolation point.

Output:

- Estimated value of y-coordinate at interpolation point derived via clamped cubic spline.

#### Numerical Differentiator

Differentiation, along with integration, is one of the two major operators taught in calculus. The chain rule, product rule, and quotient rule are among the techniques used to compute derivatives analytically. Due to the wide applicability of the techniques the set of elementary functions is closed under differentiation, that is every elementary function has an elementary derivative. Even though any derivative can be found analytically, the more complicated the function becomes the less practical it becomes to compute the derivative by hand. In these cases, it is more practical to compute the derivative numerically. The finite difference methods, such as those included in this app, are the most common methods used to compute derivatives numerically.

Finite difference methods use a given step size and the given function evaluated at one or more points to approximate the derivative at a given point. The smaller the step size and the more points used in the evaluation, the more accurate the approximation. The definition of the derivative in terms of the difference quotient is used to derive the forward, backward, and central difference formulas. Higher order methods, including the three and five point formulas can be derived using Taylor series. The [forward difference method](#Forward-Difference), the [backward difference method](#Backward-Difference), the [central difference method](#Central-Difference), the [three-point midpoint formula](#Three-Point-Midpoint-Formula), the [three-point endpoint formula](#Three-Point-Endpoint-Formula), the [five-point midpoint formula](#Five-Point-Midpoint-Formula), and the [five-point endpoint formula](#Five-Point-Endpoint-Formula) are the finite difference methods implemented in this app.

##### Forward Difference

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x (float): Point where the derivative is approximated.

- h (float): Step size. The smaller the step size, the more accurate the approximation will be.

Output:

- The approximate values of the first and second derivatives at x derived via the forward difference method.

##### Backward Difference

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x (float): Point where the derivative is approximated.

- h (float): Step size. The smaller the step size, the more accurate the approximation will be.

Output:

- The approximate values of the first and second derivatives at x derived via the backward difference method.

##### Central Difference

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x (float): Point where the derivative is approximated.

- h (float): Step size. The smaller the step size, the more accurate the approximation will be.

Output:

- The approximate values of the first and second derivatives at x derived via the central difference method.

##### Three-Point Midpoint Formula

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x (float): Point where the derivative is approximated.

- h (float): Step size. The smaller the step size, the more accurate the approximation will be.

Output:

- The approximate values of the first and second derivatives at x derived via the three-point midpoint formula.

##### Three-Point Endpoint Formula

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x (float): Point where the derivative is approximated.

- h (float): Step size. The smaller the step size, the more accurate the approximation will be.

Output:

- The approximate values of the first and second derivatives at x derived via the three-point endpoint formula.

##### Five-Point Midpoint Formula

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x (float): Point where the derivative is approximated.

- h (float): Step size. The smaller the step size, the more accurate the approximation will be.

Output:

- The approximate values of the first and second derivatives at x derived via the five-point midpoint formula.

##### Five-Point Endpoint Formula

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- x (float): Point where the derivative is approximated.

- h (float): Step size. The smaller the step size, the more accurate the approximation will be.

Output:

- The approximated value of the first derivative at x derived via the five-point endpoint formula.

#### Numerical Integrator

Integration, along with differentiation, is one of the two major operators taught in calculus.  Substitution, integration by parts, and partial fraction decomposition are just a few of the many techniques used to compute integrals. Techniques such as substitution and integration by parts are general techniques and can be applied in many circumstances. However, techniques such as partial fraction decomposition and trigonometric substitution are more specialized and apply in specific cases. As a result, the set of elementary functions is not closed under integration, that is not every elementary function has an elementary antiderivative. In cases where an integrand does not have an elementary antiderivative, more sophisticated techniques such as Taylor series, differentiation under the integral sign, and contour integration can on occasion be used to obtain a solution analytically. For these reasons, integration is often a very difficult process, if even possible, and it is often more practical to use numerical methods to approximate integrals. These methods include the Newton-Cotes formulas, extrapolation, and quadrature. All of these techniques make use of the fact that the integral is just the signed area under a curve.

The Newton-Cotes formulas break up the interval of integration into subintervals, and then uses polynomial interpolation and equally spaced points to approximate the area over each subinterval. It then sums up all these areas to get the total area. The more subintervals, the more accurate the approximation. The Newton-Cotes formulas implemented in this app include the [midpoint rule](#Midpoint-Rule), the [trapezoid rule](#Trapezoid-Rule), and [Simpson's rule](#Simpsons-Rule).

The combination of a Newton-Cotes formula along with the technique of extrapolation is called Romberg integration. An advantage of this method is that it can be used to approximate an integral within a given tolerance. [Romberg integration](#Romberg-Integration) is implemented in this app.

Quadrature is similar to the use of the Newton-Cotes formulas, but instead of using predetermined weights and having the user specify the number of subintervals, it chooses the grid spacing and the weights at each point such that the integral is approximated as accurately as possible. [Adaptive quadrature](#Adaptive-Quadrature) and [Gaussian quadrature](#Gaussian-Quadrature) are implemented in this app.

##### Midpoint Rule

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): Lower limit of integration.

- b (float): Upper limit of integration.

- n (integer): Number of subintervals. The larger n is, the better the approximation.

Output:

- Approximate solution of the integral derived via the midpoint rule.

##### Trapezoid Rule

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): Lower limit of integration.

- b (float): Upper limit of integration.

- n (integer): Number of subintervals. The larger n is, the better the approximation.

Output:

- Approximate solution of the integral derived via the trapezoid rule.

##### Simpson's Rule

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): Lower limit of integration.

- b (float): Upper limit of integration.

- n (integer): Number of subintervals. The larger n is, the better the approximation. The value of n must be even.

Output:

- Approximate solution of the integral derived via Simpson's rule.

##### Romberg Integration

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): Lower limit of integration.

- b (float): Upper limit of integration.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of the integral and estimated error derived via Romberg integration.

Note: This algorithm uses the trapezoid rule as the base method.

##### Adaptive Quadrature

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): Lower limit of integration.

- b (float): Upper limit of integration.

- Tolerance (float): Acceptable error for approximation.

Output:

- Approximate solution of the integral and estimated error derived via adaptive quadrature.

Note: This algorithm uses Simpson's rule as the base method.

##### Gaussian Quadrature

Inputs:
  
- Function (string): Function with independent variable x. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- n (integer): Number of weights/nodes. The larger n is, the better the approximation.

Output:

- Approximate solution of the integral derived via Gaussian quadrature.

Note: Interval of integration is from -1 to 1.

#### Numerical Solver

Differential equations are equations which contain one or more independent variables, a function and one or more of its derivatives. An ordinary differential equation (ODE) contains only ordinary derivatives, whereas a partial differential equation (PDE) contains partial derivatives. The order of a differential equation is the order of its highest order derivative. Analytical solution techniques for solving first order ODEs include direct integration, integrating factors, separation of variables, potential functions, and substitution. However, these techniques can only be applied in very specific cases. In the vast majority of cases, one must resort to the use of numerical methods to approximate solutions to ODEs. This app implements various techniques for approximating solutions of first order ODEs including linear multistep methods and Runge-Kutta methods.

Linear multistep methods use a given step size to estimate the value of the solution to an ODE until it achieves an estimate for the solution at the desired point. At each step, an estimate for the solution is obtained using the value of the function and the derivative at previous points. [Euler's method](#Eulers-Method), the [Adams-Bashforth technique](#Adams-Bashforth-Technique), and [Milue's method](#Milues-Method) are the linear multistep methods implemented in this app.

Runge-Kutta methods are similar to the linear multistep methods except the Rung-Kutta methods also use the values of the function and derivative at half step sizes to compute an estimate at each point. The Runge-Kutta methods implemented in this app are the [midpoint method](#Midpoint-Method), the [modified Euler method](#Modified-Euler-Method), [Heun's method](#Heuns-Method), and the [Runge-Kutta Method](#Runge-Kutta-method),.

##### Euler's Method

Inputs:
  
- Function (string): Function with independent variables x and y. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): The x-value where the initial condition is specified.

- b (float): The x-value where the solution of the ODE is approximated.

- y(a) (float): Value of function where the initial condition is specified.

- N (integer): Number of steps. The larger n is, the better the approximation.

Output:

- Approximate solution of the ODE at x = b derived via Euler's method.

##### Midpoint Method

Inputs:
  
- Function (string): Function with independent variables x and y. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): The x-value where the initial condition is specified.

- b (float): The x-value where the solution of the ODE is approximated.

- y(a) (float): Value of function where the initial condition is specified.

- N (integer): Number of steps. The larger n is, the better the approximation.

Output:

- Approximate solution of the ODE at x = b derived via the midpoint method.

##### Modified Euler Method

Inputs:
  
- Function (string): Function with independent variables x and y. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): The x-value where the initial condition is specified.

- b (float): The x-value where the solution of the ODE is approximated.

- y(a) (float): Value of function where the initial condition is specified.

- N (integer): Number of steps. The larger n is, the better the approximation.

Output:

- Approximate solution of the ODE at x = b derived via the modified Euler method.

##### Heun's Method

Inputs:
  
- Function (string): Function with independent variables x and y. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): The x-value where the initial condition is specified.

- b (float): The x-value where the solution of the ODE is approximated.

- y(a) (float): Value of function where the initial condition is specified.

- N (integer): Number of steps. The larger n is, the better the approximation.

Output:

- Approximate solution of the ODE at x = b derived via Heun's method.

##### Runge-Kutta Method

Inputs:
  
- Function (string): Function with independent variables x and y. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): The x-value where the initial condition is specified.

- b (float): The x-value where the solution of the ODE is approximated.

- y(a) (float): Value of function where the initial condition is specified.

- N (integer): Number of steps. The larger n is, the better the approximation.

Output:

- Approximate solution of the ODE at x = b derived via the Runge-Kutta method.

##### Adams-Bashforth Technique

Inputs:
  
- Function (string): Function with independent variables x and y. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): The x-value where the initial condition is specified.

- b (float): The x-value where the solution of the ODE is approximated.

- y(a) (float): Value of function where the initial condition is specified.

- N (integer): Number of steps. The larger n is, the better the approximation.

Output:

- Approximate solution of the ODE at x = b derived via the Adams-Bashforth technique.

Note: This algorithm uses the Runge-Kutta method as the base method.

##### Milue's Method

Inputs:
  
- Function (string): Function with independent variables x and y. See [Supported Constants and Functions](#Supported-Constants-and-Functions).

- a (float): The x-value where the initial condition is specified.

- b (float): The x-value where the solution of the ODE is approximated.

- y(a) (float): Value of function where the initial condition is specified.

- N (integer): Number of steps. The larger n is, the better the approximation.

Output:

- Approximate solution of the ODE at x = b derived via Milue's method.

Note: To view this information in the app click the "Help" button in the lower left.

___

## Future Work

When I began writing the code to evaluate mathematical expressions I did so with the intention of using the _eval_ function, but upon learning that _eval_ is insecure I decided to take a different approach. As a result, some of the code I wrote previously is not necessary. A future update will clean up this code.

The current version of this project displays the numerical solution, but has no way to visualize this solution. In future versions I will add plots as part of the outputs for the various numerical techniques that have been implemented.

This project implements various commonly used numerical methods, but there is much more that can be added including techniques of numerical linear algebra, numerical optimization and numerical partial differential equations. I eventually want to implement methods from all these areas of numerical analysis.

Some of the algorithms can take a very long time to run depending on the inputs, as a result this can cause the program to crash. To mitigate this, I will add a settings menu in a future update that will include the option to set the maximum number of iterations before the algorithm terminates. Another option I would like to add to this settings menu is an option to set the precision of the calculations and outputs.

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
