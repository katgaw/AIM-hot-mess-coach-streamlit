<p align="center" draggable="false"><img src="https://github.com/AI-Maker-Space/LLM-Dev-101/assets/37101144/d1343317-fa2f-41e1-8af1-1dbb18399719" width="200px" height="auto"/></p>

## <h1 align="center" id="heading"> 👋 Hot Mess Coach — Simple LLM App</h1>

A tiny Streamlit app with a minimal UI that calls the OpenAI Chat Completions API, with optional PDF/CSV upload.

### Quick Start

```bash
uv init
uv sync
export OPENAI_API_KEY=sk-...   # required
uv run streamlit run api/index.py --server.address 0.0.0.0 --server.port 8501
```

Open http://localhost:8501

## Run locally

### Option A: Using uv (recommended)
1) Create and activate a local venv
```bash
uv init --python 3.12
uv sync
```
2) Install deps
```bash
uv sync
```
3) Set your API key (or use a `.env` file with `OPENAI_API_KEY=...`)
```bash
export OPENAI_API_KEY="sk-..."
```
4) Start the app
```bash
uv run streamlit run api/index.py --server.address 0.0.0.0 --server.port 8501
```
Open http://localhost:8501

### Option B: Using venv + pip
1) Create and activate venv
```bash
python3 -m venv .venv
source .venv/bin/activate
```
2) Install deps
```bash
pip install -U pip
pip install streamlit openai python-dotenv PyPDF2 pandas
```
3) Set your API key (or use a `.env` file with `OPENAI_API_KEY=...`)
```bash
export OPENAI_API_KEY="sk-..."
```
4) Start the app
```bash
streamlit run api/index.py --server.address 0.0.0.0 --server.port 8501
```
Open http://localhost:8501

Notes:
- You can place a `.env` file at the repo root with `OPENAI_API_KEY=...`.
- The app entrypoint is `api/index.py` (Streamlit).


