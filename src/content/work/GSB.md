---
title: GSB entreprise pharmaceutique
publishDate: 2019-12-01 00:00:00
img: /assets/gsb-logo.png
img_alt: logo Gsb
description: |
  Dévellopement d'un site pour les rapport de visite pour l'entreprise.
tags:
  - Dev
---

### 1. Introduction
#### 1.1 Description du projet
L’objectif est de développer une application Web permettant aux visiteurs médicaux de centraliser leurs rapports de visite. Cette plateforme vise à améliorer la communication avec les praticiens et à offrir une vision synthétique de l’activité des visiteurs.

#### 1.2 Objectifs
Fournir un outil centralisé pour la saisie et la consultation des rapports de visite.

Faciliter l’accès aux informations pour une meilleure gestion et suivi des activités.

Assurer un environnement sécurisé pour la gestion des données sensibles.

### 2. Spécifications fonctionnelles
#### 2.1 Fonctionnalités principales
##### 2.1.1 Page de Connexion
Formulaire de connexion permettant l’identification des utilisateurs.

Validation des identifiants avec la base de données et gestion des sessions.

##### 2.1.2 Page d’Accueil
Point d’entrée principal avec navigation vers les différentes sections.

Affichage personnalisé en fonction de l’authentification de l’utilisateur.

##### 2.1.3 Consultation des Rapports
Accès sécurisé aux rapports de visite enregistrés.

Affichage des informations détaillées (praticiens visités, motifs, bilans, médicaments présentés, échantillons distribués).

##### 2.1.4 Saisie des Rapports
Formulaire permettant aux visiteurs médicaux d’enregistrer leurs visites.

Validation des entrées et stockage sécurisé dans la base de données.

### 3. Architecture du site
Architecture basée sur un modèle client-serveur avec interactions entre une interface Web et une base de données.

Séparation des responsabilités avec une gestion des utilisateurs et des droits d’accès sécurisés.

![Architecture du site gsb](/assets/GSB_architecture.png)

### 4. Conception technique
#### 4.1 Langages utilisés
HTML : Structure des pages Web.

CSS : Mise en forme et design.

PHP : Gestion de la logique serveur (authentification, sessions, requêtes SQL).

SQL : Interaction avec la base de données via PHPMyAdmin.

#### 4.2 Base de données
Développement sous SQL avec PHPMyAdmin pour stocker les rapports de visite et gérer les utilisateurs.

Sécurisation des accès pour garantir la confidentialité des données.

![shema base de donnée](/assets/shéma-donnée-GSB.png)

### Conclusion
Ce projet offre une solution efficace pour la gestion des rapports de visite médicale, permettant aux visiteurs de centraliser leurs activités tout en garantissant une gestion sécurisée et fluide des données.