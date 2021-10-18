# PC 5

The Petite Classe is divided into three parts. We first study yet another method for numerically integrating ODEs: RADAU5. It consists in an implicit RK scheme with an embedded formula for adaptive time stepping, with some extra properties allowing for an efficient implementation, and was popularized by the group of Hairer and Wanner at the University of Geneva. We return to the van der Pol oscillator to test this method an compare it with others previously introduced in the course. Next, we turn our attention to a specific class of large system of ODEs, obtained from a semi-discretization in space of the heat equation. We discuss the spectrum of the problem and its relation to stiffness, and explain why stabilized Runge-Kutta explicit methods, such as the ROCK4 method, are well adapted for integrating such systems. Finally, we add a reaction term to the heat equation, which generates more interesting dynamics like traveling waves, and approximate the corresponding system appropriate schemes for each part of the equation.

```{note}
The PC statement is available [here](https://moodle.polytechnique.fr/pluginfile.php/318434/mod_folder/content/0/MAP551_PC5_2021_2022.pdf?forcedownload=1)
```
