# 🌌 Projet COSMOS

Bienvenue dans **COSMOS**, une simulation d'une entreprise fictive, *Cosmos.Corp*, spécialisée dans les **nouvelles technologies** : intelligence artificielle (IA), fine-tuning, data science, développement web, gestion de serveurs et bases de données. Ce projet vise à recréer une infrastructure complète, de l'environnement physique au virtuel, en s'appuyant sur des technologies modernes comme **Proxmox**, **K3s**, **Containerd** **Next.js**, **Python**, **JavaScript/TypeScript**, et bien plus encore.

## 🚀 Aperçu du projet

*Cosmos.Corp* est une entreprise fictive qui excelle dans la création de solutions technologiques innovantes. Le projet est structuré autour de multiples **repositories** nommés d'après des divinités grecques et romaines, chacun représentant un composant clé de l'infrastructure. Ces composants sont orchestrés via **K3s** pour garantir une mise en place rapide, scalable et portable.

### 🎯 Objectifs
- Simuler une infrastructure d'entreprise complète, du système au réseau.
- Intégrer des outils modernes pour l'authentification, la CI/CD, la gestion de données, et la surveillance.
- Démontrer l'utilisation de frameworks comme **Next.js** (pour les applications web), **Python** (pour les scripts et backend), et **JavaScript/TypeScript** (pour des interfaces dynamiques).
- Fournir une documentation claire et des instructions pour déployer l'infrastructure avec **Containerd**, **Docker**, puis **K3s**.

---

## 🧑‍💻 Technologies utilisées

- **Frontend** : Next.js, JavaScript, TypeScript, Tailwind CSS
- **Backend** : Python, Node.js
- **Infrastructure** : Proxmox, PfSense, K3s, Chartes Helm, Containerd, Docker, Docker Compose
- **Authentification** : Authentik, LLDAP
- **CI/CD** : Jenkins, Gitea
- **Surveillance** : Prometheus, Grafana, Cadvisor
- **Base de données** : PostgreSQL, Qdrant
- **Automatisation** : n8n
- **IA** : OpenWebUI, Ollama
- **Gestion des secrets** : Vault

---

## 📚 Structure des repositories

Chaque repository est nommé d'après une divinité et correspond à un composant spécifique de l'infrastructure :

| **Nom du repo**                     | **Technologie**            | **Description**                                                                 |
|-----------------------------|------------------------------------|--------------------------------------------------------------------------------|
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
| **Saturne**                 | -                                  | Web App de monitoring des conteneurs via branchement à un proxy du socket docker.                                  |
| **Neptune Triton**          | OpenWebUI, Ollama, n8n, Qdrant, PostgreSQL | Plateforme d'IA et d'automatisation avec base de données vectorielle. |
| **Uranus**                  | -                                  | Drive intranet .                                  |
| **Pluton-Charon**           | Prometheus, Grafana, Cadvisor      | Surveillance et métriques de l'infrastructure.                                 |

---

## 🐳 Utilisation de Docker Swarm

- **Installation via Portainer** : L'environnement Docker Swarm est installé et géré via **Portainer**, un outil open-source pour la gestion de conteneurs. Portainer facilite le déploiement de Swarm et active le **cryptage des réseaux overlay** par défaut, assurant une communication sécurisée entre les nœuds du cluster.
- **Réseaux personnalisés MacVLAN** : Pour éviter les conflits de ports et ne pas exposer les services via NAT (Network Address Translation), nous utilisons des réseaux **MacVLAN**. Cela permet aux conteneurs d'obtenir des adresses IP et MAC directement sur le réseau physique de l'hôte, simulant des machines virtuelles indépendantes. Cela améliore la sécurité en évitant l'exposition directe des ports et facilite l'intégration avec des réseaux existants.
- **Simulation d'un environnement de développement** : Docker Swarm est utilisé ici pour simuler un environnement de développement multi-nœuds, scalable et résilient. Cela prépare une transition fluide vers **Kubernetes** en production, où des outils comme Helm ou Kustomize peuvent être adoptés pour une orchestration plus avancée. En dev, Swarm offre une courbe d'apprentissage plus douce tout en supportant des features comme les services réplicables et les stacks.

---

## ⚡ Évolutions et améliorations suggérées

Pour faire évoluer le projet COSMOS vers une maturité production-ready, voici quelques suggestions :
- **Mise en place de Kubernetes** : Une fois l'environnement dev stabilisé avec Swarm, mettre en place Kubernetes pour une orchestration pour la production. Utilisation des outils comme `kompose` pour convertir les fichiers `docker-compose.yml` en manifests Kubernetes.
- **Automatisation avancée** : Ajoutez des pipelines CI/CD plus complexes avec Jenkins pour des tests automatisés.
- **Sécurité renforcée** : Implémentez des scans de vulnérabilités avec Trivy sur les images Docker, et activez Docker Content Trust pour signer les images.
- **Scalabilité horizontale** : Tester la réplication de services critiques (ex. : bases de données avec PostgreSQL en cluster) et intégrer des outils comme Elasticsearch pour la recherche distribuée.
- **Monitoring étendu** : Étendre Grafana avec des alertes via Alertmanager.
- **IA et ML** : Améliorer Neptune Triton en intégrant des modèles ML personnalisés avec TensorFlow ou PyTorch, et explorer le fine-tunings via Hugging Face.

---

## 🛠️ Prérequis

Pour déployer l'infrastructure COSMOS, assurez-vous d'avoir les outils suivants installés :
- **Docker** et **Docker Compose** pour orchestrer les services.
- **Node.js** pour les projets basés sur **Next.js** et **TypeScript** et **JavaScript**.
- **Python** (version 3.8 ou supérieure) pour les scripts et services backend.
- Un éditeur de code comme **VS Code** pour modifier les fichiers de configuration.
