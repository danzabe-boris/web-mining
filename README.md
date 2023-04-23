# Readme

## Web Scraping du classement FIFA de l'équipe du Cameroun

Le script Python présent dans ce repository permet de réaliser du web scraping sur le site Wikipédia afin d'extraire les informations sur le classement FIFA de l'équipe de football du Cameroun.

Pour ce faire, le code utilise les bibliothèques urllib et bs4 pour récupérer le contenu de la page HTML et extraire la table contenant les informations de classement.

Les données sont ensuite stockées dans un dataframe pandas pour pouvoir être utilisées pour la classification.

## Classification des données

Le script utilise la bibliothèque scikit-learn pour effectuer une classification des données en utilisant deux modèles différents : Naïve Bayes et KNN.

Le code divise les données en deux ensembles : un ensemble d'apprentissage (70% des données) et un ensemble de test (30% des données).

Le modèle Naïve Bayes est entraîné sur l'ensemble d'apprentissage en utilisant la fonction GaussianNB de scikit-learn.

Le modèle KNN est entraîné sur l'ensemble d'apprentissage en utilisant la fonction KNeighborsClassifier de scikit-learn. Une recherche de grille est effectuée pour trouver le meilleur nombre de voisins à utiliser dans le modèle.

Des matrices de confusion sont ensuite générées pour les deux modèles en utilisant la fonction plot_confusion_matrix de scikit-learn.

## Prérequis

Ce script nécessite l'installation des bibliothèques suivantes :

- pandas
- numpy
- sklearn
- seaborn
- matplotlib

## Utilisation

Le script peut être utilisé en exécutant le fichier "main.py". Il est conseillé de le faire dans un environnement virtuel Python pour éviter les conflits de versions de bibliothèques.

Le script affichera les matrices de confusion pour les deux modèles.
