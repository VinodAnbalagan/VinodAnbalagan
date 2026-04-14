# Vinod Anbalagan
**ML Engineer & Researcher** | Operations → AI | Efficient Architectures for Reasoning

---

## About

I optimize systems under constraints. Whether managing supply chains or training neural networks, the goal is the same: **maximum performance, minimum waste**.

**Background:** 10+ years in operations and supply chain → systematic pivot to AI/ML engineering and research (2024–present)

**Research focus:** I'm interested in how intelligence emerges from structure rather than scale. Specifically: architectures that reason iteratively rather than in a single forward pass, where the answer emerges from an internal simulation, not a lookup. My current thread runs through object-centric representations, state space models, and geometric deep learning as building blocks for more efficient, interpretable reasoning systems.

---

## Current Work

### DocuNative — Cohere Expedition Hackathon (March 2026)
Privacy-first, fully offline cross-lingual document QA for migrants and newcomers. Upload a foreign legal document, ask questions in your own language, get answers with source citations and a hallucination trust score — entirely on-device, nothing sent to the cloud.

- Pipeline lead and eval researcher on a 7-person team
- Built the full RAG pipeline: PDF extraction → BGE-M3 embeddings → ChromaDB retrieval → Tiny Aya 3.35B generation → mDeBERTa NLI hallucination check
- 9,063 automated evaluations across Chinese, Hindi, and Polish
- Key finding: the bottleneck in cross-lingual RAG isn't the language model — it's the embedding space mismatch between question and document language
- Tech: Tiny Aya GGUF · llama-server · BGE-M3 · ChromaDB · mDeBERTa · Gradio
- Repo: [Docunative](https://github.com/docunative-AI/docunative) | [Cohere-Labs-Community/docunative](https://github.com/Cohere-Labs-Community/docunative)

### Loss Landscape Visualization
Visualizing neural network optimization surfaces to understand why some architectures train better than others.
Tech: PyTorch · matplotlib · 3D surface plots

### Rethinking RNN *(In Progress)*
Implementing sequence models from scratch: RNN → LSTM → Transformer → Mamba. Analyzing gradient flow and computational complexity at each step.

Goal: understand the evolution of sequential architectures from first principles — not just that they work, but *why* they work, and what each generation was designed to fix.
Tech: PyTorch (no high-level libraries) · comparative benchmarking

---

## Production Experience

**ML Engineering Intern** | M2M Tech (2024–2025)
- Built and deployed end-to-end ML pipeline (XGBoost) for a client startup
- Feature engineering, model training, API deployment, monitoring
- Stack: Python · FastAPI · Docker · AWS

**Supply Chain & Analytics** (2017–2023)
- Optimized inventory systems — prevented $500K in stockouts
- Built predictive analytics for demand forecasting (+25% revenue impact)
- Automated reporting pipelines (saved 15 hrs/week)

---

## Technical Stack

**Deep Learning:** PyTorch · Transformers · State Space Models (Mamba) · Computer Vision · NLP  
**ML Engineering:** Docker · FastAPI · CI/CD · AWS · Hugging Face  
**Foundations:** Linear Algebra · Optimization · Probability Theory

---

## Education

**M.A.Sc. Electrical Engineering** | University of Windsor (2012)  
**B.E. Electronics & Communication** | Anna University (2008)

**Recent Training (2024–2025)**
- University of Toronto: ML & Data Science Professional Certificate
- Stanford: Machine Learning Specialization (Andrew Ng)
- Google: Advanced Data Analytics

---

## Writing

**[The Meta Gradient](https://substack.com/@vinodanbalagan)** — technical writing on architecture evolution, deep learning fundamentals, and the philosophical rabbit holes these lead me down.

---

## Connect

[LinkedIn](https://www.linkedin.com/in/vinod-anbalagan/) · [Email](mailto:vinodanbalagan@gmail.com) · [Substack](https://substack.com/@vinodanbalagan)

---

*"Intelligence emerges from constraints, not just compute."*
