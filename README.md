# 📊 Analyse des données des systèmes éducatifs

Projet réalisé dans le cadre de la formation **Data Engineer - OpenClassrooms**.

L'objectif du projet est d'analyser des données éducatives mondiales afin d'identifier les pays présentant le plus fort potentiel pour l'expansion d'une academy à l'international.

---

# 🎯 Objectif du projet

Identifier les pays les plus intéressants pour l'implantation d'une academy en analysant :

* les indicateurs économiques
* les indicateurs éducatifs
* les données démographiques

Une méthode de **scoring pondéré** a été développée afin de classer les pays selon leur potentiel.

---

# 🧹 Nettoyage des données

Plusieurs étapes de préparation des données ont été réalisées :

* chargement et exploration des datasets
* suppression des colonnes contenant plus de **90 % de valeurs manquantes**
* vérification et suppression des doublons
* calcul de statistiques descriptives
* sélection des **15 années contenant le moins de valeurs manquantes**
* sélection des **15 indicateurs les plus pertinents**

Les pays contenant trop de données manquantes ont également été retirés afin d'obtenir un dataset exploitable.

---

# 📊 Analyse des indicateurs

Chaque indicateur sélectionné a été analysé individuellement :

* analyse statistique avec `describe()`
* visualisation des distributions
* interprétation des résultats

Cette étape a permis de mieux comprendre les relations entre les variables et d'identifier les indicateurs les plus pertinents pour l'analyse.

---

# 🔎 Suppression des indicateurs redondants

Une analyse de corrélation a été réalisée afin d'identifier les indicateurs fortement corrélés.

Lorsque deux indicateurs présentaient une corrélation supérieure à **0.9**, l'un d'eux a été supprimé afin d'éviter la redondance et de simplifier le modèle d'analyse.

Certains indicateurs séparés par genre (homme / femme) ont également été retirés car ils étaient fortement corrélés aux indicateurs globaux.

---

# 🧠 Méthode de scoring

Un algorithme de scoring appelé **Score Academy** a été développé pour classer les pays.

Chaque pays reçoit un score basé sur plusieurs indicateurs :

| Indicateur                   | Poids |
| ---------------------------- | ----- |
| PIB par habitant             | 8     |
| Nombre d'élèves et étudiants | 3     |
| PIB total                    | 3     |
| Population totale            | 1     |

Ce score permet d'obtenir un **classement objectif des pays présentant le plus fort potentiel de marché**.

---

# 📈 Résultats

L'analyse permet de comparer les pays selon plusieurs dimensions :

* richesse économique
* taille du marché éducatif
* stabilité économique
* taille de la population

Le score final permet d'identifier les pays présentant **le plus fort potentiel pour une expansion internationale**.

---

# ⚠️ Limites de l'analyse

* données agrégées au niveau national
* absence de facteurs qualitatifs (réglementation, concurrence, culture)
* certaines données peuvent être anciennes

Ce projet constitue donc **une première analyse exploratoire** pour identifier des marchés potentiels.

---

# 🛠️ Technologies utilisées

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

Les dépendances du projet sont définies dans le fichier `pyproject.toml`.

---

# ▶️ Reproduire le projet

Cloner le repository :

git clone https://github.com/YAD95/OC-Projet-Analyse-Systemes-Educatifs.git

Installer l'environnement :

uv sync

Lancer Jupyter :

jupyter lab

---

# 📂 Contenu du repository

education_data_analysis.ipynb → analyse complète des données
project_presentation.pptx → présentation du projet
pyproject.toml → environnement reproductible

---

# 👨‍💻 Auteur

YAD95
Projet OpenClassrooms – Analyse des données des systèmes éducatifs
