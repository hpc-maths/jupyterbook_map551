# Mode d'emploi pour l'exécution des notebooks Jupyter

Afin de pouvoir exécuter les notebooks mis à disposition pour les cours et les pc, trois possibilités sont possibles :

## Utiliser son environnement personnel

Pour ce mode, il suffit de télécharger les notebooks Jupyter depuis ce site et les exécuter sur sa machine. Pour installer l'environnement logiciel nécessaire à l'exécution des notebooks du cours, suivre la procédure suivante.
  
```{admonition} Procédure pour installer Jupyter Notebook

- Installer la dernière version de miniconda contenant Python 3 (disponible sur https://conda.io/miniconda.html).
  Si vous avez déjà installé une version de miniconda ou d'anaconda, vous pouvez mettre à jour votre installation en tapant dans un terminal ou dans l'Anaconda Prompt (sous Windows) la commande :

`conda update conda`


- Créer un nouvel environnement pour le cours :

`conda create -n map551 python=3`


- Activer l'environnement map551 :

`conda activate map551` 


-  Installer les packages python nécessaires pour le cours :

`conda install jupyter jupyterlab numpy scipy plotly`


-  Lancer le serveur Jupyter :

`jupyter notebook` ou `jupyter lab`
```

## Utiliser le JupyterHub de l'école

Pour ce mode, il suffit de télécharger les notebooks Jupyter depuis ce site et les copier vers le serveur `JupyterHub` de l'école (cf. procédure suivante).

```{admonition} Utilisation du JupyterHub de l'école

- Dans un navigateur, se rendre sur le site https://jupytercloud.idcs.polytechnique.fr/ et cliquer sur le lien `jupyter` puis sur le bouton `Sign in with CNRS/INSMI/Mathrice OpenID-Connect Provider`


- Sélectionnez l'établissement Ecole Polytechnique Palaiseau puis utiliser vos identifiants de polytechnique pour vous connecter sur la plateforme


- Sur la page `Server Options`, cliquer dans le rectangle MAP551 ce qui permet de lancer un `JupyterLab` avec l'ensemble des modules necessaires au cours


- Cliquer sur l'icone `Upload files` du menu de la barre latérale gauche pour téléverser un notebook de votre machine vers le `JupyterLab` puis l'exécuter


- Récupérer un notebook depuis la plateforme vers votre machine en cliquant avec le bouton droit sur le nom du notebook dans la barre latérale gauche puis en choisissant `download`


- Remarque : déplacer vos notebooks dans le répertoire `persistent` afin qu'ils soient conserver pour une prochaine session  
``` 

## Utiliser Binder

Binder propose de déployer un environnement Jupyter accessible en ligne, sans aucune installation, à partir d’un dépôt git contenant des notebooks.
Pour lancer les notebooks du cours, il suffit de cliquer sur le lien binder présent sur chaque page du site proposant un notebook. 

Remarque : l'environnement Jupyter est supprimé lorsque que la session se termine, pensez à télécharger le notebook sur votre machine si vous souhaitez le garder. 
