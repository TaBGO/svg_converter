# convertisseur sb3/svg

Ce projet convertit les sorties produites par les programmes scratch (SB3) en fichier SVG (Scable Vector Graphics)

## usage standalone
Pour utiliser le convertisseur, il suffit d'exécuter le fichier *convertor.py* avec au moins un argument : le nom du fichier sb3 à convertir.

``python convertor.py <sb3-file>
``
Le fichier *result.svg" est créé dans le répertoire courant en utilisant un trécé simple. 

Plusieurs arguments peuvent être utilisés dans l'ordre suivant : 
* **redimensionnement** : ajuste la taille de la figure (*valeur entière*) 
* **translation en x** : indique le nombre de pixels de décalage de la figure en x (*valeur entière*) 
* **translation en y** : indique le nombre de pixels de décalage de la figure en y (*valeur entière*) 
  
``python convertor.py <sb3_file> <scale> <translation_x> <translation_y>
``

Si la valeur de redimensionnement est supérieure à 1, alors le rendu est adapté automatiquement pour le robot [ozobot](https://ozobot.com).

## usage avec TabGO
Il est aussi possible d'utiliser directement le convertisseur avec le lecteur **TabGO**. A l'issue de la reconnaissance du code, le fichier svg est produit automatiquement.


*Ce convertisseur a été développé par [Noémie Guiraud](https://github.com/NoemGir)*
