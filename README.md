# Project d'Automatisation d'Avis Client (McDonald's)

## Démonstration du Processus

### Aperçu Rapide
![2025-11-3004-41-52-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/af228ccc-158f-4365-a77c-f2219860c5c6)

## Démonstration
https://youtu.be/JQ_OsN6kvCM?si=RYWbMRV26y7JgQgc

## Aperçu du Projet

Ce projet est une solution logicielle conçue pour **automatiser la soumission d'avis clients** sur la plateforme de sondage d'une grande chaîne de restauration rapide (McDonald's).

Il est composé de deux parties principales qui travaillent ensemble :
1.  Une **interface graphique (GUI) en Python (Tkinter)** pour la planification, la gestion des statistiques et la configuration des paramètres de soumission.
2.  Un **script d'automatisation en Node.js (Puppeteer)** qui exécute les actions dans un navigateur pour remplir le formulaire et simuler la visite d'un client.

L'objectif principal est d'envoyer des avis avec des paramètres (date, heure, minute, âge) qui correspondent à une **distribution de fréquentation réaliste et crédible**, basée sur les configurations définies par l'utilisateur.

---

## Comment Ça Fonctionne ?

L'application suit un processus rigoureux pour garantir la crédibilité de chaque avis :

1.  **Planification Intelligente (Python)** :
    * Le programme lit les fichiers de configuration pour déterminer les ratios démographiques (âge) et les pics de fréquentation.
    * Il calcule une date et une heure de visite précises qui reflètent statistiquement le profil du client souhaité. 
2.  **Lancement du Bot (Python -> Node.js)** :
    * L'application Python lance le script Node.js en lui passant les paramètres calculés : la **date** (DD/MM/YYYY), la **minute du jour** (0-1439) et l'**âge cible** (valeur interne).
3.  **Simulation du Navigateur (Node.js/Puppeteer)** :
    * Le script Node.js prend le contrôle d'un navigateur headless.
    * Il remplit les champs cruciaux du formulaire (date, heure, minute, ID restaurant).
    * Il répond aux questions du questionnaire (âge, satisfaction, commentaires) de manière cohérente et positive.
4.  **Rapports et Suivi** :
    * Le résultat de chaque tentative est enregistré dans un fichier de logs (`automatisation_avis.json`).
    * Le total des avis réussis est mis à jour dans un fichier de statistiques (`stats.json`) et affiché dans l'interface graphique.
