---
title: PharmaAI Platform
emoji: 💊
colorFrom: blue
colorTo: green
sdk: streamlit
sdk_version: "1.39.0"
python_version: "3.11"
app_file: app.py
pinned: false
---
# 💊 PharmaAI Platform

A unified AI-powered document intelligence platform for pharmaceutical, regulatory, and compliance-focused workflows.

PharmaAI Platform brings together grounded retrieval, structured summarization, and compliance-oriented guidance in a single modular workspace designed to reflect enterprise-style product thinking for regulated environments.

---

## Problem

Pharmaceutical and regulated teams work with large volumes of SOPs, guidelines, policies, and quality documents that are often difficult to search, review, and interpret efficiently.

Common challenges include:
- slow manual document review
- fragmented workflows across multiple tools
- difficulty extracting actionable information from long PDFs
- limited traceability in AI-assisted workflows
- lack of structured review and approval support

---

## Solution

PharmaAI Platform is a modular AI workspace that supports document-grounded question answering, structured summarization, and compliance-oriented review support.

The platform combines:
- **PharmaRAG** for grounded pharma and regulatory Q&A
- **PharmaSummarizer** for structured document summarization
- **CompliBot** for SOP and compliance-focused guidance

It also includes workflow-oriented features such as traceability metadata, audit logging, and review queue foundations.

---

## Core Modules

### PharmaRAG
Grounded retrieval-based question answering over pharmaceutical and regulatory documents.

Typical use cases:
- What does this guideline say about GCP?
- What is pharmacovigilance according to these documents?
- What does this document say about safety communication?

### PharmaSummarizer
Structured summarization for a selected document with key highlights and extracted insights.

Typical use cases:
- summarize a regulatory guideline
- extract major highlights from a document
- generate a clean overview of a long PDF

### CompliBot
Compliance and SOP-focused assistant for evidence-backed guidance over quality documents.

Typical use cases:
- What does this SOP say about deviation handling?
- What approvals are required before closure?
- What must be documented in this process?

---

## Key Features

- Unified multi-module AI workspace
- Grounded retrieval with evidence and excerpts
- Structured single-document summarization
- Compliance-oriented question answering
- Source filtering and prepared document history
- Trace IDs and document version awareness
- Audit logging foundation
- Review queue and approval workflow foundation
- Optional LLM-ready synthesis layer

---

## Technology Stack

- **Frontend / App Layer:** Streamlit
- **Language:** Python
- **Document Parsing:** PyMuPDF (`fitz`), PyPDF
- **Embeddings:** Sentence Transformers
- **Vector Store:** ChromaDB
- **Optional LLM Layer:** Gemini-ready environment configuration
- **Local Workflow Storage:** JSONL-based audit and review records
- **Environment Management:** python-dotenv

---

## How It Works

1. Upload or prepare pharmaceutical, regulatory, or compliance documents  
2. Parse, chunk, and index document content  
3. Route the request to the appropriate module  
4. Retrieve relevant evidence or generate structured summaries  
5. Return grounded outputs with metadata, traceability, and workflow support  

---

## Project Structure

```text
pharma-ai-platform/
├── app.py
├── router.py
├── requirements.txt
├── .gitignore
├── .env.example
├── README.md
├── DEPLOYMENT_CHECKLIST.md
├── modules/
│   ├── __init__.py
│   ├── pharmarag_module.py
│   ├── pharmasummarizer_module.py
│   └── complibot_module.py
├── services/
│   ├── __init__.py
│   ├── audit_logger.py
│   ├── document_classifier.py
│   ├── document_registry.py
│   ├── engine_prep.py
│   ├── file_utils.py
│   ├── llm_client.py
│   ├── llm_config.py
│   ├── platform_health.py
│   ├── review_queue.py
│   ├── session_state.py
│   └── ui_renderers.py
├── data/
│   ├── uploads/
│   ├── audit/
│   └── review/
└── chroma_db/
```

---

## Why This Project Matters

This project demonstrates:

- modular AI system design
- retrieval-augmented workflows
- document intelligence for regulated domains
- compliance-aware product thinking
- traceability and review-oriented architecture
- enterprise-style engineering for AI applications

## Important Note

This project is a prototype/demo platform built to reflect regulated-environment design patterns. It is not a validated GxP production system.

---

## 🔗 Links & Attribution

### 🌐 Live Demo
[![Live Demo](https://img.shields.io/badge/Demo-HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/spaces/Chaitanya-Sanagana/pharma-ai-platform)

### 👤 Author
**Chaitanya Sanagana**
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Chaitanya-Sanagana)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/chaitanya-sai-sanagana-8a1827263)
