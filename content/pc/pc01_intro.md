# PC 1

In this Petite Class we discuss mathematical modeling of explosion phenomena.
When we study the evolution of the chemical composition and of the temperature of a tank filled with fluid energetic material, in order to know if there is a risk of thermal runaway and then of explosion, we can tackle the problem by studying the coupling of hydrodynamics and of the chemistry/thermic associated with the reactions which take place in the medium. However, before turning to a computer for numerical simulations, one has to choose within a hierarchy of simplified systems which takes into account various physical or chemical phenomena; this choice then implies a range of characteristic scales and one must in general have an idea about the mathematical structure of the system and
bring a precise understanding on the dynamics of the system and its qualitative behavior (one works in general in an incompressible limit or weakly thermally compressible written by the equations of Oberbeck-Boussinesq), before being able to simulate it. However, this understanding is based on two key ingredients:

1. knowing how to identify the right modeling hypotheses allowing to conduct a rapid and relevant analysis of qualitative behavior and therefore to work with the right level of modeling,
2. knowing the theory of dynamical systems in order to understand the possible behavior of the system under consideration.


```{note}
The PC statement is available [here](https://moodle.polytechnique.fr/pluginfile.php/318424/mod_folder/content/0/MAP551_PC1_2021_2022.pdf?forcedownload=1).
```

<!-- #region -->
## Historical notes

The theory of the thermal explosion originates from the work of Nikolay N. Semenov, who even though he is a chemist, worked at the interfaces of disciplines (mathematics, physics,...) in the spirit of the pure Russian tradition.

```{image} ../images/semenov.jpg
:alt: Semenov
:width: 300px
:align: center
```

>**Nikolay Nikolayevich Semyonov** (1896-1996) : 
>In the laboratories of the professor Boris Veinberg there worked  Nikolay Semenov, the future Nobel Prize winner for physical chemistry (1956). He was born in Saratov (1896), graduated from the Saratov Realschule and joined the Math Branch of the Math and Physics Department at Petrograd Imperial University. After graduation, he stayed at the university as a professorial fellow.

His work covers mainly the study of chemical transformation mechanisms and in particular an exhaustive study of the theory of chain reactions, with applications in particular to combustion processes.

```{image} ../images/stele_semenov.jpg
:alt: Semenov Stele
:width: 300px
:align: center
```

>In the spring of 1918 Semenov went on vacation to his parents in Samara, where he was called to arms to the Kolchak White People’s Army. After doing his service for 3 weeks, he deserted and moved to Tomsk, which was the nearest city with a university. Until 1920 Nikolay Semenov did postgraduate studies in the Tomsk Institute of Technology, and then he returned to Petrograd.
In 1931 he established the Institute of Chemical Physics of Russian Academy of Science (ICP RAS) and stayed as its irreplaceable director until the end of his days. Together with the Soviet physicist Pyotr Leonidovich Kapitsa, Nikolay Semenov founded the Moscow Institute of Physics and Technology in 1946.
Nikolay Semenov was the only Soviet physicist and chemist who was awarded the Nobel Prize.

The second name associated with the theory of the thermal explosion is the one of David A. Frank-Kamenetskii. Invited by Semenov to whom he had sent a letter on chemical thermodynamics, he worked for seven years from 1934 to 1941 at the Institute of Physical Chemistry of the Russian Academy of Sciences founded by Semenov, where he worked on the problems of thermal explosion and met another figure of the Russian combustion community: Yakov Borisovich Zel'dovich, with whom he would become very friendly.


```{image} ../images/kamenetskii.jpg
:alt: Frank-Kamenetskii
:width: 200px
:align: center
```
  
>**David Albertovich Frank-Kamenetskii** (1910-1970): 
>He was a Soviet theoretical physicist and chemist, professor and doctor of physical, chemical and mathemetical sciences. He developed the thermal explosion theory, worked on plasma physics problems and in astrophysics.
<!-- #endregion -->
