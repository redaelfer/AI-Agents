# AI Agent 

**ai-agents** is a local intelligent assistant designed for system supervision and document analysis. It utilizes the **Llama 3.2** model via **Ollama** to interact with your operating system and process your files with full confidentiality.

## 🌟 Features

* **System Supervision**: Real-time monitoring of CPU and RAM usage.
* **Document Analysis**: Reading, extraction, and structured summarization of files in `.txt`, `.py`, `.md`, `.pdf`, and `.docx` formats.
* **Task Manager**: Adding and viewing reminders stored locally in a `reminders.txt` file.
* **Email Triage**: Automatic classification and summarization module for emails.
* **File Exploration**: Ability to list directory contents and read specific files using natural language commands.

## 🛠️ Technical Architecture

The project is based on a hybrid architecture combining free-form discussion (Chatbot) and function execution (Agent):

* **User Interface**: Developed with **Streamlit** for an interactive experience.
* **AI Core**: Orchestrated via **Ollama** with "Tool Calling" support to execute Python scripts.
* **Modules**:
* `summarize.py`: Logic for document processing and email triage.
* `monitor.py`: System monitoring functions and reminder management.
* `app.py`: Application entry point and conversation flow management.



## Installation and Launch

### 1. Prerequisites

* [Ollama](https://ollama.com/) installed with the `llama3.2` model.
* Python 3.10 or higher.

### 2. Dependency Installation

Activate your virtual environment and install the required libraries:

```bash
pip install -r requirements.txt

```

*Dependencies notably include `psutil`, `PyPDF2`, `python-docx`, `streamlit`, and `ollama`.*

### 3. Execution

Launch the user interface with the following command:

```bash
streamlit run app.py

```

## 📂 Project Structure

* `app.py`: Main interface and supervisor agent logic.
* `summarize.py`: Document analysis and messaging simulation tools.
* `monitor.py`: System monitoring and reminder management tools.
* `requirements.txt`: List of Python dependencies.
