## Classification musicale 
## Méthode des k plus proches voisins avec Scikit-Learn

### Auteur :
* Akilhoussen Houzefa Onaly

### Enseignant encadrant : 
* M. Emmanuel DELLANDREA

## Jeu de données

Les données sont divisées en deux sous-ensembles : un sous-ensemble d’apprentissage   
et un sous-ensemble de test, reconnaissables par l’extention _app et _test,   
respectivement pour les données d’apprentissage et de test.  
Pour chacun de ces sous-ensembles, les données suivantes sont fournies :  
noms : vecteur contenant le nom des titres musicaux  
* classes : vecteur contenant un entier identifiant le genre musical de chaque titre  
	* 1 : classique
	* 2 : disco
	* 3 : jazz
	* 4 : rock
* donnees : matrice contenant les données audio. Chaque ligne correspond à un titre musical,  
et les valeurs en colonnes correspondent aux valeurs d’amplitude brutes du signal sonore.  

Chaque morceau de musique dure 1 seconde et est échantillonné à 44 khZ.  

## Descripteurs utilisés et méthode

Pour chaque musique, on extrait 4 descripteurs à partir de l'enveloppe d'énergie :
* le centroïde temporel 
* la durée effective
* l’énergie globale
* le taux de passage par zéro

On applique ensuite la méthode des k plus proches voisins pour classifier les musiques test.

## Résultats 

Précision de 62.5 % atteinte avec k=3

## Conseils d'utilisation

Vous pouvez utiliser le programme en utilisant vos propres données et modifier le code en conséquence.    
Vous pouvez également utiliser d'autres descripteurs et rajouter des genres.  

## Screenshot 
![ ](https://i.ibb.co/Yc9R14p/Capture.png)
