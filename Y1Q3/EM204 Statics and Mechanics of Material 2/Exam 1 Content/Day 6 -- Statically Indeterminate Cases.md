# Learning Objectives
1. Design statically indeterminate transmission shafts
# Axially Loaded Cases
Typically when solving statics problems, the sum of forces in each direction will give us enough equations to solve for any unknowns. However, in the situations where force equilibrium does not provide enough equations to solve for all unknowns, we must look at displacements. These cases are known as "statically indeterminate cases"

## Solving a typical statically indeterminate problem
1. Equilibrium equations: $$\Sigma F_{y}=0 \quad \rightarrow \quad F_{a}+F_{b}=P$$
which provides 1 equation with 2 unknowns. 
2. Load deflection: $$\delta_{a} = \frac{F_{a}L_{a}}{A_{a}E_{a}};\quad \delta_{b}=\frac{F_{b}L_{b}}{A_{b}E_{b}}$$
which then provides another 2 equations in 2 unknowns. This brings our total to 3 equations in 4 unknowns.
3. Geometric constraints: $$\delta_{a}=\delta_{b}$$
which gives us another equation in 0 unknowns, bringing our totals to 4 equations in 4 unknowns.

# Torsion Cases
The solving steps for a torsional case are very similar to an axially loaded case. Start with equilibrium equations, look at load deflections, and observe your geometric constraints. This should yield enough equations to solve for all of your unknowns.

## Solving a typical statically indeterminate problem in Torsion
1. Equilibrium equations: $$\Sigma M_{x} = 0 =T-T_{a}-T_{b} \quad \rightarrow \quad T = T_{a}+T_{b}$$
yielding 1 equation in 2 unknowns.
2. Load deflection: $$\theta_{A}=(\frac{TL}{JG})_{A};\quad \theta_{b}=(\frac{TL}{JG})_{B}$$
which yields 2 equations in 2 unknowns, raising our count to 3 equations in 4 unknowns.
3. Geometric constraints: $$\theta_{T}=0=\theta_{A}+\theta_{B}$$
which is our fourth equation, giving us 4 equations in 4 unknowns. We can then proceed to solve the system of equations for all of our unknowns.