---
title: GLPI
publishDate: 2023-10-02 00:00:00
img: /assets/logo-glpi.png
img_alt: logo glpi.
description: |
  Decouverte et parametrage de l'outils de gestion de parc informatique GLPI
tags:
  - Dev
---

#### GLPI ?
GLPI (Gestionnaire Libre de Parc Informatique) est un logiciel open-source de gestion des services informatiques (ITSM). Il permet aux entreprises et organisations de gérer efficacement leur parc informatique, leurs tickets d’assistance, leurs interventions et bien d’autres aspects liés à la gestion IT.


#### 1. Vision générale de la plateforme
GLPI est un outil de gestion de parc informatique permettant de suivre les équipements, les licences, les utilisateurs et les tickets d’assistance. L’interface technicien offre un tableau de bord centralisé avec des filtres pour afficher les informations sur les tickets et le parc matériel.

![Visu générale](/assets/Matrice_urgence_GLPI.png)

#### 2. Saisie d’inventaire
Paramétrage des lieux et entités : Organisation des équipements selon des entités (périmètre logique avec restrictions d’accès) et des lieux (emplacements physiques).

Plan de nommage : Chaque appareil est identifié par un code composé de son type, du numéro de salle et d’une désignation unique.

#### 3. Matrice d’urgence
Un système de classification des incidents selon leur impact et leur urgence :

![matrice d'urgence](/assets/glpiBase.PNG)


#### 4. Cycle de vie d’un ticket utilisateur

![Cycle de vie d’un ticket](/assets/cycle_vie_tickets.png)

Ouverture : Création du ticket par l’utilisateur.

Classification : Évaluation et assignation du ticket.

Traitement : Résolution en cours avec mises à jour régulières.

Solution : Problème corrigé et documenté.

Validation : Confirmation par l’utilisateur.

Fermeture : Archivage et amélioration continue.

####

#### 6. Requêtes de consultation du parc
Exemples de requêtes SQL pour analyser le parc :

Liste des PC avec 4 Go de RAM :

sql
Copier
Modifier
SELECT * FROM computers WHERE ram = 4;
Nombre de PC avec Office 2007 installé :

sql
Copier
Modifier
SELECT COUNT(*) FROM software WHERE software_name = 'Office 2007';
Liste des 50 PC les moins performants :

sql
Copier
Modifier
SELECT * FROM computers WHERE ram = 4 AND ram_technology = 'DDR3' AND disk_space_partition < 128 LIMIT 50;

#### 7. Statistiques et analyse
Taux de résolution des tickets : Identification des problèmes récurrents et optimisation du support.

Temps moyen de réponse : Suivi des délais par niveau de priorité.

Satisfaction des utilisateurs : Évaluation continue pour améliorer le service d’assistance.


#### Compétence

![Tableau de Compétence](/assets/tableauCompGLPI.png)

#### Documentation

[📄 Compte Rendu avec plus détaille](/assets/GLPI_CompteRendu.pdf)
