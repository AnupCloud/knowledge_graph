# Knowledge Graph Generator

A Python-based tool for generating and visualizing knowledge graphs using LangChain and OpenAI. This project helps in creating interactive knowledge graphs from text data, with a user-friendly web interface built using Streamlit.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.13+](https://img.shields.io/badge/python-3.13+-blue.svg)](https://www.python.org/downloads/)

## Project Insights

### Overview
This project is a sophisticated knowledge graph generator that leverages the power of Large Language Models (LLMs) to create meaningful connections between concepts from text data. The system uses LangChain and OpenAI to process text and generate structured knowledge graphs that can be visualized and explored interactively.

### Key Components

1. **Text Processing Pipeline**
   - Utilizes LangChain for text processing and entity extraction
   - Implements OpenAI's language models for understanding context and relationships
   - Processes text in chunks for efficient handling of large documents

2. **Knowledge Graph Generation**
   - Extracts entities and relationships from processed text
   - Creates nodes and edges based on semantic understanding
   - Supports multiple relationship types and entity categories

3. **Visualization System**
   - Interactive graph visualization using Pyvis
   - Customizable node and edge properties
   - Export functionality to HTML format
   - Real-time graph updates and modifications

4. **Web Interface**
   - Streamlit-based user interface
   - Real-time graph generation and updates
   - Interactive parameter controls
   - Responsive design for various screen sizes

### Technical Architecture

## Features

- Generate knowledge graphs from text input using LangChain and OpenAI
- Interactive web interface using Streamlit
- Visualize knowledge graphs using Pyvis
- Export graphs to HTML format
- Support for custom graph generation parameters

## Prerequisites

- Python 3.13 or higher
- OpenAI API key
- UV package installer (recommended)

## Installation

### Using UV (Recommended)

1. Install UV if you haven't already:
```bash
# For macOS/Linux
curl -LsSf https://astral.sh/uv/install.sh | sh

# For Windows (PowerShell)
(Invoke-WebRequest -Uri "https://astral.sh/uv/install.ps1" -UseBasicParsing).Content | pwsh -Command -
```

2. Clone the repository:
```bash
git clone https://github.com/AnupCloud/knowledge_graph.git
cd knowledge_graph
```

3. Create and activate a virtual environment using UV:
```bash
# Create virtual environment
uv venv

# Activate virtual environment
# On macOS/Linux:
source .venv/bin/activate
# On Windows:
.venv\Scripts\activate
```

4. Install dependencies using UV:
```bash
# Install all dependencies
uv add -r requirements.txt

```

5. **Development Workflow**
   ```bash
   # Add a new dependency
   uv add package_name

   # Install development dependencies
   uv add -r requirements.txt

   # Update all packages
   uv add --upgrade -r requirements.txt
   ```

## Environment Setup

1. Create a `.env` file in the project root directory
2. Add your OpenAI API key:

## Project Structure

```
knowledge_graph/
├── src/
│   ├── app.py                 # Streamlit web application
│   ├── generate_knowledge_graph.py  # Core graph generation logic
│   └── knowledge_graph.ipynb  # Jupyter notebook for development
├── requirements.txt           # Project dependencies
├── pyproject.toml            # Project configuration
└── README.md                 # This file
```

## Running the Application

### Using UV

1. Make sure you're in the project directory and your virtual environment is activated:
```bash
source .venv/bin/activate  # On Windows, use `.venv\Scripts\activate`
```

2. Start the Streamlit application:
```bash
streamlit run src/app.py
```

3. Open your web browser and navigate to the provided local URL (typically http://localhost:8501)


### Core Dependencies
- langchain >= 0.1.0
- langchain-experimental >= 0.0.45
- langchain-openai >= 0.1.0
- python-dotenv >= 1.0.0
- pyvis >= 0.3.2
- streamlit >= 1.32.0


## Acknowledgments

- LangChain for the LLM framework
- OpenAI for the language model
- Streamlit for the web interface
- Pyvis for graph visualization
- UV for fast Python package management