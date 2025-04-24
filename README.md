# 🧠 Multi-Tool Chatbot with LangGraph and LangChain

This project builds a **conversational AI assistant** capable of intelligently using external tools like Wikipedia and Arxiv to answer complex queries. It uses **LangChain**, **LangGraph**, and **Grok/Mistral LLMs** hosted via `langchain-groq`.

## 📌 Features

- 🌐 **Tool Integration**: Automatically invokes tools like Wikipedia and Arxiv for research-style questions.
- 🔁 **Graph-Based Reasoning**: Uses LangGraph to define stateful workflows for better decision-making.
- 🧠 **LLM-Powered**: Backed by powerful LLMs (Mistral 7B via Groq).
- 🔍 **Multi-step Reasoning**: Each query is passed through a series of nodes (graph) to determine the right course of action.

---

## 🧰 Tech Stack

| Tool            | Purpose                                       |
|-----------------|-----------------------------------------------|
| `langchain`     | LLM orchestration and tool binding            |
| `langgraph`     | Workflow logic via graph-based state machine  |
| `langchain-groq`| LLM support using Groq API (Mistral models)   |
| `pydantic`      | Input/output validation                       |
| `arxiv`, `wikipedia` | Toolkits used to fetch external knowledge |
| `python-dotenv` | Load environment variables securely           |

---

## 🚀 Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/multitool-chatbot
   cd multitool-chatbot

2. **Install dependencies**:   
```bash
pip install -r requirements.txt
```

3. **Set up environment variables: Create a .env file with the following keys**:
```
GROQ_API_KEY=your_groq_api_key
```

4. **Run the Notebook: Launch Jupyter or VSCode and open chatbotmultipletoos.ipynb**.


## 🧪 Example Use Cases
"Search for recent papers on quantum computing from Arxiv."

"What is LangGraph? Use Wikipedia for details."

"Explain the difference between LangChain and LangGraph."

## 📚 Based On
This project follows the structure taught in Krish Naik's LangGraph Course, extending it with additional tools and structured graph-based logic.

## 🛠️ Future Enhancements
 Add more tools (e.g., Wolfram Alpha, YouTube search)

 Add memory and conversation context using LangChain memory

 Build a Streamlit or web-based frontend

 Deploy via Docker or Hugging Face Spaces

