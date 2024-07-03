# Getting started

The instructions are for macOS but should work with Linux and (with small modifications) Windows, too.

Clone the repo and create a virtual environment for the project. Install required dependencies:

```bash
pip install -r requirements.txt
```

## Create and edit .env

You should create a .env file that contains at least the following:

```
# Specify LLM provider and model
LLM_PROVIDER="openai"
MODEL_NAME="gpt-4"
OPENAI_API_KEY="your-secret-key-goes-here"
# Directory for your course data:
CHAT_DATA_FOLDER ="resources" 
# Total model call quota:
TOTAL_MODEL_QUOTA=5
# Max number of tokens per call
MAX_PROMPT_TOKENS=2000
# Capacity management:
MAX_CONCURRENCY=2
MAX_QUEUE=10
```

# Launch the app

Run:

```bash
gradio app.py
```

Once the app is running, it will tell you the address where you can find the chatbot interface.
