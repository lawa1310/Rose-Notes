If you are confused with any of the following terminology, please refer to [[Helpful Terminology]]
# What are Accounting Principles?
Accounting principles are what allow us to keep track of the properties of a system. Fundamentally, the *fundamental accounting principle* that this class will interact can be written in two forms: the finite form and the rate form. 
## Finite and Rate Forms
The finite form of the fundamental accounting principle simply measures the change of a property of a system over time, $\Delta t$ . The change of a property of a system over time is simply the final state minus the initial state, giving the finite form of the fundamental account principle as $$B_{sys,f}-B_{sys,i}=B_{in}-B_{out}+B_{gen.}-B_{cons.} \tag{1} $$where $B_{in}$ and $B_{out}$ are simply the amount of the property that moves across the system boundary. $B_{gen}$ and $B_{cons.}$ are two terms that may or may not be applicable depending on the property being examined.

The rate form of the fundamental accounting principle measures the change of a property of a system over an infinitesimally small period of time, displayed as the time-based derivative of the change of the property in the system, represented as 
$$
\frac{dB}{dt}=\frac{dB_{in}}{dt}-\frac{dB_{out}}{dt}+\frac{dB_{gen}}{dt}-\frac{dB_{cons.}}{dt} \tag{2}

$$
where each term represents the change in the given property with respect to time.

In other words,

$B_{in}$ represents the amount of *B* that enters the system.
$\dot B_{in}$ represents the rate at which *B* enters the system.
$\Delta B_{sys} = B_{sys, final}-B_{sys, initial}$ represents the change in the amount of *B* in the system.
$\frac{dB_{sys}}{dt}$ represents the rate at which the amount of *B* changes in the system.

# Properties of Interest
If a property is conserved, then the generation and consumption terms must equal 0. ConApps focuses on the following properties:

| Property         | Is it Conserved?                             |
| ---------------- | -------------------------------------------- |
| Mass             | Yes (Conservation of Mass, CoM)              |
| Linear Momentum  | Yes (Conservation of Linear Momentum, CoLM)  |
| Angular Momentum | Yes (Conservation of Angular Momentum, CoAM) |
| Energy           | Yes (Conservation of Energy, CoE)            |
| Entropy          | **NO** (Accounting of Entropy, AoS)          |
All of these properties are extensive.

There are a few impacts on the fundamental accounting principles if certain criterion are met:
1. If an extensive property is *conserved*, there is no generation or destruction term for *B*
	1. $B_{gen}=0$, $B_{cons.}=0$ 
2. If the system of interest is closed, the property *B* cannot be transported into or out of the system
	1. $B_{in}=0$, $B_{out}=0$ 
3. If the system is at steady-state (S.S.), the amount of *B* cannot vary with time.
	1. $\frac{dB_{sys}}{dt}=0$

# More detailed accounting principle
The rates of exchange of the property *B* with the surroundings ($\dot B_{in}$ and $\dot B_{out}$ ) contain two components each:
* a **transfer term** that represents the rate of exchange of the property **not involving matter**
* a **transport term** that represents the rate of exchange of the property **involving matter**
As such, the fundamental accounting principle can be represented by the following equations:
$$
\dot B_{in} = \dot B_{transfer, in} + \dot B_{transport, in} \tag{2.1}
$$$$
\dot B_{out} = \dot B_{transfer, out} + \dot B_{transport, out} \tag{2.2}
$$

Since the **transport** term involves matter, it can be further expressed in terms of the mass flow rate and the intensive form of the property, which we will denote by the lowercase *b*:
$$\dot B_{transport, in} = (\dot mb)_{in} \tag{2.3}$$
$$\dot B_{transport, out} = (\dot mb)_{out} \tag{2.4}$$
By combining these equations, we can expand Equation 2 into the following:
$$
\frac{dB_{sys}}{dt} = \dot B_{transfer, in} - \dot B_{transfer, out} + (\dot mb)_{in} - (\dot mb)_{out} +\dot B_{gen} - \dot B_{dest} \tag{2.5}
$$
# Dimensions and Units
Dimensions and Units are how we describe the physical state of a system. Dimensions are the traits that a system exhibits and units are how we quantify those traits. 

Units can also help you check if your process is right. If you're expecting an answer in *J* but your answer is in $N*s$, something is probably wrong.