# PC 4

This Petite Classe is divided into three parts. We first investigate the absolute stability properties of the RK methods as well as some other explicit methods available in the community, such as the Dormand and Price class of methods and draw some stability diagrams in order to properly understand their influence on the performances of the method. The second part is devoted to the integration of the Belousov-Zhabotinsky oscillating reaction. The objective of this second part is two-fold. First, we want to characterize the stiffness of the system of equations and investigate how a standard Runge-Kutta method is dealing with such a stiffness, and what is the impact on the global error. Second, we will use an adaptative embedded Runge-Kutta method in order to experiment with time-step adaptation and clarify the impact of such a numerical strategy at two levels:

1. the size of the time steps and the correspondance with the local stiffness of the dynamics of the system of equations,
2. what is the local error estimate, its link to the effective local error, and finally the resulting global error.

It is essential to have a clear understanding of the various errors as well as a clear picture of the relevance of the local error estimate. Finally, we switch to one of the most difficult and renown test case: the van der Pol oscillator. The purpose is here to extend the study we conducted on the Euler methods in PC 3, and to get a precise idea about the influence of the concepts of absolute stability, accuracy and order, and their response to the presence of stiffness for high order Runge-Kutta methods.

```{note}
The PC statement is available [here](https://moodle.polytechnique.fr/pluginfile.php/318429/mod_folder/content/0/MAP551_PC3_2021_2022.pdf?forcedownload=1)
```
