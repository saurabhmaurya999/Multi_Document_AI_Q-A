# Multi-Document AI Q&A — Flask UI

This Flask UI wraps the RAG workflow from the uploaded notebook:
PDF upload -> PyPDFLoader -> RecursiveCharacterTextSplitter (500/100) ->
all-MiniLM-L6-v2 embeddings -> FAISS -> MMR retrieval -> Qwen3 via Hugging Face.

## Run

1. Create/activate a virtual environment.
2. Install dependencies:
   `pip install -r requirements.txt`
3. Set your Hugging Face token as an environment variable.

Windows PowerShell:
`$env:HF_TOKEN="YOUR_HUGGING_FACE_TOKEN"`

Windows CMD:
`set HF_TOKEN=YOUR_HUGGING_FACE_TOKEN`

Linux/macOS:
`export HF_TOKEN="YOUR_HUGGING_FACE_TOKEN"`

4. Start:
   `python app.py`
5. Open:
   `http://127.0.0.1:5000`

Do not hard-code your Hugging Face token into the source code.
"# Multi_Document_AI_Q-A" 
