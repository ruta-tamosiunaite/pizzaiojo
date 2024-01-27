# Projet d'Analyse de Données Pizzaïo’jo

## Contexte du Projet
Ce projet d'analyse de données porte sur un ensemble de données relatives aux commandes de pizzas. L'objectif est d'extraire des informations utiles et de tirer des conclusions significatives à partir de ces données.

## Données Utilisées
Les données utilisées dans ce projet sont extraites d'un ensemble de commandes de pizzas. Elles comprennent des informations telles que les identifiants de commande, les dates, les tailles de pizzas, les catégories de pizzas, les prix unitaires, les quantités commandées, etc.


## 1. Données de Base
### a. Pizzas Uniques
Le jeu de données comprend 91 pizzas uniques (distinctes par pizza_id).

### b. Commandes Uniques
Il y a 21350 commandes distinctes (distinctes par order_id) dans le jeu de données.

## 2. Analyse Temporelle
### a. Plage de Dates
La plage de dates dans le jeu de données va de 2015-01-01 à 2015-12-31.
### b. Commandes par Jour
Le nombre de commandes passées chaque jour varie. La moyenne quotidienne est d'environ 59,64 commandes.
### c. Durée Moyenne de Traitement des Commandes
La durée moyenne pour traiter une commande est 11.02 minutes.
  
Bien qu'il soit délicat de calculer le temps moyen de commande étant donné que l'heure de fin de préparation de la commande n'est pas disponible, nous pouvons avoir une vue globale du temps de commande.

Les résultats identiques ont été obtenus par deux méthodes de calcul:

La première méthode consiste à calculer les intervalles entre les commandes, puis à trouver la moyenne de ces intervalles.
La deuxième méthode implique le calcul du temps de travail quotidien, c'est-à-dire la période entre la première et la dernière commande de la journée, divisé par la somme des écarts de temps entre chaque commande de cette journée. Nous avons opté pour cette dernière approche.

## 3. Analyse de la Quantité
### a. Quantité Moyenne de Pizzas
La quantité moyenne de pizzas commandées est 2.32.
### b. Taille la Plus Fréquemment Commandée
La taille de pizza la plus fréquemment commandée est L.
### c. Catégorie la Plus Fréquemment Commandée
La catégorie de pizza la plus fréquemment commandée est Classic.

## 4. Analyse des Prix
### a. Prix Unitaire Moyen
Le prix unitaire moyen des pizzas est 16.51.
### b. Prix Total Moyen d'une Commande
Le prix total moyen d'une commande est 38.31.
### c. Pizza au Prix Unitaire le Plus Élevé
La pizza au prix unitaire le plus élevé est The Greek Pizza XXL - 35.95.

## 5. Répartition par Taille et Catégorie
Le nombre de pizzas vendues par taille et catégorie varie. Pour plus de détails, référez-vous à l'analyse par taille (pie charts).

## 6. Analyse des Ingrédients
### a. Ingrédients les Plus Couramment Utilisés
Les ingrédients les plus couramment utilisés dans toutes les pizzas sont Garlic, Tomatoes, Red Onions, Red Peppers, Spinach.
### b. Pizzas Contenant un Ingrédient Spécifique
Le nombre de pizzas contenant un ingrédient spécifique Pepperoni est 16.

## 7. Détails de la Commande
La répartition des prix totaux pour les commandes et du nombre de pizzas par commande varie. Pour plus de détails, référez-vous à l'analyse détaillée des commandes (histograms).

## 8. Analyse du Chiffre d'Affaires en Fonction du Temps
### a. Chiffre d'Affaires Quotidien
Le chiffre d'affaires quotidien varie. Pour plus de détails, référez-vous à l'analyse du chiffre d'affaires (bar chart).
### b. Corrélation Heure de la Journée et Total de la Commande
La première vue sur le scatter plot suggère que davantage de pizzas sont vendues pendant l'heure du déjeuner. Cependant, le coefficient de Spearman ainsi que la médiane des boîtes (box plot) indiquent que l'heure de la journée n'a pas d'impact significatif sur les ventes. Il est possible que le regroupement des heures en catégories (matin, déjeuner, après-midi, dîner, soirée) puisse modifier la situation.

## 9. Pizzas Populaires
### a. 5 Pizzas les Plus Commandées en Quantité
Les 5 pizzas les plus commandées en quantité sont Big Meat S, Thai Chicken L, Five Cheese L, Four Cheese L, and Classic Deluxe M.
### b. 5 Pizzas les Plus Commandées en Chiffre d'Affaires
Les 5 pizzas les plus commandées en termes de chiffre d'affaires sont Thai Chicken L, Five Cheese L, Four Cheese L, Spicy Italian L, and Big Meat S.

## 10. Chiffre d'Affaires par Taille et Catégorie
La répartition du chiffre d'affaires pour chaque catégorie et taille de pizza varie. Pour plus de détails, référez-vous à l'analyse du chiffre d'affaires (pie charts)

## 11. Corrélation entre Prix et Quantité
### a. Corrélation Prix Unitaire et Quantité Commandée
Il y a faible corrélation entre le prix unitaire et la quantité commandée.
### b. Prix Unitaire Moyen par Taille de Pizza
Le prix unitaire moyen pour différentes tailles de pizza varie:
S - 12.54
M - 16.01
L - 20.01
XL - 25.50
XXL - 35.95

## 12. Tendances Saisonnières
### a. Tendances Saisonnières dans les Commandes de Pizza
Il y a eu une baisse de chiffre d'affaires au cours des mois de février, septembre et octobre dans les commandes de pizza. Cependant, il est important de noter que le camion à pizza a travaillé moins en octobre, ce qui pourrait potentiellement fausser les résultats. 
### b. Corrélation Jour de la Semaine et Quantité de Commandes
Le test de Kruskal-Wallis est un test non paramétrique utilisé pour déterminer s'il existe des différences statistiquement significatives entre les médianes de trois groupes indépendants ou plus. Dans notre cas, les groupes correspondent aux différents jours de la semaine, et la variable d'intérêt est la quantité de commandes.
  
Dans le résultat, la valeur de p est de 0,423. Cette valeur de p est plus élevée que le niveau de signification typique de 0,05. En statistique, une valeur de p supérieure au niveau de signification suggère que nous ne pouvons pas rejeter l'hypothèse nulle, indiquant l'absence de différence significative dans la médiane de la quantité de commandes entre les différents jours de la semaine. 

Statistiquement, la distribution des quantités de commandes est similaire tous les jours de la semaine.

