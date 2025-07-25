# finance-bot
# LangChain-based Financial Assistant Bot

This project is a simple financial assistant chatbot that reads financial documents (e.g., text or PDF) and answers user queries using Retrieval-Augmented Generation (RAG) powered by LangChain and OpenAI.

---

## Features

- Reads and processes financial documents
- Converts document chunks into vector embeddings
- Retrieves relevant information to answer user queries
- Uses OpenAI API and FAISS for document search
- Includes a simple interface for testing

---

## File Structure
├── main.py # Main script (entry point)
├── test.py # Optional testing script
├── requirements.txt # Python dependencies
├── .env # Contains your API keys
├── .env.example # Sample env file for setup
├── .gitignore # Ignore venv, .env, etc.
└── venv/ # Python virtual environment (ignored)

---

## Setup Instructions

1. **Clone this repository**
```bash
git clone https://github.com/your-username/langchain-financial-bot.git
cd langchain-financial-bot

python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

pip install -r requirements.txt

OPENAI_API_KEY=your-key-here

python main.py

NOTES
If you encounter OpenAI quota errors, consider switching to local models (e.g., sentence-transformers).

The project is modular and can be extended to support PDF upload, Streamlit interface, etc.


