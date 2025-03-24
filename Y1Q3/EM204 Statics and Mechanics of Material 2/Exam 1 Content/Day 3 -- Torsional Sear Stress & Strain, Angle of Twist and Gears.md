# Learning Objectives
1. Calculate the shear stress and shear strain experienced at any point in a shaft
2. Describe the sign conventions as used for uniaxial & torsion loading
3. Calculate max shear stress for torsion problems involving gears
4. Calculate angle of twist for torsion problems involving gears

# Shear Strain and Shear Stress
Torques (twisting forces) inside a shaft cause **shear stress** and **shear strain**.

Take a shaft with radius $c$ and length $L$. When a torque is applied to the free end of the shaft, $B$ will be displaced from its original position to a new position, $B'$, a distance $\theta$ away. We can analyze the triangle created, Triangle $ABB'$. We take the angle of deflection, $\gamma$ to be very small such that $\overline{AB'} \perp \overline{BB'}$ . Analyzing $ABB'$, we find that:
$$tan(\gamma_{max}) = \frac{BB'}{AB}=\frac{c\theta}{L}$$
Given that we assume that $\gamma$ is a very small angle, we find that
$$\gamma = \frac{c\theta}{L}$$
and for any radii, $\rho$, we find:
$$\gamma_{\rho} = \frac{\rho\theta}{L}\tag{1}$$
Given that $\theta$ is the angle between $B$ and $B'$, we can define:
$$\theta=\frac{L}{\rho}\gamma_{\rho}\tag{1.1}$$
Substituting $(1)$ into $(2)$, we find that:
$$\gamma_{max} = \frac{c}{L}\frac{L}{\rho}\gamma_{\rho}$$
$$\gamma_{max}=\frac{c}{\rho}\gamma_{\rho}\tag{2}$$
where $\gamma_{max}$ represents the shear strain at any radius $\rho$, $\theta$ is the angular displacement of the end of that radius, and $L$ represents the length of the shaft. Solving $\gamma$ for the radius of the shaft, we find:
$$\gamma_{max}=\frac{\theta c}{L}\tag{2.1}$$

Assuming that Hooke's Law applies in torsion/shear, we find that the shear stress, $\tau$, is given by:
$$\tau = G\gamma\tag{3}$$
where $\gamma$ is the strain in the shaft and $G$ is the shear modulus of the material. Substituting for $\gamma$, we find that:
$$\tau = \tau_{max}\frac{\rho}{c}$$
Given that the net effect from shear stress must balance the applied torque $T$, we find that
$$T = \int distance\cdot elemental force$$
$$T = \int \rho\cdot\tau(\rho)\cdot2\pi\rho d\rho$$
$$T = \frac{2\pi\tau_{max}}{c}\int_{0}^{c}\rho^3d\rho$$
$$T = \frac{2\pi\tau_{max}}{c}\cdot\frac{2\pi c^4}{4} = \frac{\tau_{max}}{c}\cdot\frac{\pi c^4}{2}$$
We then group the term $\frac{\pi c^4}{2}$ into a variable, $J$, representing the polar moment of inertia of the shaft. This then gives:
$$T = \frac{\tau_{max}}{c}J$$
$$\tau_{max}=\frac{Tc}{J}\tag{4}$$
For any radius $r$ or diameter $d$ of a solid shaft, $J$ is given by:
$$J = \frac{\pi r^4}{2}=\frac{\pi d^4}{32}\tag{5}$$
For a hollow shaft with an inner radius $c$ and outer radius $b$, or outer diameter $d_{o}$ and inner diameter $d_{i}$, $J$ is given by:
$$J = \frac{\pi(c^4-b^4)}{2} = \frac{\pi(d_{o}^4-d_{i}^4)}{32}\tag{6}$$
# Angle of Twist
From equations $(2.1)$, $(3)$, and $(4)$, we find that:
$$\frac{\theta c}{L} = \frac{Tc}{J}\cdot\frac{1}{G}$$
$$\frac{T}{JG} = \frac{\theta}{L}$$
solving for $\theta$, we find that the angle of twist can be expressed in radians as:
$$\theta = \frac{TL}{JG}\tag{7}$$
# Gear Ratios
For two gears, $A$ and $B$ with radii $r_{A}$ and $r_{B}$that experience torques $T_{A}$ and $T_{b}$, we can establish a relationship using arclengths such that:
$$r_{A}\theta_{A} = r_{B}\theta_{B}$$
which gives the following relationship:
$$\frac{r_{A}}{r_{B}}=\frac{\theta_{B}}{\theta_{A}}=\frac{N_{A}}{N_{B}}\tag{8}$$
where N is the number of teeth on the gear.