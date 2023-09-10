# NumericalMethodsCalculator

A calculator which implement various numerical methods and includes support for many special functions.
___
## About The Project

Numerical methods, also referred to as numerical analysis, is a branch of mathematical analysis which studies methods of approximating solutions, and deriving error bounds, to problems which are either too difficult or even impossible to solve exactly. It has applications to many disciplines in STEM and business including, but not limited to computational physics, computational chemistry, engineering, conputational finance, and acturial science.

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

#### Functions

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

When I began writing the code to evaluate mathematical expression I did so with the intent of using the _eval_ function, but upon learning the _eval_ is insecure I decided to take a different approach. As a result some of the code I wrote previously is not necessary. A future update will clean up this code.

The current version of this project displays the numerical solution, but has no way to visulize it. In future versions. I will add plots as part of the outputs for the various numerical techniques that have been implemented.

This project implements various commonly used numerical, but there is much more that can be abbed including techniques of numerical linear algebra, numerical optimization and numerical partial differental equation. I eventually want to implement methods from all the areas of numerical analysis.
___
## Acknowledgements

I acknowledge the extensive use of the math and mpmath Python modules in this project and am grateful for the work done by the creators of these packages. Without these libraries this project would have been much harder.

The book Numerical Analysis by Burden & Faires, 9th edition was used as a reference over the course of the project, and I thank the authos of this book which served as a valuable resource.

Furthermore, Wolfram MathWorld allowed me to learn about the various special functions I didn't know about prior to this project. I thank the creators of this website, for the material I referred to during this project. As well as serving as a great resource for nearly every area of mathematics

I thank the owner of the YouTube channel Clear Code. His tkinter tutorial helped me learn how to create user interfaces in Python. Including the one for this project.

I thank Liu Zuo Lin for his [Medium article](https://medium.com/codex/another-python-question-that-took-me-days-to-solve-as-a-beginner-37b5e144ecc) on how to evaluate Python strings as mathematical expressions. This helped me avoid the use of the _eval_ and _exec_ functions, which have been shown to be insecure

Note: To view this information in the app click the "Acknowledgements" button in the lower right.

___
## Disclaimer

This project was originally created by Joseph W Barnett. As long as credit is given to the original author, it can be altered and distributed for noncommercial use.
