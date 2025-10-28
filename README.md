# Enterprise AI RAG (Basic)

Minimal Retrieval‑Augmented Generation demo with local embeddings (Sentence‑Transformers), FAISS retrieval, and Flan‑T5 generation, including simple guardrails for PII redaction and policy checks.

## Features

- Dense embeddings via all‑MiniLM‑L6‑v2 and FAISS IndexFlatIP search.
- Local generation with google/flan‑t5‑base (no API keys required).
- Simple chunking + metadata, plus citations in answers.
- Guardrails: PII redaction (email/phone/IDs) and policy‑violation blocking.

## Install

- Python 3.10+ recommended
- pip install:  
  - faiss‑cpu  
  - transformers==4.44.2  
  - accelerate  
  - sentence‑transformers==3.0.1

## Quickstart

- Open and run notebooks/enterprise_ai_rag_guardrails_Marktechpost.ipynb top‑to‑bottom.[1]
- It will: build embeddings, create a FAISS index, apply guardrails, and answer queries with citations from the local corpus.[1]

- Runs fully local; GPU is optional and auto‑detected for embeddings if available.[1]
- For larger corpora or production, consider hybrid retrieval, re‑ranking, and a vector DB service.[1]

## License

- MIT (suggested). Adjust as needed for your org.[1]

[1](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/83997507/57beb504-faf9-4ee3-9933-f9a9932f1f7a/enterprise_ai_rag_guardrails_Marktechpost.ipynb)
