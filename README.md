# Prédiction du Prix des Logements - Projet IA 
Modèle de régression basé sur des caractéristiques socio-économiques.

## Description :
Ce projet consiste à prédire le prix de logements à partir d'un dataset public provenant de Kaggle : 
Housing Dataset : https://www.kaggle.com/datasets/huyngohoang/housingcsv/code
Le modèle utilise un ensemble de caractéristiques décrivant la zone dans laquelle se trouve chaque logement, puis applique différents traitements d'analyse, de visualisation et finalement une régression linéaire pour estimer le prix des biens immobiliers. 

## Caractéristiques utilisées
Le modèle s'appuie sur les variables suivantes :
- Avg. Area Income - Revenu moyen de la zone
- Avg. Area House Age - Âge moyen des maisons
- Avg. Area Number of Rooms - Nombre moyen de pièces
- Avg. Area Number of Bedrooms - Nombre moyen de chambres
- Area Population - Population moyenne dans la zone
Ces facteurs montrent une bonne corrélation avec le prix, en particulier :
Avg. Area Income, fortement corrélé positivement avec Price.

## Objectifs du projet
- Explorer et analyser le dataset
- Étudier les corrélations entre les variables
- Construire et entraîner un modèle de régression linéaire
- Évaluer les performances (MSE, R²)
- Tester des prédictions manuelles
- Sauvegarder un modèle entraîné pour un usage ultérieur
  
## Résultats du modèle
Les performances obtenues avec LinearRegression :
- Erreur quadratique moyenne (MSE)
  - 10089009299.499458 
  - Cela correspond à une erreur moyenne d'environ 100 000 $ par prédiction, ce qui est cohérent pour un modèle linéaire appliqué à ce dataset.
- Coefficient de détermination (R²)
  - 0.9179971706985317
  -  Un R² proche de 1 indique que le modèle explique très bien la variance du prix des logements.

## Prédiction manuelle
Le notebook présente un exemple illustrant :
- la préparation des données d'entrée sous forme de tableau
- l'appel au modèle .predict()
- l'affichage du prix estimé

## Sauvegarde du modèle
Le projet montre également comment :
- Enregistrer un modèle déjà entraîné (joblib)
- Le recharger plus tard sans réentraînement
Cela permet d'utiliser directement la régression pour des prédictions en production ou dans une application intégrée.

## Comment exécuter le projet
1. Cloner le dépôt :
git clone https://github.com/longuetbriandavid/PredictionDuPrixDesLogements.git
1. Ouvrir le fichier dans google colab:
Prédiction_du_prix_des_logements.ipynb
1. Exécuter le notebook cellule par cellule?

Vous pouvez également retrouver le modèle utilisé dans le dépôt ; il vous suffira de le charger. 
