# SchrodingerEq.jl

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

The time dependent Schrodinger equation describes the evolution of the wavefunction $\Psi$ of a quantum system. In one spatial dimension, the equation reads
\begin{equation}
i \hbar \frac{\partial \Psi}{\partial t} = -\frac{\hbar^2}{2 m} \frac{\partial^2 \Psi}{\partial^2 x} + V(x) \Psi \ ,
\end{equation}
where $t$ is the time parameter, $x$ is the space coordinate, $m$ the mass of the particle and $\hbar$ is the Plank constant. The probability density to find the particle at the position $x$ at time $t$ will be given by $|\Psi|^2$. 
 

## Acknowledgment 


