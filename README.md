# Projet d'Automatisation d'Avis Client (McDonald's)

## Démonstration du Processus

### Aperçu Rapide

![Image](https://raw.githubusercontent.com/rakou-fr/Review-Bot-Hello-Mcdo/refs/heads/main/UggUiVO.png)

---

# Aperçu du Projet

Cette application desktop permet d'automatiser la soumission d'avis clients sur la plateforme de sondage de McDonald's.

Le projet repose sur une architecture moderne basée sur **Electron**, **React**, **Node.js** et **Puppeteer**, offrant une interface utilisateur intuitive ainsi qu'un moteur d'automatisation capable de simuler un parcours client complet.

L'objectif principal est de générer des avis cohérents en utilisant des paramètres réalistes (date, heure, tranche d'âge) afin de reproduire des comportements de fréquentation crédibles.

---

# Stack Technique

## Frontend

* React
* Electron
* HTML / CSS / JavaScript

## Backend

* Node.js
* Puppeteer

## Intégrations

* GitHub API
* GitHub Repository

## Stockage

* Fichiers JSON
* Configuration locale

---

# Architecture

```text
Electron Application
│
├── React Interface
│   ├── Dashboard
│   ├── Configuration
│   ├── Statistiques
│   └── Gestion des tâches
│
└── Node.js Backend
    │
    ├── Puppeteer Automation Engine
    ├── Planificateur
    ├── Gestionnaire de statistiques
    └── GitHub Integration
```

---

# Fonctionnalités

## Tableau de Bord

* Visualisation des statistiques
* Suivi des avis envoyés
* Historique des exécutions
* Monitoring en temps réel

## Configuration

* Gestion des ratios démographiques
* Paramétrage des pics de fréquentation
* Configuration des commentaires
* Réglage des délais d'automatisation

## Automatisation

* Lancement automatique des sessions
* Simulation de navigation utilisateur
* Remplissage des formulaires
* Gestion des scénarios d'exécution

## Reporting

* Historique complet des opérations
* Journaux détaillés
* Statistiques cumulées
* Suivi des performances

---

# Comment Ça Fonctionne ?

## 1. Planification Intelligente

L'application analyse les paramètres configurés afin de déterminer :

* La date de visite
* L'heure de visite
* La tranche d'âge cible
* Les paramètres du scénario

Ces données sont générées selon une logique de répartition personnalisable.

---

## 2. Préparation de l'Automatisation

Le moteur Node.js récupère les informations calculées et prépare le scénario d'exécution :

* Date de visite
* Heure
* Minute
* Âge
* Identifiant du restaurant

---

## 3. Exécution Puppeteer

Le moteur Puppeteer prend le contrôle d'un navigateur automatisé afin de :

* Accéder au formulaire
* Remplir les champs requis
* Répondre aux questions du questionnaire
* Soumettre l'avis

---

## 4. Suivi et Statistiques

Chaque tentative est enregistrée dans les fichiers locaux :

### Logs

```text
automatisation_avis.json
```

### Statistiques

```text
stats.json
```

Les données sont ensuite affichées directement dans l'interface React.

---

# Technologies Utilisées

| Technologie | Utilisation               |
| ----------- | ------------------------- |
| React       | Interface utilisateur     |
| Electron    | Application desktop       |
| Node.js     | Backend local             |
| Puppeteer   | Automatisation navigateur |
| GitHub API  | Intégrations GitHub       |
| JSON        | Stockage local            |
| GitHub      | Gestion du code source    |

---

# Compétences Démontrées

* Développement React
* Développement Electron
* Automatisation web avec Puppeteer
* Architecture Desktop moderne
* Communication IPC Electron
* Gestion de données JSON
* Intégration d'API externes
* Gestion des tâches asynchrones
* Monitoring et journalisation
* Gestion de projet avec GitHub

---

# Auteur

Développé par Rakou.
