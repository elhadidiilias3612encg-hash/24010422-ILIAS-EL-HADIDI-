# 📊 Projet Data Science – Prédiction des Prix des Céréales

## 🧠 Contexte
Les prix des céréales jouent un rôle central dans l’économie mondiale et la sécurité alimentaire.
Ce projet exploite **30 années de données historiques** afin d’analyser les tendances des prix
et de construire un modèle de **Machine Learning** capable de prédire leur évolution future.

---

## 🎯 Objectifs du Projet
- Analyser l’évolution historique des prix des céréales  
- Identifier les tendances et la saisonnalité  
- Construire un modèle prédictif robuste  
- Évaluer la performance du modèle  

---

## 📁 Dataset
- **Source :** Kaggle  
- **Nom :** *Cereal Prices Changes Within Last 30 Years*  
- **Type :** Série temporelle multivariée  
- **Période :** ~30 ans  

---

## 🔧 Méthodologie

### 1️⃣ Préparation des données
- Conversion des dates
- Suppression des doublons
- Traitement des valeurs manquantes (médiane)

### 2️⃣ Analyse Exploratoire (EDA)
- Statistiques descriptives
- Analyse des tendances temporelles
- Corrélations entre céréales
- Visualisations graphiques

### 3️⃣ Feature Engineering
- Extraction de variables temporelles :
  - Année
  - Mois
  - Trimestre

### 4️⃣ Modélisation
- Algorithme utilisé : **RandomForestRegressor**
- Séparation Train / Test
- Entraînement du modèle

### 5️⃣ Évaluation
- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score

### 6️⃣ Optimisation
- GridSearchCV
- Ajustement des hyperparamètres

---

## 📈 Résultats
Le modèle Random Forest :
- capture correctement les tendances globales,
- présente des erreurs maîtrisées,
- montre une bonne capacité de généralisation.

---

## 🚀 Perspectives
- Modèles de séries temporelles (ARIMA, Prophet)
- Réseaux de neurones (LSTM)
- Intégration de données externes (climat, inflation)

---

## 📂 Structure du Projet
```
├── README.md
├── rapport_complet.md
├── Code_PROJET.ipynb
├── data/
```

---

## 🛠️ Technologies Utilisées
- Python
- Pandas / NumPy
- Matplotlib / Seaborn
- Scikit-learn
- KaggleHub

---

## 👨‍🎓 Auteur
Projet réalisé dans le cadre d’un apprentissage en **Data Science & Machine Learning**.

---

⭐ *N'hésitez pas à explorer le rapport complet pour plus de détails techniques.*
