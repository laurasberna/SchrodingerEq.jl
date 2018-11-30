# SchrodingerEq.jl

A project for the Computational Physics UW course (module III), by Laura Sberna. In this project, composed of two notebooks, we solve the time dependent Shroedinger equation in one spatial dimension.

<!-- # To do:
- create git repository (done)
-PLC (done?)
- wave function struct (done)
- initial state (done)
- discretization, rhs (done)
- euler (done)
- rk 2 (done)
- rk 4 (done)
- free in a box animation with classical solution (done)
- potential (done)
- box condition (done?)
- derive finite difference for laplacian (done)
- barrier in a box (done)
- animation (with classical solution) (done)
- better parameters for barrier (done)
- convergence tests (done)
- classical sol for free (done)
- compare codes (first improve n): import data and compare. (done)
- comments and remove useless text from notebook, save pictures (1 done, 2  done)
- quantitative comparison codes. (?)
- write readme (add pictures)
- tag the final commit as "version 1 release"

links:[ATNF catalogue](http://www.atnf.csiro.au/research/pulsar/psrcat/)
imgs:<img src="https://i.imgur.com/AybngWD.png" width="600" height="400">
-->

## Solving the time dependent Schrodinger equation

The time dependent Schrodinger equation describes the evolution of the wavefunction of a quantum system. The equation is a parabolic PDE. 

We implement a fourth order Runge-Kutta solver with second order discretization in space. We test the solver for a free particle, implementing a series of tests to make sure that the code is reliable. 

<img src="https://i.imgur.com/k1YiFhn.gif" width="600" height="400"> 

In the following test, for instance, we show that the difference between the numerical and exact solution decreases as the resolution is improved (increasing the number of grid points).

<img src="https://i.imgur.com/CW8qh2X.png" width="600" height="400">

A more interesting application is the quantum tunneling of a Gaussian packet through a square barrier. For this problem, we compare the output of the Runge-Kutta solver with that of a different solving algorithm, the Suzuki-Trotter method (for more information, see [de Vries and De Raedt](https://journals.aps.org/prb/abstract/10.1103/PhysRevB.47.7929) ). The Suzuki-Trotter solver has fourth order accuracy in both space and time. The two solvers are in excellent qualitative agreement, as the figure shows.

<img src="https://i.imgur.com/dclGNxM.gif" width="600" height="400"> 

## Acknowledgment 

The Suzuki-Trotter solver was set up by Job Feldebrugge. 

