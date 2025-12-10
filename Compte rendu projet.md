# Cereal Prices Changes Within Last 30 Years -- Data Analysis & Machine Learning Project

## 1. Introduction

Ce projet analyse l'évolution des prix de plusieurs céréales (blé, maïs,
riz, avoine...) sur 30 ans et développe un modèle de Machine Learning
pour prédire leurs prix futurs.\
Dataset utilisé : **Cereal Prices Changes Within Last 30 Years
(Kaggle)**.

## 2. Chargement du Dataset

Les données sont importées via `kagglehub` dans Google Colab puis
chargées avec `pandas`.

## 3. Nettoyage des Données

-   Conversion de la colonne Date
-   Suppression des doublons
-   Imputation des valeurs manquantes (médiane)
-   Vérification des types

## 4. Analyse Exploratoire (EDA)

-   Statistiques descriptives
-   Analyse de tendance temporelle
-   Heatmap de corrélation
-   Étude de la volatilité
-   Visualisation des séries temporelles

## 5. Feature Engineering

Ajout de nouvelles variables temporelles : - year - month - quarter

## 6. Modèle Machine Learning

Modèle utilisé : **RandomForestRegressor**\
Objectif : prédire le prix du blé ou d'une autre céréale

## 7. Évaluation du Modèle

Métriques utilisées : - MAE - RMSE - R² score

## 8. Optimisation du Modèle

Utilisation de **GridSearchCV** pour optimiser : - n_estimators -
max_depth - min_samples_split

## 9. Importance des Variables

Visualisation des features influentes : - Variables temporelles -
Céréales corrélées - Tendances globales

## 10. Conclusion

Le modèle Random Forest obtient de bonnes performances et permet de
comprendre les facteurs qui influencent les prix des céréales.\
Le projet peut être étendu vers : - LSTM (Deep Learning) - Prophet
(prévision avancée) - Modèles ARIMA

------------------------------------------------------------------------

## Structure recommandée du dépôt GitHub

    📁 cereal-prices-ml
     ├── README.md
     ├── notebook.ipynb
     ├── data/
     ├── plots/
     └── model.pkl
