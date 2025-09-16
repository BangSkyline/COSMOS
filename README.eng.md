# 🌌 COSMOS Project

Welcome to **COSMOS**, an ambitious simulation of a fictional company, *Cosmos.Corp*, specializing in **new technologies**: artificial intelligence (AI), fine-tuning, data science, web development, server, and database management. This project aims to recreate a complete infrastructure, from physical to virtual environments, leveraging modern technologies like **Docker**, **Next.js**, **Python**, **JavaScript/TypeScript**, and more.

## 🚀 Project Overview

*Cosmos.Corp* is a fictional company excelling in creating innovative technological solutions. The project is structured around multiple **repositories** named after Greek and Roman deities, each representing a key component of the infrastructure. These components are orchestrated using **Docker** to ensure fast, scalable, and portable deployment.

### 🎯 Objectives
- Simulate a complete enterprise infrastructure, from frontend to backend.
- Integrate modern tools for authentication, CI/CD, data management, and monitoring.
- Demonstrate the use of frameworks like **Next.js** (for web applications), **Python** (for scripts and backend), and **JavaScript/TypeScript** (for dynamic interfaces).
- Provide clear documentation and instructions for deploying the infrastructure with **Docker**.

## 📚 Repository Structure

Each repository is named after a deity and corresponds to a specific component of the infrastructure:

| **Name**                     | **Technology**                     | **Description**                                                                 |
|-----------------------------|-------------------------------------|--------------------------------------------------------------------------------|
| **Helios**                  | Authentik                          | Centralized authentication system for managing identities and access.           |
| **Apollon V2**              | Next.js, TypeScript                | Dashboard for data management and visualization.                              |
| **Mercure**                 | LLDAP                              | Lightweight directory service for managing users and groups.                   |
| **Venus**                   | Vault                              | Secure management of secrets and keys for the infrastructure.                  |
| **Aphrodite Optimus**       | Next.js, TypeScript                | Web application for Cosmos.Corp's client services.                            |
| **Gaia**                    | Gitea, Jenkins                     | Code management platform (Gitea) and CI/CD pipeline (Jenkins).                |
| **Artemis**                 | Next.js, JavaScript                | Web application for specific functionalities.                                 |
| **Selene**                  | Next.js, TypeScript                | Cosmos.Corp intranet for internal collaboration.                              |
| **Hecate**                  | Next.js, TypeScript                | Web application for advanced project management.                              |
| **Mars**                    | GLPI                               | IT asset management and helpdesk system.                                      |
| **Jupiter Optimus**         | Next.js, TypeScript                | Main website for Cosmos.Corp, the company's showcase.                         |
| **Saturn**                  | -                                  | (Under development, details to come).                                         |
| **Neptune Triton**          | OpenWebUI, Ollama, n8n, Qdrant, PostgreSQL | AI and automation platform with a vector database.                   |
| **Uranus**                  | -                                  | (Under development, details to come).                                         |
| **Pluton-Charon**           | Prometheus, Grafana, Cadvisor      | Infrastructure monitoring and metrics.                                        |

## 🛠️ Prerequisites

To deploy the COSMOS infrastructure, ensure you have the following tools installed:
- **Docker** and **Docker Compose** to orchestrate services.
- **Node.js** (version 18 or higher) for projects based on **Next.js** and **TypeScript**.
- **Python** (version 3.8 or higher) for scripts and backend services.
- A code editor like **VS Code** to edit configuration files.

## 🚀 Installation and Deployment

1. **Clone the repositories**:
   ```bash
   git clone https://github.com/<repo_name>.git
   ```
   Replace `<repo_name>` with the name of the corresponding repository (Helios, Apollon V2, etc.).

2. **Set up the Docker environment**:
   Each repository contains a `docker-compose.yml` file to orchestrate services. Run:
   ```bash
   cd <repo_name>
   docker-compose up -d
   ```

3. **Customize environment variables**:
   Some services (like Venus or Helios) require `.env` files. Refer to the specific instructions in each repository.

4. **Access the applications**:
   Once the containers are running, the applications are accessible via local URLs (e.g., `http://localhost:3000` for Next.js apps).

## 🧑‍💻 Technologies Used

- **Frontend**: Next.js, JavaScript, TypeScript, Tailwind CSS
- **Backend**: Python, Node.js
- **Infrastructure**: Docker, Docker Compose
- **Authentication**: Authentik, LLDAP
- **CI/CD**: Jenkins, Gitea
- **Monitoring**: Prometheus, Grafana, Cadvisor
- **Database**: PostgreSQL, Qdrant
- **Automation**: n8n
- **AI**: OpenWebUI, Ollama
- **Secret Management**: Vault
