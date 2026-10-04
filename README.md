# AIQ Assistant

> Adaptive Intelligence for Private, Offline, Evidence-Grounded Q&A.

## Overview

AIQ Assistant is a phone-first, privacy-focused AI assistant concept designed to answer questions using knowledge available on the device.

Instead of using the same amount of AI computation for every request, AIQ first understands the question and dynamically selects the smallest suitable level of intelligence.

### Core pipeline

**Understand → Route → Retrieve → Reason → Verify → Answer**

## Key Features

- 🔒 Privacy-focused local AI design
- 📴 Offline-first core Q&A workflow
- 🧠 Adaptive intelligence routing
- 📚 Local Retrieval-Augmented Generation (RAG)
- ⚡ Lightweight processing for simple questions
- 🔎 Deeper local reasoning for complex questions
- ✅ Evidence-based answer verification
- 🎤 Text and voice interaction concept
- 📊 Processing and system insights
- 🌙 Dark/light interface
- 📱 Phone-first design

## Three Intelligence Levels

| Level | Processing | Typical Use |
|---|---|---|
| L1 | SLM Router | Intent, topic and complexity detection |
| L2 | SLM + Local RAG | Direct lookup, simple Q&A and summarization |
| L3 | Local LLM + Local RAG | Comparison, interpretation and multi-step reasoning |

## Architecture

```text
User Question
      ↓
L1 — SLM Intent & Complexity Classifier
      ↓
Adaptive Router
   ↙       ↘
Simple     Complex
  ↓           ↓
L2 — SLM    L3 — Local LLM
+ Local RAG  + Local RAG
   ↘         ↙
   Verification Layer
          ↓
Final Answer + Evidence
```

## Current Prototype

This repository currently contains an interactive frontend prototype demonstrating the AIQ concept, adaptive routing flow, local knowledge interface, evidence display, demo mode, and system insights.

The current prototype uses simulated/mock responses for demonstration. It does not yet implement a production local LLM, real document indexing pipeline, or production RAG backend.

## Technology

- HTML5
- CSS3
- JavaScript
- Local AI / SLM / LLM architecture concept
- Retrieval-Augmented Generation (RAG) concept
- Evidence verification concept

## Project Structure

```text
AIQ-Assistant/
├── index.html
├── README.md
├── LICENSE
├── .gitignore
├── docs/
└── assets/
    └── screenshots/
```

## Future Scope

- Real local SLM integration
- Real local LLM integration
- Local document ingestion and indexing
- Vector search / local knowledge store
- On-device embeddings
- Real evidence verification
- Smartphone CPU/GPU/NPU optimization
- Latency, memory and energy evaluation
- Fully functional offline Q&A pipeline

## Demo

The frontend prototype can be deployed as a static website using Netlify or GitHub Pages.

## Important Design Boundary

"Offline" refers to the intended core Q&A pipeline when the required models, indexes, documents and inference components are installed locally. Model installation, updates, or optional cloud features may require connectivity.

## License

MIT License
