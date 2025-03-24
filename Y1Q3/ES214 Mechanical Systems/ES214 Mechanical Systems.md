# What is Mechanical Systems?

Mechanical Systems is a course that studies systems in motion, also known as 'Dynamics'. It builds off of the content found in [[ES201 Conservation & Accounting Principles]] and aims to deepen the our understanding of kinematics and kinetics of rigid bodies. 

# What are the Learning Objectives?
- Apply the rate form of linear and angular momenta conservation to particles and rigid bodies undergoing planar motion
- Apply the finite-time form of linear and angular momenta conservation to particles and rigid bodies undergoing planar motion with or without an impact
- Apply the finite-time form of energy conservation to particles and rigid bodies undergoing planar motion
- Analyze the unconstrained or constrained kinematics of particles and rigid bodies undergoing planar motion
- Create and execute a numerical simulation of a dynamic system using Simulink and MATLAB
# Why Study Mechanical Systems?
Not every system will be stationary, as nice as that would be. MSys allows us to study these systems in motion in a more meaningful way.

# Concepts from ES201 ConApps
The Rate Form of conservation of Linear Momentum is :
$$\frac{d \overrightarrow P_{sys}}{dt} = \Sigma \overrightarrow F +\Sigma \dot m_{in} \overrightarrow V_{in} - \Sigma \dot m_{out} \overrightarrow V_{out}$$
The Rate form of Conservation of Angular Momentum is:
$$\frac{d \overrightarrow L_{sys}}{dt} = \Sigma \overrightarrow M_{o} + \Sigma (\overrightarrow r_{in} \times \dot m_{in} \overrightarrow V_{in}) - \Sigma(\overrightarrow r_{out} \times \dot m_{out} \overrightarrow V_{out}) $$
The Rate form of Conservation of Energy is:
$$\frac{dE_{sys}}{dt} = \dot W_{in,net} + \dot Q_{in,net} +\Sigma \dot m_{in}(h+\frac{v^2}{2}+gz)_{in} - \Sigma \dot m_{out}(h+\frac{v^2}{2}+gz)_{out} $$
## How will these concepts be applied in ES204?
We'll be investigating *adiabatic* and (primarily) closed systems. When applied to the core concepts from ConApps, it yields the following:
$$\frac{d\overrightarrow P_{sys}}{dt} = \Sigma \overrightarrow F \tag{1}$$
$$\frac{d \overrightarrow L_{sys}}{dt} = \Sigma \overrightarrow M_{o \tag{2}} $$
$$\frac{dE_{sys}}{dt} = \dot W_{in,net} $$
These 3 equations can be put into their Finite Forms:

| Conservation Principle | Rate Form                                                                | Finite Form                                                                                         |
| ---------------------- | ------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| Linear Momentum        | $$m\overrightarrow a = \frac{d\overrightarrow P_{sys}}{dt}=\Sigma F $$   | $$m\overrightarrow v_{2}-m\overrightarrow v_{1} = \Delta\overrightarrow P_{sys} = \int\Sigma Fdt $$ |
| Angular Momentum       | $$\frac{d\overrightarrow L_{sys,o}}{dt} = \Sigma\overrightarrow M_{o} $$ | $$\Delta\overrightarrow L_{sys,O} = \int\Sigma\overrightarrow M_{o} dt $$                           |
| Energy                 | N/A                                                                      | $$\Delta E_{sys} = W_{i\rightarrow f}$$                                                             |
## When would I use each of these conservation principles?
| Conservation Principle  | Rate Form                                                                                                                                                     | Finite Form                                                                                                                                                     |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Linear/Angular Momentum | - Want to find forces, moments, or accelerations<br>- Want to find velocities or distances travelled (integrate the kinematic relationships for acceleration) | - Have an impact, impulsive force, or several objects interacting<br>- Wanting to find velocities, times, or forces<br>- Given force as a function of time      |
| Energy                  |                                                                                                                                                               | - Interested only in particular states of a system<br>- Want to find speeds, distances, or forces (occasionally)<br>- Given force as a function of displacement |
## What's the procedure to solve problems in ES204?
1. Determine with what kind of problem you are dealing with
	1. Are we dealing with an impact, or are we interested in the energy of a system?
2. Define the system you need to analyze
	1. What do we care about
3. Establish a coordinate system
4. Draw an appropriate diagram
	1. Kinetic Diagram/Free Body Diagram for CoLM/CoAM problems
	2. Energy Interaction Diagram for CoE problems
5. Apply the appropriate conservation principles and kinematic relationships
6. Check that you have enough independent equations to solve for the unknowns
	1. Solving a system of equations, at least the same number of equations as solutions
7. Solve the system of equations
# Review of Kinematic Relationships
| Kinematic Term | Symbol | Definition                           | Standard Units   |
| -------------- | ------ | ------------------------------------ | ---------------- |
| Position       | $$x$$  | $$-$$                                | $$m, ft$$        |
| Velocity       | $$v$$  | $$v=\frac{dx}{dt}$$                  | $$m/s, ft/s$$    |
| Acceleration   | $$a$$  | $$a=\frac{dv}{dt} = \frac{dv}{dx}v$$ | $$m/s^2,ft/s^2$$ |
## Review of Separation of Variables
Given $v$ or $a$, we can separate variables and integrate to find $x$. ie:

If: $v(t) \rightarrow v(t) = \frac{dx}{dt}$
	$\int dx = \int v(t)dt \rightarrow x = \int v(t)dt$
If: $v(t) \rightarrow v(x) = \frac{dx}{dt}$
	$\int dt = \frac{1}{v(x)} \rightarrow t=\int\frac{1}{v(x)}$
If: $a(x) \rightarrow a(x)$
	$\frac{d}{dt}(v(x)) = \frac{d}{dt}v(x(t)) = \frac{d}{dx}v(x)*\frac{d}{dt}x(t)$
	$a(x) = \frac{dv}{dt}v(t) \rightarrow \int a(x)dx = \int vdv$
If: $a(v) \rightarrow a(v) = \frac{dv}{dx}v$
	$\int dx = \int \frac{v}{a(v)}dv$
If: $a(v) \rightarrow a(v) = \frac{dv}{dt}$
	$\int dt = \int \frac{1}{a(v)}dv$
	