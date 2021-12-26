# La labellisation des differentes startups de type licornes

L'objectif du projet est de catégoriser toutes les start-up ayant une valorisation qui atteint ou dépasse les un milliard de dollars afin de leur attribuer des balises, entre 1 et 0.

1: Pour les start-up dont leur valorisation évoluent très vite;

0: Pour les start-up dont leur valorisation évoluent lentement.

Pour la réalisation de ce projet se sont les données du dataset "Unicorn Startup" qui seront utilisées avec 936 lignes et 11 colonnes.

![alt text]()

Apres l'analyse des donnes du dataset, je passe a l'etape suivante le preprocessing: j'encode les donnees avec la OdinalEncoder de sklearn, j'utilise la fonction make_pipeline de sklearn afin d'éviter les fuites de données, j'entre en paramètre les fonctions: MinMaxScaler afin de standardiser les données entre le MAximum et le Minimum et je met également en paramètre la fonction KMeans de sklearn qui qui a fin d'utiliser des cluster pour catégoriser les différentes données.

En suite je convertis la sortie du modele qui en tableau numpy en dictionnaire avec comme nom de variable: "test" qui a comme KEY:"Avenir" et VALUE:"La prediction du model", ensuite  je convertis le dictionnaire "test" en DataFrame en le nommant “predire” pour ensuite le fusionner au premier DataFrame “data” et le seconde “predire”.

Ce qui donne ceci:

![alt text]()
