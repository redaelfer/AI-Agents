# AI Agent 🤖

**ai-agents** est un assistant intelligent local conçu pour la supervision de système et l'analyse de documents. Il utilise le modèle **Llama 3.2** via **Ollama** pour interagir avec votre système d'exploitation et traiter vos fichiers en toute confidentialité.

## 🌟 Fonctionnalités

* **Supervision Système** : Monitoring en temps réel de l'utilisation du processeur (CPU) et de la mémoire vive (RAM).
* **Analyse de Documents** : Lecture, extraction et résumé structuré de fichiers aux formats `.txt`, `.py`, `.md`, `.pdf` et `.docx`.
* **Gestionnaire de Tâches** : Ajout et consultation de rappels enregistrés localement dans un fichier `reminders.txt`.
* **Triage d'Emails** : Module de classification et de résumé automatique des courriels.
* **Exploration de Fichiers** : Capacité de lister le contenu des répertoires et de lire des fichiers spécifiques via des commandes naturelles.

## 🛠️ Architecture Technique

Le projet repose sur une architecture hybride combinant discussion libre (Chatbot) et exécution de fonctions (Agent) :

* **Interface Utilisateur** : Développée avec **Streamlit** pour une expérience interactive.
* **Cœur IA** : Orchestration via **Ollama** avec support du "Tool Calling" pour exécuter des scripts Python.
* **Modules** :
* `summarize.py` : Logique de traitement des documents et triage des emails.
* `monitor.py` : Fonctions de monitoring système et gestion des rappels.
* `app.py` : Point d'entrée de l'application et gestion du flux de conversation.



## 🚀 Installation et Lancement

### 1. Prérequis

* [Ollama](https://ollama.com/) installé avec le modèle `llama3.2`.
* Python 3.10 ou supérieur.

### 2. Installation des dépendances

Activez votre environnement virtuel et installez les bibliothèques requises :

```bash
pip install -r requirements.txt

```

*Les dépendances incluent notamment `psutil`, `PyPDF2`, `python-docx`, `streamlit` et `ollama`.*

### 3. Exécution

Lancez l'interface utilisateur avec la commande suivante :

```bash
streamlit run app.py

```

## 📂 Structure du Projet

* `app.py` : Interface principale et logique de l'agent superviseur.
* `summarize.py` : Outils d'analyse de documents et simulation de messagerie.
* `monitor.py` : Outils de monitoring système et gestion des rappels.
* `requirements.txt` : Liste des dépendances Python.
