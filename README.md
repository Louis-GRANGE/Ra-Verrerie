# Ra-Verrerie
 Projet de verrerie 
Problématique :  Faire une application pour un restaurant pour prévisualiser des collections de verres (4 types de verres différents, eau, vin, cocktail, bière,... plusieurs collections) et des carafes.  
 
Nous allons développer une application mobile (android) permettant de faire tourner l’application en réalité augmentée afin de visualiser les verres et carafes. 
 
L’utilisateur doit placer les marqueurs de différents types de verres/carafes (eau, vin, cocktail, bière,...) ou il souhaite voir apparaître le verre, puis il va pouvoir les visualiser grâce à son téléphone en pointant la caméra sur l’image. 
 
Pour changer de collection de verre il faudra cliquer sur des boutons dans l’UI, et les verres changeront pour appartenir à la nouvelle collection. (aucun changement de marqueurs physiques n’est nécessaire pour changer de collection)  
 
L’accès à la caméra de l’appareil sera demandé pour utiliser l’application. 
 
Les marqueurs (images physiques d’un verre) seront en noirs et blanc pour une meilleur efficacité. 
 
Possibilité de faire tourner les verres et les carafes en cliquant à droite et à gauche sur l’écran. 
 
Point fort :  - La reconnaissance des marqueurs est rapide et fiable. 
 
Points faibles : - Demande des marqueurs physiques des différents verres pour fonctionner.  - Connection internet obligatoire pour que l’application fonctionne 
 
Recommandation : Placer toutes les marqueurs physiques de verres, puis observer les différentes collections en cliquant sur les boutons dans l’UI sans retoucher les marqueurs physiques. 
 
Vous pouvez voir différents verres de différentes collections aux mêmes endroits seulement en cliquant sur le bouton de la collection souhaité. 
 
 
Technologies : Unity3D + Vuforia Compilation pour Android Compilation possible pour PC  
 
Modèles 3D : Modélisés sur 3DS Max 



Partie technique avancée : 

 Les 3 boutons en haut permettent de changer de collection, c'est le script UISwap.cs dans assets/ressource qui change les modèles 3D sur le click des boutons
 
 Cliquer sur un bouton fera aussi apparaitre un autre menu permettant de comparer une collection avec une autre (script dans assets : SwapButton.cs, CompareScript.cs ActiveComparObjects.cs) 
 
La comparaison prendre la modèle actuel et celui cliqué par le nouveau boutton, nous verrons les 2 modèles 3D en même temps.

Le bouton Hidden/Show en bas permet d'activer un petit UI au dessus des verres, il indiquera la collection du verre, très utile pendant les comparaisons pour savoir à quel collection appartiennent les verres affichés (script  ui : TextMeshLook.cs dans assets/scenes, bouton : ToggleText.cs dans assets/scenes)

Pour la réalité augmentée utilisation de Vuforia engine et des database.

 
 
 
