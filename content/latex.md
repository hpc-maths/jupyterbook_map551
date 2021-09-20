# Rédaction de compte rendu avec LaTeX

Dans le cadre de MAP551, il est demandé de faire des compte-rendus des différents TP et, la manière la plus simple de les rédiger est d'utiliser des éditeurs de texte scientifique tels que $\LaTeX$. Cela permet de rédiger des documents clairs et, pour ceux qui ne l'ont jamais utilisé, ce sera une occasion d'acquérir et développer un outil essentiel pour la suite (stages, mémoires, recherche, rapports, ...). Même si son utilisation n'est pas obligatoire pour MAP551, il est fortement suggéré d'utiliser $\LaTeX$. Vous ne serez pas pénalisé pour un défaut de connaissance de $\LaTeX$ et je vous encourage à vous documenter au fur et à mesure ou de me poser des questions via mon mail : *arthur.loison@polytechnique.edu*.


## Qu'est ce que $\LaTeX$ ?

$\LaTeX$  est un éditeur de texte adapté à la rédaction de document scientifiques (articles, livres, rapport) qui permet de faciliter, entre autres la rédaction de formules mathématiques et de la mise en page.

Le principe est de rédiger/coder un document utilisant les normes de $\LaTeX$ : balises et environnements tels que `section`, `equation`, `align`, `figure`, `table`, ...


## Par où commencer ?

La façon la plus simple d'utiliser $\LaTeX$ est d'utiliser des logiciels gratuits tels que Overleaf (en ligne via un navigateur web) ou de télécharger un éditeur (TeXStudio ou autre).


### Overleaf

Rendez-vous sur *Overleaf.com*, connectez-vous/créez-vous un un compte. Dans la barre de gauche, sélectionnez "New project" puis dans le menu déroulant "Example project".

Une page s'ouvre avec, à gauche, le code $\LaTeX$ dans un fichier ".tex", et, à droite, le rendu en PDF.

Il suffit alors de compiler le code pour obtenir le PDF correspondant.


### Autres éditeurs

Télécharger et installer un éditeur sur votre ordinateur, démarrer un nouveau document dans un dossier de votre choix en sélectionnant un template de votre choix du type `article`, `report` ou autre. De manière identique, le code et le rendu PDF sont proposés dans deux fenêtres différentes et il ne reste plus qu'à compiler le code pour obtenir le fichier PDF (que vous retrouverez dans le dossier où vous travaillez).


## Premiers pas avec $\LaTeX$

Une tonne de livres très complets (je peux vous en faire passer un par mail si vous le souhaitez) ou de tutoriels gratuits sont disponibles sur internet pour découvrir (par exemple sur le site d'Overleaf), apprendre et se perfectionner en $\LaTeX$. L'essentiel consiste à partir d'une base assez simple comme décrite dans l'exemple de projet d'Overleaf et de réutiliser les morceaux de codes déjà inscrits, la mise en page par défaut de $\LaTeX$ suffit à la clarté d'un rapport. Les subtilités de mise en page $\LaTeX$ peuvent s'avérer difficile à maîtriser et sont réservées à des utilisateurs expérimentés. Je vous propose néanmoins les outils de bases qui seront nécessaires à votre rapport dans ce document ainsi qu'un document avec la liste des raccourcis utiles.

<!-- #region -->
### Les packages

Avant toute chose, $\LaTeX$ est un language enrichi par de nombreux packages qui permettent pleins de fonctionnalités intéressantes (bibliographie, langues, références, insertion d'images, symboles mathématiques supplémentaires, mise en page, ...) et sont insérés en début de document via des balises du type : 

```latex
\usepackage{NomDuPackage},
```

Que ce soit sur Overleaf ou dans les autres éditeurs, ces packages sont alors téléchargés au moment de la compilation du code.

Je vous conseille donc d'insérer les packages suivants `graphicx` (pour insérer des images), `amsmath` et `amssymb` (nombreux symboles mathématiques utiles). Si une commande que vous souhaitez utiliser ne fonctionne pas, assurez vous d'avoir déclarer le package dans l'en-tête.
<!-- #endregion -->

<!-- #region -->
### Le texte

Le texte s'organise via les balises 

```latex
\section{Titre de la section}
```

ainsi que 

```latex 
\subsection{Titre de la sous-section}
```

et 

```latex
\subsubsection{Titre de la sous-sous-section}  
```

pour l'organisation en parties, sous-parties et sous-sous parties.

Le texte brut s'écrit, lui directement entre ces balises.
<!-- #endregion -->

<!-- #region -->
### Les formules mathématiques

Pour écrire des symboles mathématiques, il y a plusieurs méthodes :

1. Formule au sein du texte en utilisant `$Votre formule$` e.g. : `$\int_0^1 x^2 dx = \frac{1}{3}$` donne $\int_0^1 x^2 dx = \frac{1}{3}$
        
2. Avec un retour à la ligne et centré via : `$$\int_0^1 x^2 dx= \frac{1}{3}$$` qui donne 

$$\int_0^1 x^2 dx= \frac{1}{3}$$

3. Idem que le point précédent mais à privilégier, via 
```latex
\begin{equation*} 
\int_0^1 x^2 dx= \frac{1}{3}
\end{equation*}
```
ce qui donne 
\begin{equation*} 
\int_0^1 x^2 dx= \frac{1}{3}
\end{equation*}

4. Une suite d'équation alignée avec `align` e.g. : 
```latex
\begin{align*}
\int_0^1 x^2 dx &= \frac{1^3}{3}-\frac{0^3}{3}\\
                &= \frac{1}{3}.
\end{align*}
```

ce qui donne :

\begin{align*}
\int_0^1 x^2 dx &= \frac{1^3}{3}-\frac{0^3}{3}\\
                &= \frac{1}{3}.
\end{align*}

La liste des symboles mathématiques en $\LaTeX$ est disponible un peu partout sur internet.
<!-- #endregion -->

<!-- #region -->
### Les images

Pour insérer des images, notamment des courbes exportées des notebooks Jupyter ou autres, je vous conseille d'ouvir un environnement `figure` via :
```latex
\begin{figure} 
\includegraphics[width=largeur]{nomdufichier}
\caption{Titredelafigure}
\end{figure} 
```
où `nomdufichier`est le nom du fichier à ajouter et `Titredelafigure` le contenu de la légende.

Vous pouvez laisser à $\LaTeX$ le choix du lieu de l'affichage de l'image ou bien vous pouvez le forcer à l'afficher entre les paragraphes de textes où vous avez déclarer l'environnement `figure` via l'option `h!` via `\begin{figure}[h!]`.
<!-- #endregion -->

<!-- #region -->
### Les tableaux

Pour insérer un tableau, je vous conseille d'utiliser un environnnement `table` et un sous-environnement `tabular`. Les colonnes du tableaux se déclarent via des lettres via `$\begin\{figure\}{c|lrc}` où l'on a par exemple un tableau de 4 colonnes, la première étant centrée, séparée par une ligne verticale des autres puis trois colonnes alignées à gauche `l`, à droite `r` puis centrée `c`.

Une ligne du tableau se déclare case par case séparée par `&` et le retour à la ligne par `\\`. 

Exemple de tableau :
```latex
\begin{table}[h!]
        \centering
        \begin{tabular}{c|lrc}
                1 & 2 & 3 & 4\\
                \hline
                5 & 6 & 7 & 8
        \end{tabular}
        \caption{Un exemple de tableau.}
        \label{tab:exemple}
\end{table}
```

Les traits horizontaux se déclarent via `hline`.


<!-- #endregion -->

### Les références

Les références permettent de lier automatiquement le numéro d'une image, d'un tablea ou d'une équation même après réarrangement dans l'ordre de déclaration, de suppression ou d'ajout d'un nouvel élément. Cela permet de faire des références sans se soucier de vérifier la correspondance des chiffres des figures.

Pour cela, il suffit de labelliser les environnements via la balise `\label{votreLabel}` et d'y faire référence dans le texte via `\ref{votreLabel}`. Afin de s'y retrouver dans les labels, je vous conseille d'utiliser des labels courts ou de les commencer par `fig:...`, `tab:...`, `eq:...` afin de reconnaitre le type d'élémént auquel on fait référence.


## $\LaTeX$ Cheat Sheet

Vous trouverez un résumé en deux pages des principales commandes $LaTeX$ [ici](https://wch.github.io/latexsheet/latexsheet.pdf).


### Le mot de la fin

$\LaTeX$ est un language très utilisé, très documenté et pour lequel on trouve toutes les réponses sur internet, des questions les plus basiques au plus techniques. Même si cela prend du temps au début, vous trouverez rapidement vos marques et l'effort demandé sera de moins en moins élevé.
