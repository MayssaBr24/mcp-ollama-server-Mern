# Serveur MCP avec Ollama

##  Description
Serveur MCP (Model Context Protocol) permettant aux agents IA d'interagir avec des APIs backend via Ollama. Ce projet implémente un serveur MCP standard avec des outils pour la gestion d'utilisateurs.

## Fonctionnalités
- Serveur MCP conforme aux spécifications
- Intégration avec Ollama pour exécution locale de LLMs
- Outils disponibles:
  - `getListUsers`: Récupère tous les utilisateurs
  - `list-users`: Filtre les utilisateurs par prénom
- Compatible avec MCP Inspector pour le débogage
- Validation des paramètres avec Zod

##  Architecture
Frontend → Backend Express (port 3001)
↓
Serveur MCP (ce projet) → Ollama (port 11434)
↓
API Utilisateurs

##  Relation avec d'autres projets

**Ce projet est conçu pour fonctionner avec:**
- [Backend API]](https://github.com/MayssaBr24/MernECommerce)- L'API utilisateurs sur le port 3001
- [Frontend Application]

> **Note importante:** Ce serveur MCP dépend d'une API backend existante. Assurez-vous que le backend est en cours d'exécution sur `localhost:3001` avant de démarrer ce serveur.

## Prérequis
- Node.js 24
- Ollama installé localement
- Modèle Llama téléchargé (ex: `ollama pull llama3.1:8b`)
- Le [backend API](https://github.com/[votre-username]/[backend-repo-name]) en cours d'exécution


