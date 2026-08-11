# Hi, I'm Vinod 👋

**ML engineer working on inductive bias and representation — how a constraint changes what a network learns.**

📍 Toronto, Canada · [LinkedIn](https://www.linkedin.com/in/vinod-anbalagan/) · [Hugging Face](https://huggingface.co/vinod-anbalagan) · [The Meta Gradient](https://substack.com/@vinodanbalagan)

I spent ten years forecasting demand in warehouses and grocery stores, which is a crude way of modelling a world that keeps surprising you. I learned machine learning trying to understand why those models failed, and I'm still on that question with better tools.

---

## 🔬 Current Research

**Inductive Bias & Representation** *(in progress)*

How does a constraint — built into the architecture, or into the learning rule — change what a network actually represents?

One measurement harness pointed at a sequence of probes rather than a single experiment: local learning rules first, then architectural equivariance, then world models. Built in JAX/Equinox, with a PyTorch lane reserved for reproducing published baselines before a reimplementation counts.

Run with pre-registered hypotheses, an append-only results log, and a decisions file recording reasoning rather than conclusions — so it's visible later when a decision's assumptions have expired.

`JAX` `Equinox` `PyTorch` `Mechanistic Interpretability` `Representation Learning`

---

## 📌 Selected Work

### 🌍 Multicultural Riddles Benchmark — Cohere Labs Open Science Community *(private repo)*
Cultural reasoning benchmark spanning 50+ languages and 70+ contributors.

- Cross-team coordination across data creation, evaluation, and analysis tracks
- Shipped the v1 pilot dataset on a canonical schema for downstream benchmarking
- Built tooling that turns validator output into plain-language guidance for non-technical contributors
- Open-science publication in preparation

`Python` `Pandas` `Hugging Face Datasets` `Schema Design`

### 📄 [DocuNative](https://github.com/docunative-AI/docunative) — Cohere Expedition Hackathon
Fully offline multilingual document QA for newcomers and migrants. **Pipeline lead**, 7-person team.

- End-to-end RAG: PDF extraction → BGE-M3 embeddings → ChromaDB retrieval → Tiny Aya generation → mDeBERTa hallucination verification
- 9,000+ automated evaluations across Chinese, Hindi, and Polish
- Finding: cross-lingual **embedding** quality, not LLM capability, was the primary retrieval bottleneck

`Python` `PyTorch` `ChromaDB` `BGE-M3` `Gradio`

### 📊 [Adaption Charts P2](https://huggingface.co/datasets/vinod-anbalagan/adaption-charts-p2) — Multimodal Chart Understanding
Synthetic dataset pairing business charts with visual question answering and chart-to-table extraction. 500+ downloads across versions.

Paired with a [Llama-3.2-3B LoRA adapter](https://huggingface.co/vinod-anbalagan/Llama-3.2-3B-marketing-spend-revenue-qa) fine-tuned for table-grounded QA with reasoning traces.

`LoRA/PEFT` `Multimodal` `Synthetic Data`

### 🌾 [Tamil Agricultural Advisory Dataset](https://huggingface.co/datasets/vinod-anbalagan/tamil-agri-advisory-qa) — Adaption Labs Uncharted Data Challenge
Tamil agricultural instruction dataset built from public-sector sources (Kisan Call Centre, TNAU, ICAR). [Repo](https://github.com/VinodAnbalagan/tamil-agri-dataset-)

- 187 structured records · 48 crops · 20 categories · 10 iterative submissions over six weeks
- **Grade A (9.4/10)**, honorary recognition from Sara Hooker, co-founder of Adaption Labs
- Follow-up: [11-language Indian agricultural dataset](https://huggingface.co/datasets/vinod-anbalagan/indian-agri-advice-multilingual) using a layered regex + LLM-as-judge filtering pipeline

`Python` `Pandas` `Dataset Engineering` `Multilingual NLP`

---

## ✍️ Writing — [The Meta Gradient](https://substack.com/@vinodanbalagan)

Building and breaking AI systems to understand them, with the philosophical bits left in.

- [Finding the Manifold: Where Neural Networks Land](https://vinodanbalagan.substack.com/p/finding-the-manifold-where-neural) — the geometry of optimization, visually
- [NeurIPS 2025: The Year We Admitted We Were Lost](https://vinodanbalagan.substack.com/p/neurips-2025-the-year-we-admitted) — notes on the cracks in scaling orthodoxy
- [Animals, Ghosts, and Chimeras](https://vinodanbalagan.substack.com/p/animals-ghosts-and-chimeras-the-ai) — a four-part series on the embodiment debate
- [Building the Dataset Tamil Farmers Deserve](https://vinodanbalagan.substack.com/p/building-the-dataset-tamil-farmers) — where AI fails the Global South

---

## 📚 Currently Learning

Deep learning theory through a structured reading list, and backend systems engineering in Python and Go — the parts of ML engineering that live outside the model.

---

## 🛠 Skills

| Area | Tools |
| --- | --- |
| **Languages** | Python · Go *(learning)* · SQL · Bash |
| **Research** | JAX · Equinox · PyTorch · mechanistic interpretability · experiment design · pre-registration |
| **ML / DL** | Transformers · LoRA/PEFT · state space models · scikit-learn · XGBoost · model evaluation · probability calibration |
| **NLP & Retrieval** | Hugging Face · embeddings · RAG · ChromaDB · multilingual NLP · LLM evaluation |
| **Data** | Pandas · NumPy · dataset curation · schema design · data validation · evaluation pipelines |
| **Deployment** | Docker · FastAPI · AWS · Git · Linux |

---

## 🎓 Background

- **Microcredential, Artificial Intelligence** — University of Toronto, 2025
- **M.A.Sc., Electronic & Computer Science Engineering** — University of Windsor
  *Thesis: FPGA implementation of face recognition using Eigenfaces*
- **B.E., Electronics & Communication Engineering** — Anna University

Certifications: Wolfram ML Statistical Foundations · NVIDIA AI Infrastructure & Operations · Stanford Online / Coursera ML Specialization · Azure AI-900

Before all of this: ten years in supply chain operations, procurement analysis, and process optimization.

---

*Understanding by implementing. Measuring before concluding.*
