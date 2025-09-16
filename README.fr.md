# 🌌 Projet COSMOS

Bienvenue dans **COSMOS**, une simulation ambitieuse d'une entreprise fictive, *Cosmos.Corp*, spécialisée dans les **nouvelles technologies** : intelligence artificielle (IA), fine-tuning, data science, développement web, gestion de serveurs et bases de données. Ce projet vise à recréer une infrastructure complète, de l'environnement physique au virtuel, en s'appuyant sur des technologies modernes comme **Docker**, **Next.js**, **Python**, **JavaScript/TypeScript**, et bien plus encore.

## 🚀 Aperçu du projet

*Cosmos.Corp* est une entreprise fictive qui excelle dans la création de solutions technologiques innovantes. Le projet est structuré autour de multiples **repositories** nommés d'après des divinités grecques et romaines, chacun représentant un composant clé de l'infrastructure. Ces composants sont orchestrés via **Docker** pour garantir une mise en place rapide, scalable et portable.

### 🎯 Objectifs
- Simuler une infrastructure d'entreprise complète, du frontend au backend.
- Intégrer des outils modernes pour l'authentification, la CI/CD, la gestion de données, et la surveillance.
- Démontrer l'utilisation de frameworks comme **Next.js** (pour les applications web), **Python** (pour les scripts et backend), et **JavaScript/TypeScript** (pour des interfaces dynamiques).
- Fournir une documentation claire et des instructions pour déployer l'infrastructure avec **Docker**.

## 📚 Structure des repositories

Chaque repository est nommé d'après une divinité et correspond à un composant spécifique de l'infrastructure :

| **Nom**                     | **Technologie**                     | **Description**                                                                 |
|-----------------------------|-------------------------------------|--------------------------------------------------------------------------------|
| **Hélios**                  | Authentik                          | Système d'authentification centralisé pour gérer les identités et l'accès.     |
| **Apollon V2**              | Next.js, TypeScript                | Tableau de bord (dashboard) pour la gestion et la visualisation des données.   |
| **Mercure**                 | LLDAP                              | Service d'annuaire léger pour la gestion des utilisateurs et groupes.          |
| **Vénus**                   | Vault                              | Gestion sécurisée des secrets et des clés pour l'infrastructure.               |
| **Aphrodite Optimus**       | Next.js, TypeScript                | Application web pour les services clients de Cosmos.Corp.                     |
| **Gaïa**                    | Gitea, Jenkins                     | Plateforme de gestion de code (Gitea) et pipeline CI/CD (Jenkins).            |
| **Artémis**                 | Next.js, JavaScript                | Application web pour des fonctionnalités spécifiques.                          |
| **Sélénée**                 | Next.js, TypeScript                | Intranet de Cosmos.Corp pour la collaboration interne.                         |
| **Hécate**                  | Next.js, TypeScript                | Application web pour la gestion de projets avancés.                           |
| **Mars**                    | GLPI                               | Gestion des actifs informatiques et helpdesk.                                 |
| **Jupiter Optimus**         | Next.js, TypeScript, Python        | Site web principal de Cosmos.Corp, vitrine de l'entreprise.                   |
| **Saturne**                 | -                                  | (En cours de développement, détails à venir).                                  |
| **Neptune Triton**          | OpenWebUI, Ollama, n8n, Qdrant, PostgreSQL | Plateforme d'IA et d'automatisation avec base de données vectorielle. |
| **Uranus**                  | -                                  | (En cours de développement, détails à venir).                                  |
| **Pluton-Charon**           | Prometheus, Grafana, Cadvisor      | Surveillance et métriques de l'infrastructure.                                 |

## 🛠️ Prérequis

Pour déployer l'infrastructure COSMOS, assurez-vous d'avoir les outils suivants installés :
- **Docker** et **Docker Compose** pour orchestrer les services.
- **Node.js** pour les projets basés sur **Next.js** et **TypeScript** et **JavaScript**.
- **Python** (version 3.8 ou supérieure) pour les scripts et services backend.
- Un éditeur de code comme **VS Code** pour modifier les fichiers de configuration.

## 🚀 Installation et déploiement

1. **Cloner les repositories** :
   ```bash
   git clone https://github.com/CosmosCorp/<nom_du_repo>.git
   ```

2. **Configurer l'environnement Docker** :
   Chaque repository contient un fichier `docker-compose.yml` pour orchestrer les services. Lancez :
   ```bash
   cd <nom_du_repo>
   docker-compose up -d
   ```

3. **Personnaliser les variables d'environnement** :
   Certains services nécessitent des fichiers `.env`. Consultez les instructions spécifiques dans chaque repository.

4. **Accéder aux applications** :
   Une fois les conteneurs lancés, les applications sont accessibles via des URL locales (ex. : `http://localhost:3000` pour les apps Next.js).

## 🧑‍💻 Technologies utilisées

- **Frontend** : Next.js, JavaScript, TypeScript, Tailwind CSS
- **Backend** : Python, Node.js
- **Infrastructure** : Docker, Docker Compose
- **Authentification** : Authentik, LLDAP
- **CI/CD** : Jenkins, Gitea
- **Surveillance** : Prometheus, Grafana, Cadvisor
- **Base de données** : PostgreSQL, Qdrant
- **Automatisation** : n8n
- **IA** : OpenWebUI, Ollama
- **Gestion des secrets** : Vault
