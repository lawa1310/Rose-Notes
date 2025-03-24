# Learning Objectives
1. Calculate the ***shear stress*** on oblique planes using the principle of equilibrium of forces
2. Calculate the ***normal stress*** on oblique planes using the principle of equilibrium of forces
3. Design transmission shafts for given constraints
# Stress on Oblique Planes
From empirical studies, ductile materials fail in shear while brittle materials fail in tension. In other words, ductile materials tend to fail with a straight fault like while brittle materials tend to fail with angled fault lines.

When a torque is applied to a shaft, the "fibers" of the material experience shear.

If we consider a small element on the surface of a shaft at the point $A$: $dx$, $dy$, and $dz$, we can draw a rectangle with sides $dx$ and $dy$ and depth $dz$. The forces along the edges of the area concentrate towards two opposite corners. If we apply an equilibrium of forces in the normal and tangential direction, we find that:
$$\Sigma F_{n} = 0:\sigma_{n}dA-(\tau_{xy}dAcos(\alpha))sin(\alpha)-(\tau_{xy}dAsin(\alpha))cos(\alpha)$$
$$\Sigma F_{t} = 0: \tau_{nt}dA-\tau_{xy}dAcos(\alpha)cos(\alpha)+\tau_{xy}dAsin(\alpha)sin(\alpha)$$
These simplify to the following expressions:
$$\sigma_{n}=2\tau_{xy}sin\alpha cos\alpha = \tau_{xy}sin(2\alpha)\tag{1}$$
$$\tau_{nt} = \tau_{xy}(cos^2\alpha-sin^2\alpha)=\tau_{xy}cos(2\alpha) \tag{2}$$
where $\alpha$ is the angle between the vertical and the oblique plane, or the normal direction and the horizontal.

When $\sigma_{n}$ and $\tau_{xy}$ are plotted, we find that $\sigma_{n}$ is maximized at $45\textdegree$ to the shaft cross section, and $\tau_{xy}$ is maximized at $0\textdegree$ to the cross-section.
# Design of Transmission Shafts
The amount of power transmitted depends on the torque applied to the shaft and the angular speed of the shaft.

## Governing Equation
$$P = T\omega$$
but given that $\omega = 2\pi f$, we can rewrite $P$ as:
$$P = 2\pi fT \tag{3}$$
where $\omega$ is in radians per second, $f$ is cycles/sec or Hz