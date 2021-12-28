# DYNA2GAMS - optimal control with GAMS

The __DYNA2GAMS__ project aims at solving optimal control problems with the help of the
[GAMS](https://www.gams.com) modeling language.

Optimal control deals with the problem of finding a control law for a given dynamical system
governed by differential equations such that a certain optimality criterion is achieved.
Optimal control problems arise in many exciting applications in science, economy, and
engineering. Examples are trajectory optimization in robotics, aerospace engineering
(ascent/descent/emergency trajectories, orbit transfers...), vehicle simulation (avoidance
trajectories, virtual test-driving, chassis control...), controller design (linear quadratic
regulator, model-predictive control...), process engineering (chemical processes...),
fishing strategies, biology, etc.

The General Algebraic Modeling System ([GAMS](https://www.gams.com/products/gams/gams-language/))
is a high-level modeling system for mathematical programming and optimization. It consists of
a language compiler and a range of integrated high-performance solvers. GAMS is specifically
designed for modeling linear, nonlinear and mixed integer optimization problems.

In a nutshell, optimal control problems (OCP) are usually described by:
- A state-space model of a system. This can be either a set of ordinary differential
  equations or differential algebraic equations.
- Initial and/or final conditions (sometimes also conditions at other points).
- A cost functional, i.e. a scalar value that depends on the state trajectories and the
  control function which has to be minimized or maximized.
- Sometimes, additional equations and variables that, for example, relate the initial and
  final conditions to each other or constraint the control or state path.
The goal of __DYNA2GAMS__ suite is to make it possible to input such problem descriptions as
simply as possible, without having to worry about the mathematics of the actual solver. Once
a problem has been properly modeled, __DYNA2GAMS__ suite will take care of all the steps
necessary in order to return a solution.

__DYNA2GAMS__ translates a model written in DYNA dialect to a GAMS file, which can be further
processed by GAMS. In other words, it transcribes optimal control problems (OCP) into large
but sparse nonlinear programming problems. In doing so, it allies the power of a
mathematical programming tool with a set of high level features dedicated to optimal control
that simplify the formulation of the problems.

DYNA dialect allows to formulate optimal control problems in a way that is very similar to
their mathematical description. Take a look at the [Tutorial](https://dyna2gams.github.io/tutorial.html)
to grasp the basic structure and characteristics of a DYNA model and how it relates to the
mathematical formulation.

__DYNA2GAMS__ has been developed in the course of the year 2018 and is regularly updated since
then. It is available for download on this web site. On top, it comes with a very large set of
examples borrowed from the literature and various academic or commercial OCP solvers.

__DYNA2GAMS__ is free of charge for non-commercial use throughout the year 2022 at least. It is
licensed under the
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International terms](https://creativecommons.org/licenses/by-nc-sa/4.0/).
It is based on [Regina Rexx Interpreter](https://regina-rexx.sourceforge.io/).
Regina is distributed under the terms of the GNU Library General Public License Version 2.

Please visit our [website](https://dyna2gams.github.io/).

Feel free to contact us for any questions you might have (dyna2gams@outlook.com).

Copyright (c) 2018-2021 Alain J. Michiels. All rights reserved.
