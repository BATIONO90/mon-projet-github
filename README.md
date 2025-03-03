# Solutions-GED-IntelliGED-Autodoc
# IntelliGED - Gestion Électronique des Documents Intelligente

## Introduction

IntelliGED est un projet de Gestion Électronique des Documents (GED) qui intègre l'intelligence artificielle pour automatiser divers processus documentaires. Ce projet vise à simplifier la gestion des documents en utilisant des techniques avancées d'analyse, d'indexation, de classification, et de recherche sémantique.

## Contexte et Justification

Avec l'évolution rapide des technologies et l'accroissement exponentiel des données, les entreprises et les organisations ont besoin de solutions efficaces pour gérer leurs documents. L'automatisation de la gestion documentaire permet de réduire les efforts manuels, d'améliorer l'efficacité et de garantir une meilleure organisation des informations.

IntelliGED est conçu pour répondre à ces besoins en offrant une solution complète et intégrée qui utilise l'intelligence artificielle pour automatiser les tâches répétitives et complexes liées à la gestion des documents.

## Public Cible

Le projet IntelliGED s'adresse principalement à :
- **Entreprises et organisations** : Qui ont besoin de gérer un grand volume de documents de manière efficace et sécurisée.
- **Institutions éducatives** : Pour organiser et gérer les documents académiques et administratifs.
- **Professionnels indépendants** : Qui souhaitent automatiser la gestion de leurs documents personnels et professionnels.

## Modules du Projet

### 1. Catalogage automatique des documents
Ce module permet de cataloguer automatiquement les documents en extrayant les métadonnées et en les enregistrant dans la base de données.

### 2. Analyse automatique ou assistée IA des documents
Ce module utilise l'API OpenAI pour analyser le contenu des documents et générer des résumés ou des analyses détaillées.

### 3. Indexation automatique des documents
Ce module indexe les documents pour permettre une recherche rapide et efficace en utilisant des techniques d'indexation avancées.

### 4. Classification automatique des documents
Ce module utilise des modèles de machine learning pour classifier les documents en différentes catégories prédéfinies.

### 5. Recherche sémantique assistée IA
Ce module permet de rechercher des documents en utilisant des techniques de recherche sémantique pour obtenir des résultats plus pertinents.

### 6. OCR pour les documents scannés
Ce module utilise Tesseract OCR pour extraire le texte des documents scannés et des fichiers PDF contenant des images.

### 7. Gestion des utilisateurs et des permissions
Ce module permet de gérer les utilisateurs et leurs permissions d'accès aux documents pour garantir la sécurité et la confidentialité des informations.

### 8. Suivi des modifications et versioning des documents
Ce module permet de suivre les modifications apportées aux documents et de gérer les différentes versions pour assurer la traçabilité.

### 9. Notifications et alertes
Ce module envoie des notifications et des alertes aux utilisateurs pour les informer des événements importants, tels que l'ajout de nouveaux documents ou les résultats d'analyse.

### 10. Recherche avancée et filtrage des documents
Ce module offre des fonctionnalités de recherche avancée et de filtrage pour permettre aux utilisateurs de trouver rapidement les documents dont ils ont besoin.

### 11. Déploiement de l'application GED
Ce module utilise Docker et Docker Compose pour faciliter le déploiement de l'application dans des environnements de production.

## Téléchargement et Installation

### Prérequis
1. **XAMPP** : Installez et démarrez XAMPP.
2. **Base de données MySQL** : Créez une base de données MySQL dans XAMPP.
3. **Clé API OpenAI** : Obtenez une clé API OpenAI valide.
4. **Python 3.x** : Installez Python 3.x et les bibliothèques nécessaires.
5. **Tesseract OCR** : Installez Tesseract OCR.
6. **Docker** : Installez Docker.
7. **Docker Compose** : Installez Docker Compose.

### Étapes pour monter le projet

#### Étape 1 : Catalogage automatique des documents
1. **Installer les bibliothèques nécessaires** :
    ```sh
    pip install openai pymysql python-docx PyMuPDF
    ```
2. **Créer la base de données et la table `documents`** :
    ```sql
    CREATE DATABASE ged_db;
    USE ged_db;
    CREATE TABLE documents (
        id INT AUTO_INCREMENT PRIMARY KEY,
        file_name VARCHAR(255),
        file_path TEXT,
        metadata TEXT
    );
    ```
3. **Exécuter le script de catalogage** :
    ```sh
    python catalogue_documents.py
    ```

#### Étape 2 : Analyse automatique ou assistée IA des documents
1. **Installer les bibliothèques nécessaires** :
    ```sh
    pip install openai pymysql python-docx PyMuPDF
    ```
2. **Créer la table `document_analysis`** :
    ```sql
    USE ged_db;
    CREATE TABLE document_analysis (
        id INT AUTO_INCREMENT PRIMARY KEY,
        file_name VARCHAR(255),
        file_path TEXT,
        analysis TEXT
    );
    ```
3. **Exécuter le script d'analyse des documents** :
    ```sh
    python analyze_documents_with_chatgpt.py
    ```

#### Étape 3 : Indexation automatique des documents
1. **Installer les bibliothèques nécessaires** :
    ```sh
    pip install pymysql python-docx whoosh PyMuPDF
   
