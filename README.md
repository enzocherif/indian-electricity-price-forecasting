# 🇮🇳 Indian Electricity Market Price Forecasting

> **Objectif :** Prédire les prix journaliers du marché de l’électricité en Inde (MCP) à l’aide de données de production d’énergie, de prix passés et de conditions météo.

---

## 📂 Contenu du projet

Ce projet a été réalisé dans un court délai (un week-end) suite à un second entretien avec ENGIE dans le cadre d’un V.I.E en Inde. Il vise à démontrer mes compétences en :
- collecte de données réelles (CSV/API)
- préparation et fusion de sources hétérogènes
- modélisation prédictive avec des algorithmes de machine learning
- interprétation des résultats et visualisations

---

## 🔧 Données utilisées

Les données proviennent de deux jeux de données publics disponibles sur Kaggle :

- 📊 [Indian Energy Exchange Time Series (2019–2024)](https://www.kaggle.com/datasets/mukund604/indian-energy-exchange-time-series-forecasting)  
  → Prix de l'électricité (MCP), demande/volume échangé, données de marché.

- ⚡ [Daily Power Generation in India (2013–2023)](https://www.kaggle.com/datasets/krishnadaskv/daily-power-generation-in-india-2013-2023)  
  → Données de production par source : charbon, hydro, solaire, éolien, etc.

- 🌦️ [API météo (Open-Meteo)](https://open-meteo.com/)  
  → Données météorologiques agrégées pour l’Inde : température, précipitations, rayonnement, vent.

---

## 🧠 Modèles testés

Deux modèles ont été entraînés pour prédire le prix MCP :

| Modèle        | MAE (₹) | RMSE (₹) | R²     |
|---------------|---------|----------|--------|
| Random Forest | 547     | 1098     | 0.744  |
| XGBoost       | 483     | 999      | 0.789  |

> 🎯 L’objectif n’était pas de battre un record mais de proposer une solution robuste, documentée, et réutilisable.

---

## 📈 Visualisations incluses

- Courbe MCP réel vs MCP prédit
- Histogramme des résidus (erreurs)
- Importance des variables (features)
- Scatter plots entre production et prix
- Analyse des performances

---

## ⚙️ Installation

Installe les dépendances nécessaires :

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost requests
```

---

## 🚀 Lancer le projet

Lance le notebook :

```bash
jupyter notebook Indian_Electricity_Price_Prediction.ipynb
```

---

## ✍️ Remarques personnelles

Ce projet a été réalisé rapidement après un échange avec ENGIE où l’on m’a proposé d’envoyer des travaux supplémentaires. J’ai voulu relever ce défi personnel afin de prouver mes compétences en data science appliquée à l’énergie. Je suis conscient que le projet peut encore être amélioré (feature engineering, tuning, enrichissement météo plus précis, etc.) mais je suis fier de cette démonstration.

---

## 📬 Contact

* 👨‍💻 Enzo CHERIF
* 📧 [enzocherife@gmail.com](mailto:enzocherife@gmail.com)
* 🌐 [enzocherif.github.io](https://enzocherif.github.io)
