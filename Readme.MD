# Hi, I'm Vinod 👋

**ML engineer and independent researcher working on representation learning, multimodal AI, and world models. I’m interested in a simple question: when a model succeeds, has it learned the structure of the problem, or the surface cues that happen to correlate with it?**

🔬 **I'm looking to join research groups working on world models, representation learning, and multimodal learning, through research engineering, research assistantships, internships, or funded MS/PhD positions.** If you lead a lab or research group and think my work might fit, I'd be glad to hear from you.

📍 Toronto, Canada · [LinkedIn](https://www.linkedin.com/in/vinod-anbalagan/) · [Hugging Face](https://huggingface.co/vinod-anbalagan) · [The Meta Gradient](https://substack.com/@vinodanbalagan) · [Website](https://vinodanbalagan.vercel.app/)

I spent ten years forecasting demand in warehouses and grocery stores, which is a crude way of modelling a world that keeps surprising you. I learned machine learning trying to understand why those models failed, and I am still on that question with better tools.

---

## 🔭 What I'm working on

**Multicultural Riddles Benchmark** · Cohere Labs Open Science Community · *first author, paper in preparation*
A cultural-reasoning benchmark spanning **51 languages and ~6,100 riddles**, built with ~100 contributors. Riddles are a setting where surface fluency and genuine understanding come apart sharply: a model can produce perfect Tamil and still miss what a Tamil riddle is actually about.

**Reverie: does a world model represent what it cannot see?** · *in progress*

---

## 📌 Selected work

### 🌍 Cultural Riddles Benchmark
Cohere Labs Open Science Community · **First author** · Apr 2026 to present · *(repo private until publication)*

- Lead the data, publishing, and analysis infrastructure for a multilingual cultural-reasoning benchmark of ~6,100 natively written, human-evaluated riddles across 61 communities and 51 languages (paper in preparation).
- Built the self-serve contribution pipeline: fork-based submissions auto-validated on each pull request via GitHub Actions, plus a one-command publisher that rebuilds the dataset and ships versioned releases to Hugging Face with contributor credits and ISO language codes, so the benchmark keeps growing after release without the core team.
- Built a public results dashboard on Hugging Face Spaces with per-model, per-culture, difficulty, and error-type views, every figure reconciled to the human-evaluation source data.
- Owned data integrity across 30 evaluated models: caught scoring-definition and coverage issues that were inflating results, added automated reconciliation checks, and ran an annotation audit that led to re-validating a community whose scores were unreliable.
- Coordinated ~100 contributors across writing, validation, and evaluation on shared schema, validation rules, and release requirements, and built Python tooling that turns validator output into contributor-ready feedback to speed up review.

`Python` `Pandas` `Hugging Face Datasets` `schema design` `LLM evaluation`

### 📊 Adaption Labs AutoScientist Challenge
**2nd place, $1,000 USD** · Data & Visualization track · 2026

- **[Adaption Charts P2](https://huggingface.co/datasets/vinod-anbalagan/adaption-charts-p2)**: synthetic multimodal dataset for chart QA and chart-to-table extraction, designed to raise difficulty through varied chart styles, truncated axes, and reduced dependence on superficial visual cues
- Paired **[Llama-3.2-3B LoRA adapter](https://huggingface.co/vinod-anbalagan/Llama-3.2-3B-marketing-spend-revenue-qa)** fine-tuned for table-grounded QA with reasoning traces

`LoRA/PEFT` `multimodal` `synthetic data` `evaluation design`

### 📄 [DocuNative](https://github.com/docunative-AI/docunative)
Cohere Expedition Hackathon · **Pipeline lead**, 7-person team, one week

Fully offline multilingual document QA for newcomers and migrants. Nothing leaves the user's machine.

- End-to-end RAG: PDF extraction → BGE-M3 embeddings → ChromaDB retrieval → Aya generation → mDeBERTa hallucination verification
- 9,000+ automated evaluations across Chinese, Hindi, and Polish
- Finding: cross-lingual **embedding** quality, not LLM capability, was the primary retrieval bottleneck

`Python` `PyTorch` `ChromaDB` `BGE-M3` `Gradio`

### 🌾 [Tamil Agricultural Advisory Dataset](https://huggingface.co/datasets/vinod-anbalagan/tamil-agri-advisory-qa)
Adaption Labs Uncharted Data Challenge · **Grade A (9.4/10)** · [repo](https://github.com/VinodAnbalagan/tamil-agri-dataset-)

Tamil agricultural instruction dataset built from public-sector sources (Kisan Call Centre, TNAU, ICAR). 187 curated records, 48 crops, 20 categories, 10 iterative submissions over six weeks. Honorary recognition from Sara Hooker.

Follow-up: **[11-language Indian agricultural dataset](https://huggingface.co/datasets/vinod-anbalagan/indian-agri-advice-multilingual)** using a layered regex plus LLM-as-judge filtering pipeline.

`dataset engineering` `multilingual NLP` `data validation`

---

## ✍️ Writing: [The Meta Gradient](https://substack.com/@vinodanbalagan)

Building and breaking AI systems to understand them, with the philosophical bits left in.

- **[Finding the Manifold: Where Neural Networks Land](https://vinodanbalagan.substack.com/p/finding-the-manifold-where-neural)** · the geometry of loss landscape, with a live demo
- **[The Architecture of Dreams: How Neural Networks Learned to Imagine](https://vinodanbalagan.substack.com/p/the-architecture-of-dreams-how-neural)** 
- **[Freezing the Noise](https://vinodanbalagan.substack.com/p/freezing-the-noise)** · How one line of algebra made sampling differentiable

---

## 🛠 Skills

| Area | Tools |
| --- | --- |
| **Languages** | Python · SQL · Bash  |
| **Research** | JAX · PyTorch · probing · causal intervention · experiment design  |
| **ML / DL** | Transformers · LoRA/PEFT · state space models · scikit-learn · XGBoost · probability calibration |
| **NLP & retrieval** | Hugging Face · embeddings · RAG · ChromaDB · multilingual NLP · LLM-as-judge evaluation |
| **Data** | Pandas · NumPy · dataset curation · schema design · data validation · benchmark construction |
| **Systems** | Docker · FastAPI · Weights & Biases · MLflow · AWS · Git · Linux |
| **Visualization** | Matplotlib · Seaborn · Plotly · Marimo · Tableau |

---

## 🎓 Background

- **Machine Learning Foundations** · University of Toronto, 2025
- **MASc, Electronic & Computer Science Engineering** · University of Windsor, 2010–2012
  *Thesis: FPGA implementation of face recognition using Eigenfaces*
- **BE, Electronics & Communication Engineering** · Anna University, 2004–2008

Cohere Labs ML Summer School (2026) · Wolfram ML Statistical Foundations · NVIDIA AI Infrastructure & Operations · Stanford Online ML Specialization · Azure AI-900 · OpenEDG Python Institute

Before all of this: ten years in supply chain operations, procurement analysis, and process optimization.

---

*Understanding by implementing. Measuring before concluding.*
