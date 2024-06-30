# Numerical modeling of Polymerization reaction
Numerical solution of differential equations for modeling the simplest catalysis reaction A + B $\to$ A + C

# Description
The reacting system can be described as a finite volume with a random initial distribution $N$ particles in 
it and given periodic boundary conditions. We assume that the reaction occurs with probability $p = 0.001$ when 
particles $A$ and $B$ are closer than $4.0 nm$ to each other. The interaction of particles can be described 
using the following potential:

$\V(vec{r_i}, vec{r_j)) = $varepsilon*[ C_1*(\sigma/r_ij)^4 + C2*(\sigma/r_ij)^2]
$$\begin{cases}
    \frac{\partial \vec{u}}{\partial t} + (\vec{u}, \nabla) \vec{u} - \nu \Delta \vec{u} + \nabla p = \vec{0} \\
    (\nabla, \vec{u}) = 0
\end{cases}$$
