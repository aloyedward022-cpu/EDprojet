# EDprojet
# 📊 Pro-Quant Trader
Application d’analyse financière et de backtesting développée avec **Python** et **Streamlit**, dans le cadre du module **Mathématiques appliquées au traitement des données**.
Ce projet vise à transformer des concepts mathématiques (statistiques, probabilités, calculs vectorisés) en un **outil concret d’analyse financière**, inspiré de plateformes professionnelles comme **TradingView**, **Bloomberg** et **Binance**.
 🎯 Objectifs pédagogiques

L’objectif principal est de démontrer la capacité à :
* Manipuler des données financières sous forme matricielle
* Calculer et interpréter des indicateurs financiers
* Appliquer des concepts statistiques aux rendements
* Implémenter et tester une stratégie de trading simple
* Visualiser les résultats de manière claire et professionnelle

 🧠 Fonctionnalités principales

1) Acquisition des données

* Récupération des données financières via **Yahoo Finance (yfinance)**
* Actifs supportés : actions, indices, cryptomonnaies (ex: AAPL, NVDA, BTC-USD)
* Paramètres configurables :

  * Actif financier
  * Date de début et de fin
  * Fréquence temporelle : journalière, horaire, 5 minutes
2) Indicateurs techniques

Les indicateurs sont calculés manuellement afin de garantir la rigueur mathématique.

* Moyenne Mobile Simple (SMA rapide et lente)
* Relative Strength Index (RSI)
* Bandes de Bollinger

Les paramètres sont entièrement modifiables via l’interface Streamlit.

---

3) Stratégie de trading

Stratégie basée sur :

* Croisement de moyennes mobiles (SMA rapide / SMA lente)
* Filtre RSI pour éviter les zones de sur-achat

**Règles :**

* Achat : SMA rapide > SMA lente et RSI < 70
* Position neutre sinon

Les positions sont décalées d’une période afin d’éviter tout biais de regard vers le futur.

---

4) Backtesting

Le module de backtesting calcule :

* Rendements de la stratégie
* Frais de transaction paramétrables
* Capital cumulé (capital initial = 1000)

#### 📈 Métriques de performance

* Rendement total
* Volatilité annualisée
* Ratio de Sharpe (taux sans risque = 0)
* Drawdown maximum
* Taux de réussite (Win Rate)

---

5) Statistiques et probabilités

Analyse statistique des rendements :

* Moyenne, médiane, écart-type
* Skewness et Kurtosis
* Tests de normalité (Jarque-Bera)

**Interprétation :**

* Si p-value < 0.05 → rejet de l’hypothèse de normalité
*
* 6) Visualisation

* Graphique principal en chandeliers (Plotly)
* Superposition des indicateurs techniques
* Comparaison stratégie vs benchmark
* Interface sombre inspirée des plateformes professionnelles

---

## 🛠️ Technologies utilisées
* **Python 3.8+**
* **Streamlit** – interface interactive
* **Pandas / NumPy** – traitement des données
* **Plotly** – visualisations interactives
* **yfinance** – données financières
* **SciPy** – statistiques
## 🚀 Installation et exécution
### 1️⃣ Cloner le projet

```bash
git clone https://github.com/votre-username/pro-quant-trader.git
cd pro-quant-trader
---

## 📌 Inspirations

* TradingView – analyse technique
* Bloomberg Terminal – structure des dashboards
* Binance – interface de trading

---

📚 Améliorations futures

* Ajout du MACD et EMA
* Multi-actifs et corrélations
* Export des résultats en CSV
* Backtesting multi-stratégies
* Mode temps réel

---

👤 Auteur

**Aloysius Edward**
Projet académique – Mathématiques appliquées à la finance CMC
