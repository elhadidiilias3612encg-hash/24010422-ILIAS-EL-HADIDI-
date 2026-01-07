![Évolution des prix des céréales](images/ilias.jpg)

# Projet : Évolution des prix des céréales (30 dernières années)                                                                                                                            

## Description générale
Ce projet vise à analyser l’évolution des prix de plusieurs céréales (blé, maïs, riz, avoine, etc.) sur une période de 30 ans, puis à développer un modèle de Machine Learning capable de prédire les prix futurs.  
Il combine analyse statistique, visualisation de données et modélisation prédictive.

Dataset utilisé : **Cereal Prices Changes Within Last 30 Years (Kaggle)**

---

## Objectifs du projet
- Comprendre les tendances historiques des prix des céréales  
- Identifier les facteurs influençant les variations de prix  
- Construire un modèle prédictif fiable  
- Évaluer et optimiser les performances du modèle  

---

## Environnement et outils utilisés
- **Python**
- **Google Colab**
- **Bibliothèques principales** :
  - pandas
  - numpy
  - matplotlib / seaborn
  - scikit-learn
  - kagglehub

---

## Structure du projet
- `data/` : dataset brut et nettoyé  
- `notebook.ipynb` : notebook d’analyse et de modélisation  
- `README.md` : documentation du projet  
- `results/` : graphiques et résultats du modèle  

---

## Étapes détaillées du projet

### 1. Chargement des données
Les données sont téléchargées depuis Kaggle à l’aide de `kagglehub`, puis importées dans un DataFrame pandas pour traitement.

### 2. Nettoyage des données
- Conversion de la colonne **Date** en format datetime  
- Suppression des doublons  
- Traitement des valeurs manquantes par imputation (médiane)  
- Vérification et correction des types de données  

### 3. Analyse Exploratoire des Données (EDA)
- Calcul des statistiques descriptives  
- Étude des tendances temporelles des prix  
- Analyse de la corrélation entre les céréales  
- Mesure de la volatilité des prix  
- Visualisation des séries temporelles  

### 4. Feature Engineering
Création de nouvelles variables explicatives :
- Année (`year`)
- Mois (`month`)
- Trimestre (`quarter`)

Ces variables permettent de mieux capturer la saisonnalité et les tendances.

### 5. Modélisation
- Modèle choisi : **RandomForestRegressor**
- Variable cible : prix d’une céréale (ex. blé)
- Séparation des données en jeu d’entraînement et de test

### 6. Évaluation du modèle
Les performances sont évaluées à l’aide des métriques suivantes :
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

### 7. Optimisation
Optimisation des hyperparamètres avec **GridSearchCV** :
- `n_estimators`
- `max_depth`
- `min_samples_split`

### 8. Importance des variables
Analyse de l’importance des features afin d’identifier :
- L’impact des variables temporelles  
- Les céréales les plus corrélées  
- Les tendances globales du marché  

---

## Résultats et interprétation
Le modèle Random Forest montre de bonnes performances et permet de comprendre les facteurs clés influençant les prix des céréales. Les résultats confirment l’importance de la dimension temporelle et des corrélations inter-produits.

---

## Limites et perspectives
- Intégration de facteurs macroéconomiques (inflation, climat, géopolitique)  
- Utilisation de modèles avancés :
  - LSTM (Deep Learning)
  - Prophet
  - ARIMA / SARIMA  

---

## Auteur
Projet académique – Analyse de données et Machine Learning
