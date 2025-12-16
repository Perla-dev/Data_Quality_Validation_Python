# Data_Quality_Validation_Python
# 📊 Data Quality Validation and Consistency Checks (Python/SQL)

## 🎯 Aperçu du Projet

Ce projet est une implémentation de scripts de contrôle qualité et de validation de la cohérence des données, simulant les vérifications nécessaires dans un environnement de type **DataLake** ou de **pipeline ETL**. L'objectif est de s'assurer de l'**intégrité et de la conformité des données** après un processus de transformation ou de chargement.

## 🔑 Compétences et Outils Démontrés

| Domaine | Outils et Technologies |
| :--- | :--- |
| **Langage de Scripting** | **Python** (pour l'automatisation des vérifications et le traitement de la logique de test). |
| **Validation de Données** | **SQL** (pour les requêtes de vérification d'intégrité, de volume, et de cohérence). |
| **Tests Ciblés** | **Tests ETL** (Extraction, Transformation, Loading) et **Tests E2E** (validation de la donnée de bout en bout). |
| **Librairies Python** | Pandas (pour la manipulation et l'analyse des jeux de données). |
| **Processus** | Détection d'anomalies, rapports d'erreurs et proposition d'ajustements techniques. |

## ⚙️ Scénarios de Validation Clés

Le projet exécute des contrôles basés sur des règles métier critiques :

1.  **Vérification de l'Intégrité (SQL) :**
    * Contrôle de l'absence de valeurs nulles (NULL) dans les champs clés.
    * Validation de l'unicité des identifiants (clés primaires).
    * Vérification des références (clés étrangères) entre les tables.

2.  **Vérification de la Cohérence et de la Qualité (Python/Pandas) :**
    * Contrôle des formats de données (dates, chaînes de caractères).
    * Validation des plages de valeurs (ex. : les montants doivent être positifs).
    * Tests de volume (vérification que le nombre d'enregistrements transférés correspond aux attentes).

3.  **Rapport d'Anomalies :**
    * Les scripts identifient et loguent les incohérences de données, facilitant la traçabilité et le suivi des anomalies.

## ▶️ Comment Exécuter les Scripts

### Prérequis

* Python 3.x
* Librairies : Pandas, `psycopg2` ou `mysql-connector-python`.

### Étapes d'exécution

1.  Cloner le dépôt : `git clone https://github.com/Perla-dev/Data_Quality_Validation_Python.git`
2.  Installer les dépendances : `pip install -r requirements.txt`
3.  Mettre à jour les paramètres de connexion à la base de données de démo dans le fichier `config.py`.
4.  Lancer le script de validation : `python run_validation.py`

