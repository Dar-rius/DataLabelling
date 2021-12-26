# La labellisation des differentes startups de type licornes

L'objectif du projet est de categoriser toutes les start-up ayant une valorisation qui atteint ou depasse les un millard de dollars a fin de leur attribuer des balises, entre 1 et 0, 

1: Pour les start-up dont leur valorisation evolueront tres vite.

0: Pour les start-up dont leur valorisation evolueront lentement.

Pour la realisation de ce projet se sont les donnees du dataset "Unicorn Startup" qui seront utiliser avec 936 lignes et 11 colonnes.

"Image"

Apres avoir chargement du dataset, je passe a l'analyse pour comprendre les donnees du dataset

 "Image"

Apres l'analyse je passe l'etape du preprocessing: j'encode les donnees avec la OdinalEncoder de sklearn, 

"Image"

puis j'utilise la fonction make_pipeline de sklearn a fin d'evite les fuites de donnees, j'entre en parametre les fonctions: MinMaxScaler a fin de standariser les donnees entre le MAximum et le Minimum et je met egalement en parametre la fonction KMeans de sklearn qui qui a fin d'utiliser des cluster pour categoriser les differentes donnees.

"Image"

En suite je cree un dictionnaire "test" qui a comme KEY:"Avenir" et VALUE:"La prediction du model", puis je convertis le dictionnaire "test" pour ensuite le fuisionner au dataset

"Image code"

Ce qui donne ceci: 

"image finale"