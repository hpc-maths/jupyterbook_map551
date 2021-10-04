# Systèmes dynamiques pour la modélisation et la simulation des milieux réactifs multi-échelles

Dans un nombre croissant d’applications scientifiques et industrielles, la modélisation et la simulation numérique jouent un rôle clef pour comprendre et analyser les phénomènes physiques complexes mis en jeu. Un élément commun à ces systèmes énergétiques, spatiaux, biologiques, mécaniques, fluides, etc... tourne autour de la notion de systèmes dynamiques. En mathématiques, un système dynamique est la donnée d’un système et d’une loi décrivant l’évolution de ce système dans le temps. Ces systèmes sont particulièrement multi-échelles, c’est-à-dire qu’ils impliquent une très large variété d’échelles en temps, voire d’espace. Ils posent alors de nombreuses difficultés si l’on veut les analyser et en faire une résolution numérique précise afin de disposer d’outils fiables de prédiction de leur dynamique. 

Dans le champ mathématique, l’étude des systèmes dynamiques est un domaine particulièrement riche et passionnant depuis les travaux d’H. Poincaré jusqu’aux travaux plus récents sur les systèmes dynamiques chaotiques en passant par l’étude des points critiques, de leur stabilité et l’analyse des bifurcations qui touche à la géométrie différentielle.

Ce cours a été conçu pour donner une base tant au niveau de la modélisation (compréhension de ce qu’est une hiérarchie de modèles à différentes échelles), que de l’analyse théorique et de l’analyse numérique. Il s’agit de maîtriser un ensemble d’outils et d’être capable de conduire une analyse complète de systèmes dynamiques issus d’un vaste champ d’applications. Nous proposons d’identifier les enjeux en termes mathématiques afin de comprendre et d’analyser la dynamique de ces systèmes en dimension finie, voire d’en proposer une simulation précise, fiable et prédictive. 

Nous étudierons des exemples dans de nombreux domaines d’application comme la combustion, la mécanique des fluides, la dynamique des populations, la dynamique chimique non-linéaire, le génie biomédical ou la physique des plasmas, que l’on rassemble sous le vocable de “milieux réactifs" (un milieu impliquant plusieurs “espèces" qui “réagissent" entre elles avec un certain niveau de complexité impliquant un large spectre d’échelles de temps, voire d’espace). 

Les domaines sur lesquels le cours donnera une expertise sont : analyse mathématique, schémas numériques pour les systèmes d’équations différentielles, analyse de la stabilité des systèmes - bifurcation, implémentation numérique et bibliothèques de programmes permettant la simulation numérique ou l’analyse de bifurcations. Des applications sur machines permettent une analyse de la dynamique mais aussi une compréhension des schémas numériques à la base d’une simulation précise et robuste, ainsi qu’une ouverture sur les enjeux du calcul haute performance. L’ensemble des petites classes se fait au moyen de notebooks Jupyter, ce qui permet une familiarisation avec les concepts et les méthodes numériques particulièrement efficace, puis d’analyser les résultats en termes des applications. L’ensemble des techniques proposées sera illustré sur des exemples simples mais symptomatiques des enjeux des systèmes complexes rencontrés dans les véritables applications. Un mini-projet permet de mettre en œuvre les notions et méthodes enseignées et de se confronter à des systèmes appliqués dans un large spectre de domaines applicatifs.


Le cours ne demande pas de pré-requis et se situe dans le cadre des départements de Mathématiques APpliquées (MAP) et de Mécanique (MEC) de l’Ecole polytechnique. Il s’inscrit dans le cadre du parcours MAP-MECA et est offert dans le cadre du PA Sciences et Défis du Spatial.

L’évaluation se fait sous la forme d’un contrôle continu par évaluation de comptes rendus de Travaux Pratiques (6 CRTP - 2/3 note finale). L’évaluation finale sous la forme d’un mini-projet en binôme et d’une soutenance (1/3 note finale). 

L’équipe pédagogique est constituée de M. Massot (Cours), M. Breden (PC), L. Séries (Jupyter) et A. Loison (Mini-projets et CRTP).

## Dynamical Systems for the modeling of multi-scale reactive media

In a growing number of scientific and industrial applications, modeling and numerical simulation play a key role in understanding and analyzing the complex physical phenomena involved. A common element to these energetic, spatial, biological, mechanical, fluid systems, etc... revolves around the notion of dynamical systems. In mathematics, a dynamical system consists in a system and a law describing the evolution of this system in time. These systems are particularly multiscale, that is to say that they involve a very large variety of scales in time and even space. They pose many difficulties if we want to analyze them and make a precise numerical resolution in order to have reliable tools for predicting their dynamics. 

In the mathematical field, the study of dynamical systems is a particularly rich and exciting area, from the work of H. Poincaré to the more recent work on chaotic dynamical systems, including the study of critical points and their stability, and the analysis of bifurcations, which touches on differential geometry.

This course has been designed to provide a foundation in modeling (understanding what a hierarchy of models at different scales is), theoretical analysis and numerical analysis. The aim is to master a set of tools and to be able to conduct a complete analysis of dynamic systems from a wide range of applications. We propose to identify the issues at stake in mathematical terms in order to understand and analyze the dynamics of these systems in finite dimension, and even to propose an accurate, reliable and predictive simulation. 

We will study examples in many fields of application such as combustion, fluid mechanics, population dynamics, nonlinear chemical dynamics, biomedical engineering or plasma physics, which are grouped under the term "reactive media" (a medium involving several "species", which "react" with each other, with a certain level of complexity involving a wide range of time and even space scales) 

The areas in which the course will provide expertise are: mathematical analysis, numerical schemes for systems of differential equations, stability analysis of systems - bifurcation, numerical implementation and libraries of programs for numerical simulation or bifurcation analysis. Applications and simulation on computers allow an analysis of the dynamics but also an understanding of the numerical schemes at the basis of an accurate and robust simulation, as well as an opening on the stakes of high performance computing. All the Petite Classes rely on Jupyter notebooks, which allow a particularly effective familiarization with the concepts and numerical methods, and then to analyze the results in terms of applications. All the techniques proposed will be illustrated on simple examples but symptomatic of the stakes of complex systems encountered in real applications. A mini-project will allow the students to implement the notions and methods taught and to be confronted with systems applied in a wide range of application domains.


The course does not require any pre-requisites and is part of the Applied Mathematics (MAP) and Mechanics (MEC) departments of the Ecole Polytechnique. It is part of the MAP-MECA track and is offered as part of the PA Sciences et Défis du Spatial.

The evaluation is done in the form of a continuous assessment by evaluation of reports of practical work (6 CRTP - 2/3 of final grade). The final evaluation in the form of a mini-project in pairs and a defense (1/3 final grade). 

The pedagogical team is composed of M. Massot (Courses), M. Breden (PC), L. Séries (Jupyter) and A. Loison (Mini-projects and CRTP).


### Bibliographie Mathématique :

- J.P. Demailly, Analyse numérique et Equations différentielles, Presses Universitaires de Grenoble (1996)
- J. Guckenheimer, P.J. Holmes, Nonlinear Oscillations, Dynamical Systems, and Bifurcation of Vector Fields, Applied Mathematical Sciences Vol 42, Springer (1983)
- E. Hairer, S.P. Nørsett, G. Wanner,  Solving Ordinary Differential Equations I - Nonstiff Problems, Springer Series in Computational Mathematics (1993)
- E. Hairer, G. Wanner,  Solving Ordinary Differential Equations II - Stiff and Differential-Algebraic Problems, Springer Series in Computational Mathematics (1996)
- E. Hairer, C. Lubich and G. Wanner, Geometric Numerical Integration, Structure-Preserving Algorithms for Ordinary Differential Equations, 2nd edition, Springer Verlag, Berlin (2006)
- S. Wiggins, Ìntroduction to Applied Nonlinear Dynamical Systems and Chaos, Texts in Applied Mathematics, Springer (2003)
- M. Duarte, Méthodes numériques adaptatives pour la simulation de la dynamique de fronts de réaction multi-échelles en temps et en espace, Thèse de Doctorat de l'Ecole Centrale Paris (2011) sur TEL

### Bibliographie Appliquée :

- I.R. Epstein and J.A. Pojman, An Introduction to Nonlinear Chemical Dynamics: Oscillations, Waves, Patterns and Chaos, Oxford University Press (1998)
- Ya.B. Zeldovich, G.I. Barenblatt, V.B. Librovich, G.M.  Makhviladze, The Mathematical Theory of Combustion and Explosions, Consultant Bureau (1985)
- P. Gray, S.K. Scott, Chemical Oscillations and Instabilities: Non-linear Chemical Kinetics, International Series of Monographs in Chemistry - 21, Clarendon Press, Oxford (1994)
- P. Manneville, Instabilité, Chaos et Turbulence, Les éditions de l'Ecole polytechnique (2004)
- V. Giovangigli, Multicomponent Flow Modeling, Modeling and Simulation in Science, Engineering and Technology Series, Birkhäuser (1999)
- P. Holmes, J. Lumley, G. Berkooz, C.W. Rowley, Turbulence, coherent structures, dynamical systems and symmetry. Second edition. Cambridge Monographs on Mechanics. Cambridge University Press (2012)

