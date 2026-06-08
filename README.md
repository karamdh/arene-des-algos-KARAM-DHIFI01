Projet fil rouge de la semaine ML (IPSSI). Objectif : comparer plusieurs algorithmes de Machine Learning sur différents datasets et justifier le choix du meilleur.

Programme
J1 : Pipeline supervisé + non-supervisé, première Arène
J2 : Nettoyage de données
J3 : Arsenal complet des algos
J4 : Réseaux de neurones, évaluation, déploiement
J5 : Projet groupe + soutenance

# Arène des Algorithmes - KARAM DHIFI

## Objectif du projet

L'objectif de ce projet est de comparer plusieurs algorithmes de Machine Learning sur différents jeux de données afin d'identifier leurs forces, leurs limites et leur comportement selon le contexte.

Le projet a été réalisé en suivant les principales étapes d'un pipeline de Machine Learning :
- Exploration des données
- Préparation des données
- Entraînement des modèles
- Évaluation des performances
- Comparaison des algorithmes
- Analyse des résultats


## Datasets utilisés

### 1. Breast Cancer Dataset
Dataset médical contenant 569 observations et 30 caractéristiques décrivant des cellules tumorales.

Objectif :
Prédire si une tumeur est :
- Maligne
- Bénigne

### 2. Wine Dataset
Dataset contenant 178 observations et 13 caractéristiques chimiques.

Objectif :
Classer les vins dans l'une des 3 catégories disponibles.

---

## Algorithmes comparés

- Logistic Regression
- Random Forest
- K-Nearest Neighbors (KNN)
- Decision Tree
- KMeans (clustering non supervisé)

---

## Phase 1 : Exploration des données

Analyse de la structure des datasets :
- nombre de lignes
- nombre de colonnes
- répartition des classes

Tests réalisés :
- cas normal
- cas limite
- cas déséquilibré

Cette étape a montré que l'accuracy seule peut être trompeuse lorsque les classes sont déséquilibrées.

---

## Phase 2 : Classification supervisée

Mise en place d'un pipeline de Machine Learning :

- séparation train/test
- normalisation des données
- entraînement des modèles
- évaluation par accuracy

---

## Phase 3 : Arène des algorithmes

Comparaison des modèles sur le même découpage train/test afin de garantir une comparaison équitable.

Exemple de classement obtenu :

1. Logistic Regression
2. KNN
3. Random Forest
4. Decision Tree

---

## Phase 4 : Clustering non supervisé

Utilisation de KMeans sans fournir les étiquettes.

Objectif :
Déterminer si les données possèdent naturellement une structure proche des classes réelles.

Comparaison réalisée avec les vraies étiquettes grâce à l'Adjusted Rand Index (ARI).

---

## Phase 5 : Changement de dataset

Réutilisation de la fonction d'arène sur le dataset Wine.

Objectif :
Vérifier que le pipeline fonctionne également pour un problème multi-classe.

---

## Phase 6 : Visualisation

Création de :
- graphiques de comparaison des performances
- matrices de confusion

Ces outils permettent de comprendre non seulement combien d'erreurs sont commises, mais aussi lesquelles.

---

## Phase 7 : Scaling et Data Leakage

Étude de l'impact du StandardScaler sur les performances.

Constats :
- KNN bénéficie fortement du scaling
- Logistic Regression bénéficie également du scaling
- Decision Tree est peu impacté



## Résultats et conclusion

Les performances varient selon le dataset utilisé.

Le modèle le plus performant sur le dataset Breast Cancer a été :

**Logistic Regression**

Pourquoi ce choix ?

- Excellente accuracy
- Modèle rapide à entraîner
- Facile à interpréter
- Adapté aux applications médicales

Ce projet a permis de mettre en pratique :
- la classification supervisée
- le clustering non supervisé
- l'évaluation des modèles
- la visualisation des résultats
- les bonnes pratiques de préparation des données

---

