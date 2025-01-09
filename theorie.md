# GLPI, Fusion Inventory, Nagios - Théorie

## Informations

| Champ           | Détails                                            |
|-----------------|----------------------------------------------------|
| **Auteur**      | William Mbakop                                     |
| **Profession**  | étudiant en alternance - BTS SIO SISR              |
| **Version**     | 1.0.0                                              |
| **Date**        | 9 janvier 2025                                     |
| **Description** | GLPI, Fusion Inventory, Nagios - Théorie           |


## Introduction

GLPI, FusionInventory et Nagios sont trois outils populaires utilisés dans la gestion de l'infrastructure informatique et la surveillance des systèmes. Bien qu'ils aient des objectifs différents, ils peuvent être utilisés ensemble pour offrir une solution complète de gestion, d'inventaire et de surveillance des équipements.

## GLPI (Gestionnaire Libre de Parc Informatique)
Objectif : GLPI est un outil de gestion de parc informatique (ITSM - Information Technology Service Management) qui permet de gérer les ressources informatiques, telles que les équipements, les logiciels, les licences, et les services.

Fonctionnalités principales :

- Inventaire des équipements : GLPI permet de suivre et de gérer tout le matériel informatique de l'entreprise (ordinateurs, serveurs, imprimantes, etc.) et les logiciels associés.
- Gestion des incidents et des demandes : GLPI permet de gérer les tickets d'incidents et de demandes des utilisateurs. Cela inclut la création de tickets, l'attribution à des techniciens, et la gestion du flux de travail.
- Suivi des interventions : Il permet aux administrateurs de suivre les interventions, les maintenances et les réparations effectuées sur les équipements.
- Planification et gestion des changements : GLPI permet de suivre les modifications effectuées sur les équipements, de planifier les mises à jour et d'appliquer des politiques de gestion des actifs.
- Intégration avec d'autres outils : GLPI peut être étendu avec des plugins (comme FusionInventory et Nagios) pour ajouter des fonctionnalités supplémentaires, notamment l'inventaire automatique et la surveillance.
Utilisation principale : Gestion d'inventaire, suivi des actifs, gestion des tickets de support et des interventions.

## FusionInventory

Objectif : FusionInventory est un outil d'inventaire automatique et de gestion des équipements, qui s'intègre parfaitement avec GLPI pour récupérer les informations sur le matériel et les logiciels des postes de travail et des serveurs.

Fonctionnalités principales :

- Inventaire matériel et logiciel : FusionInventory permet de récupérer automatiquement des informations sur le matériel (processeur, RAM, disque dur, carte mère, etc.) et les logiciels installés sur les machines (y compris les licences logicielles).

- Gestion des périphériques réseau : FusionInventory peut aussi être utilisé pour inventorier des périphériques réseau comme les imprimantes, les switchs et les routeurs.

- Dépannage à distance : Il propose des fonctionnalités pour exécuter des commandes à distance sur les machines clientes.
Rapports : FusionInventory génère des rapports détaillés sur l'état des équipements et leur configuration.

- Communication avec GLPI : FusionInventory s'intègre directement avec GLPI, ce qui permet de synchroniser automatiquement les informations d'inventaire et de gestion des équipements entre les deux systèmes.

- Utilisation principale : Inventaire des équipements et des logiciels, collecte automatique des informations matérielles, et intégration avec GLPI pour la gestion centralisée des ressources.

## Nagios

Objectif : Nagios est un outil de surveillance des systèmes et des réseaux qui permet de surveiller l'état des équipements informatiques, des serveurs, des services, et des applications.

Fonctionnalités principales :

- Surveillance des hôtes et des services : Nagios surveille en continu les équipements (serveurs, ordinateurs, périphériques réseau) et les services (HTTP, FTP, DNS, etc.) pour détecter des pannes ou des dysfonctionnements.

- Alertes et notifications : Lorsque Nagios détecte un problème (par exemple, un serveur qui est hors ligne ou un service qui ne répond pas), il génère des alertes et envoie des notifications par e-mail, SMS ou autres moyens pour avertir les administrateurs.
Plugins extensibles : Nagios dispose d'une vaste bibliothèque de plugins qui permettent de surveiller des services et des applications spécifiques (par exemple, les bases de données, les systèmes de messagerie, les équipements réseau, etc.).

- Interface web : Nagios offre une interface web pour afficher l'état des hôtes, des services et des alertes en temps réel.
NRPE (Nagios Remote Plugin Executor) : Nagios utilise NRPE pour exécuter des vérifications à distance sur des hôtes distants, ce qui permet de surveiller des machines qui ne sont pas localement connectées au serveur Nagios.

- Utilisation principale : Surveillance des performances et de la disponibilité des hôtes, des services et des applications. Détection des pannes et gestion des alertes.

## Comment ils fonctionnent ensemble ?

- GLPI est utilisé pour gérer les ressources informatiques (matériel, logiciels, licences) et le support technique (gestion des tickets, des interventions, etc.).

- FusionInventory s'intègre à GLPI pour effectuer un inventaire automatique du matériel et des logiciels. Cela permet à GLPI de récupérer les informations sans intervention manuelle et d'avoir une vue en temps réel sur l'état des équipements.

- Nagios est utilisé pour surveiller l'état des équipements et des services. Il peut envoyer des alertes à l'administrateur si une machine ou un service devient défaillant.

Ensemble, ces outils offrent une solution complète de gestion de l'infrastructure informatique :

- GLPI gère les actifs et les tickets,

- FusionInventory collecte les données d'inventaire automatiquement,

- Nagios assure la surveillance des performances et la détection des incidents.