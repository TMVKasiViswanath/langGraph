
## Setup Instructions

### 1. Clone the Repository
```bash
git clone <repository-url>
cd LangGraph
```

### 2. Create Virtual Environment
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate

# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Environment Variables Setup
Create a `.env` file in the root directory:

```bash
# Create .env file
touch .env  # On Windows: type nul > .env
```

Add your OpenAI API key to the `.env` file:
```env
OPENAI_API_KEY=your_openai_api_key_here
```

### 5. Verify Installation
```bash
python -c "import langgraph; print('LangGraph installed successfully!')"
```

## Project Components

### Agents
- **Agent_Bot.py**: Main agent implementation
- **Drafter.py**: Drafting and content generation agent
- **Memory_Agent.py**: Agent with memory capabilities
- **RAG_Agent.py**: Retrieval-Augmented Generation agent
- **ReAct.py**: Reasoning and Acting agent

### Graphs
Jupyter notebooks demonstrating various LangGraph workflows:
- Conditional agent processing
- Basic workflows
- Loop-based processing
- Multi-input handling
- Sequential agent chains

## Usage

1. Ensure your virtual environment is activated
2. Set up your `.env` file with OpenAI API key
3. Run any of the agent scripts or Jupyter notebooks in the `Graphs/` directory

## Dependencies

The project uses the following main dependencies:
- `langgraph`: Core LangGraph framework
- `langchain`: LangChain framework
- `langchain_openai`: OpenAI integration
- `langchain_community`: Community integrations
- `chromadb`: Vector database
- `ipython`: Interactive Python shell
- `python-dotenv`: Environment variable management

## Notes

- Always activate your virtual environment before running the project
- Keep your `.env` file secure and never commit it to version control
- The `venv/` directory should be added to `.gitignore`