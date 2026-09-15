# 🏭 Détection de Défauts dans la Production Industrielle (Machine Learning)

Ce projet applique des techniques avancées d'apprentissage supervisé pour identifier et prédire automatiquement les pièces défectueuses sur une chaîne de fabrication en fonction de multiples paramètres de production (coût, temps de maintenance, score de qualité, etc.).

---

## 📌 Objectifs du Projet

L'enjeu principal est de réduire les rebuts et les coûts liés aux arrêts de production en prédisant l'état de conformité (`DefectStatus`) avant la sortie d'usine.

* **Identification précoce :** Détecter avec précision les anomalies de production.
* **Traitement des données réelles :** Gérer le déséquilibre sévère des classes (les défauts étant rares par rapport aux pièces conformes).
* **Aide à la décision :** Optimiser le compromis entre précision et rappel pour minimiser les faux négatifs.

---

## 🛠️ Stack Technique

* **Langage :** Python
* **Manipulation de Données :** Pandas, NumPy
* **Machine Learning & Modélisation :** Scikit-Learn (Random Forest, Decision Tree, GridSearchCV)
* **Traitement du Déséquilibre :** Imbalanced-learn (SMOTE)
* **Visualisation Statistique :** Matplotlib, Seaborn

---

## 📊 Méthodologie & Pipeline ML

1. **Analyse Exploratoire des Données (EDA) :**
   * Étude des corrélations entre les variables clés (`QualityScore`, `MaintenanceHours`) et le taux de défaut.
   * Détection des distributions asymétriques et des valeurs aberrantes.

2. **Prétraitement des Données :**
   * Imputation des valeurs manquantes via `SimpleImputer`.
   * Encodage et normalisation des caractéristiques numériques.

3. **Gestion du Déséquilibre de Classes :**
   * Utilisation de l'algorithme **SMOTE** (*Synthetic Minority Over-sampling Technique*) pour synthétiser des exemples de la classe minoritaire et éviter le surapprentissage de la classe majoritaire.

4. **Modélisation & Optimisation :**
   * Entraînement de classifieurs d'arbres de décision et de forêts aléatoires (*Random Forest*).
   * Réglage fin des hyperparamètres via validation croisée (`GridSearchCV`).

---

## 📈 Évaluation des Performances

Les modèles ont été évalués principalement sur :
* **Recall (Rappel) :** Métrique critique afin de minimiser le risque de laisser passer une pièce défectueuse.
* **Precision :** Mesure de la fiabilité des alertes de défauts générées par le système.
* **Matrice de Confusion & Courbe ROC-AUC.**

---

## 🚀 Installation et Utilisation

1. **Cloner le dépôt :**
   ```bash
   git clone [https://github.com/sofiane-web/industrial-defect-detection-ml.git](https://github.com/sofiane-web/industrial-defect-detection-ml.git)
   cd industrial-defect-detection-ml


   👥 Auteurs & Contributeurs
FRITIT Sofyane — Data Analytics / Machine Learning

Moad Afylal — Binôme de projet