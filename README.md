## JAVA-app  ###Gestion des Développeurs et des Projets

## Introduction

Dans le cadre de ce projet, nous avons développé une application web permettant aux chefs de projet de gérer efficacement les développeurs et leurs affectations à différents projets en fonction de leurs compétences. L’application offre également des fonctionnalités de suivi et d’évaluation des performances des développeurs pour garantir une gestion optimale des ressources humaines et des projets.

## Objectifs du Projet

Le projet vise à répondre aux besoins spécifiques des chefs de projet en matière de gestion des développeurs et des projets tout en offrant une interface intuitive et des fonctionnalités optimisées. Voici les objectifs principaux du projet :

### 1. Faciliter la gestion des développeurs
- Créer, mettre à jour et gérer les profils des développeurs.
- Recherche avancée des développeurs selon leurs compétences et leur disponibilité.

### 2. Optimiser la gestion des projets
- Création et gestion des projets (titre, description, durée estimée, compétences requises).
- Affectation des développeurs aux projets en fonction de leurs compétences spécifiques.

### 3. Évaluer les performances des développeurs
- Système d’évaluation pour les développeurs sur la qualité du travail, le respect des délais, et leur contribution.
- Fournir des retours détaillés pour améliorer leur performance.

### 4. Améliorer le suivi des contributions
- Interface pour les développeurs pour consulter les projets auxquels ils sont affectés et les évaluations reçues.
- Suivi de l’état d’avancement des projets et des contributions individuelles pour les chefs de projet.

### 5. Assurer la sécurité et la gestion des utilisateurs
- Authentification sécurisée pour les chefs de projet et les développeurs.
- Gestion des rôles et permissions en fonction des responsabilités (chef de projet ou développeur).

### 6. Respecter une architecture robuste et évolutive
- Architecture en couches (MVC) garantissant une séparation claire des responsabilités.
- Utilisation de Spring Boot et Thymeleaf pour des performances optimales.

## Diagrammes

L’objectif principal de cette application est de simplifier les tâches complexes de gestion des équipes et des projets tout en assurant une interface intuitive et des fonctionnalités robustes. Vous pouvez consulter le diagramme théorique et réel via le lien suivant : 

[Diagramme Théorique et Réel](https://drive.google.com/file/d/1EStqeASjhENKZHvJI9ePVeZzugTfKl0T/view?usp=sharing)

## Outils Utilisés

### 1. Backend
- **Spring Boot** : Framework Java utilisé pour le backend.
- **Hibernate** : Framework ORM pour la gestion des interactions avec la base de données.
- **Java** : Langage principal utilisé pour le développement backend.

### 2. Frontend
- **Thymeleaf** : Moteur de templates pour le rendu dynamique des vues HTML.
- **HTML/CSS** : Structuration et style des pages web.
- **Bootstrap** : Framework CSS pour une interface moderne et responsive.

### 3. Base de Données
- **MySQL** : Base de données relationnelle pour stocker les informations des développeurs, projets et évaluations.

### 4. Environnement de Développement
- **IntelliJ IDEA** : IDE pour le développement du projet.
- **Maven** : Outil de gestion des dépendances et de construction du projet.

## Structure du Projet

Le projet suit une architecture en couches (MVC). Voici une description des principales couches :

### 1. Couche Contrôleur (Controller)
Cette couche gère les interactions entre l’utilisateur et l’application :
- **AuthController** : Gestion de l'authentification et de l'inscription des utilisateurs.
- **ChefDeProjetController** : Gestion des projets et affectations des développeurs.
- **DeveloppeurController** : Gestion des développeurs et consultation des projets.
- **ProjetController** : Gestion des projets (création, modification).
- **EvaluationController** : Gestion des évaluations des développeurs.

### 2. Couche DAO (Data Access Object)
Interaction avec la base de données via Spring Data JPA :
- **ChefDeProjetRepository**
- **DeveloppeurRepository**
- **ProjetRepository**
- **EvaluationRepository**

### 3. Couche Service
Contient la logique métier de l’application :
- **ChefDeProjetService**, **DeveloppeurService**, **ProjetService**, **EvaluationService**

### 4. Couche Modèle (Entity)
Définition des entités métiers :
- **ChefDeProjet**, **Developpeur**, **Projet**, **Evaluation**

### 5. Couche Vue (Thymeleaf Templates)
Rendu des vues HTML interactives :
- **Pages pour le Développeur** : Menu, Liste des développeurs, Formulaire de gestion des développeurs, Consultation des projets.
- **Pages pour le Chef de Projet** : Menu, Ajout de projet, Affectation des développeurs, Évaluation.
- **Pages Générales** : Connexion, Page d’accueil.

### 6. Fichiers de Configuration
- **application.properties** : Configuration de la base de données et des paramètres de l’application.
- **SecurityConfig** : Configuration de la sécurité (authentification et autorisation).

## Test et Interfaces

Des tests ont été réalisés pour valider les principales fonctionnalités et interfaces du projet, garantissant son bon fonctionnement et sa sécurité.

## Contraintes et Difficultés

Le projet a impliqué la gestion de plusieurs utilisateurs et rôles différents, ainsi que la sécurisation des accès. Les principales difficultés ont concerné l'intégration fluide des technologies et l’adaptation de l’architecture en couches.

## Conclusion

Ce projet de gestion des développeurs et des projets a permis de créer une application robuste et intuitive répondant aux besoins des chefs de projet. Grâce aux technologies modernes comme Spring Boot et Thymeleaf, l’application garantit une gestion efficace des ressources humaines et une expérience utilisateur fluide et sécurisée. L’adoption de l’architecture MVC assure une évolutivité et une facilité de maintenance pour le futur développement de l’application.

