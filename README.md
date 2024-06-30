# Numerical modeling of Polymerization reaction
Numerical solution of differential equations for modeling the simplest catalysis reaction A + B $\to$ A + C

# Description
The reacting system can be described as a finite volume with a random initial distribution $N$ particles in 
it and given periodic boundary conditions. We assume that the reaction occurs with probability $p = 0.001$ when 
particles $A$ and $B$ are closer than $4.0 nm$ to each other. The interaction of particles can be described 
using the following potential:

$\ V ( \vec{r_i}, \vec{r_j} ) $ 
= $\\varepsilon [ C_{1} (\sigma/r_{ij})^4 + C_{2} (\sigma/r_{ij})^2]$

where $\ \varepsilon = 1.0 kJ/mol $ - energy constant,
 $\ \sigma = 1.0 nm$ — equilibrium distance between particles, $C_{1}$ and $C_{2}$ - constants,
$\ r_{ij} $  = $\ \mid \vec{r_i} - \vec{r_j} \mid $ — current distance between particles. If you set constants $C_1 = 1.0$, $C_2 = -2.0$, then the interaction between particles will be attractive, and at $C_1 = 0$, $C_2 = 1$ - repulsive. Let us assume that the reaction product $C$ polymerizes. Then the result of the reaction will be a polymer consisting of molecules of the type $C$. To describe the polymerization process, it is proposed to use a potential with attractive constants ($C_1 = 1.0$ and $C_2 = -2.0$) if both particles are of type $C$ and repulsive ($C_1 = 0$ and $C_2 = 1$) otherwise.
