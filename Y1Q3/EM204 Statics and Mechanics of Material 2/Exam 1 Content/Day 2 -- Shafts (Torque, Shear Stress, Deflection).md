# Learning Objectives
1. Draw a torque diagram and determine the maximum torque in a shaft
2. List factors that need to be considered in the design of a shaft
# Terminology
## Torque
A torque is a rotation affect created by a force applied a distance from a pivot, or a twist created by a pure moment created by any twisting motion
$$\overrightarrow \tau = \overrightarrow F \times \overrightarrow r$$
## Moment
A moment is the rotation effect caused by a force applied a distance from a pivot
$$\overrightarrow M = \overrightarrow F \times \overrightarrow r$$
## Couple
A couple is the moment created by two equal and opposite forces that are co-planar

# Shafts
## What is a shaft?
A shaft is a slender machine component subject to axial twisting moments or torques. We are interested in the strength characteristics of the shaft, so we ignore any angular velocities, the weight of the shaft, bearing reactions, etc.
## Some examples of shafts
Screwdrivers, Electric motors, driveshafts, torsional springs, tool shafts, drill bits, bolts/screws
## What information would you need to design a shaft?
weight, power/torque output, material choice (strength, stiffness, manufacturability), dimensional restrictions, cost restrictions, operating conditions
## How do we predict the possible location of failure?
Find where the maximum amount of torque experienced is via a torque diagram and using said diagram to find the magnitude and location of the maximum experienced torque.

# Torque Diagrams
## What is a torque diagram?
A torque diagram is a figure that displays how much torque shaft experiences in a given region. It is helpful to see where the maximum and minimum loads are experienced.
## How do you draw a torque diagram?
Start with a FBD. Use the RHR to establish positive/negative torques and draw the entire shaft. Then divide the shaft into smaller regions between the points of applied torque and draw smaller, individual FBDs for each region. Establish a torque "exiting" the shaft as an unknown and have that "exit" torque go into the next region. Starting on the end of the shaft with the least unknowns, solve equilibrium equations. Recall that this is statics, so the sum of all forces must be 0:
$$\Sigma \overrightarrow M_{o} = 0$$Thus, all of the torques in each segment of the shaft must sum to 0. Use this to find your unknowns. Repeat until you have analyzed the entire shaft. 

After you have found the torques in each region, you will plot all of these torques on a graph. Starting at one end, draw a horizontal line representing the experienced torque in each section (the unknown that was solved for). Repeat this process for each torque in the shaft and connect the ends with vertical lines. The horizontal line with the largest displacement from the neutral axis is the point of highest torque in the shaft. 
