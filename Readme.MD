# Hi, I'm Vinod 👋

**ML engineer working on representation and evaluation: when a model succeeds, has it learned the structure of the problem, or the surface cues that happen to correlate with it?**

📍 Toronto, Canada · [LinkedIn](https://www.linkedin.com/in/vinod-anbalagan/) · [Hugging Face](https://huggingface.co/vinod-anbalagan) · [The Meta Gradient](https://substack.com/@vinodanbalagan)

I spent ten years forecasting demand in warehouses and grocery stores, which is a crude way of modelling a world that keeps surprising you. I learned machine learning trying to understand why those models failed, and I am still on that question with better tools.

---

## 🔭 What I'm working on

**Multicultural Riddles Benchmark** · Cohere Labs Open Science Community · *first author, paper in preparation*
A cultural-reasoning benchmark spanning **51 languages and ~6,100 riddles**, built with ~100 contributors. Riddles are a setting where surface fluency and genuine understanding come apart sharply: a model can produce perfect Tamil and still miss what a Tamil riddle is actually about.

**Reverie: does a world model represent what it cannot see?** · *active*
Balls bounce and collide in a box, and sometimes one passes behind an occluder. The model is trained on the video with **no physics in the loss**. While the ball is hidden, does the internal state still contain it?

Three analyses on an RSSM, with a JEPA arm for comparison:

- **Probe** whether position, velocity and presence stay decodable from the deterministic state and the stochastic latent, tracked frame by frame through the occlusion window
- **Patch** the latent at occlusion onset, against a random-direction control of equal norm, to test whether that representation is load-bearing rather than merely correlated
- **Dynamics**: while blind, does the state hold a fixed point, drift along a slow manifold, or decay toward the prior

The sharpest control is a ball-ball collision hidden behind the occluder. It is unpredictable from the pre-occlusion state, which is what separates genuine integration from velocity extrapolation. External validation on CLEVRER, where the occlusion mechanism differs but the question does not.

**World model evaluation harness** · Cohere Labs "World Models from Scratch" · *in progress*
One small, fully instrumented 2D physics platform with exact ground truth, and a gated sequence of pre-registered experiments run on it, rather than eight unrelated demos. The through-line is measurement: when does a learned world model look plausible and fail dynamically? First a calibration study asking whether sampling disagreement is actually a usable uncertainty signal, then an architecture comparison, then exposure bias and test-time compute. Open-loop rollout is always reported separately from teacher-forced one-step quality, and visual error, state error and action error are never collapsed into one number.

Both run the same way: hypotheses and falsification conditions written down before training, a run manifest behind every figure, seed-level results rather than mean curves alone, and an append-only log so it stays visible later when a decision's assumptions have expired.

`JAX` `Equinox` `PyTorch` `probing` `activation patching` `pre-registration`

---

## 🎛 Try something

**[Loss Landscape Explorer](https://molab.marimo.io/notebooks/nb_Nc8hhS2UiJqyGRsvpY1nFo/app)** · interactive
A 2D slice through a 50,000-dimensional weight space you can rotate, with a noise-injection slider that tests whether a minimum is genuinely flat or just got lucky. Built on Ziming Liu's local-plane blending method, extended with 3D Plotly rendering and a robustness test.
Write-up: **[Finding the Manifold](https://vinodanbalagan.substack.com/p/finding-the-manifold-where-neural)**

---

## 📌 Selected work

### 🌍 Multicultural Riddles Benchmark
Cohere Labs Open Science Community · **First author** · Apr 2026 to present · *(repo private until publication)*

- Lead data creation, validation, evaluation, and analysis across 51 languages and ~6,100 riddles
- Align ~100 contributors across data, evaluation, and analysis tracks on schema design, validation rules, and release requirements
- Built Python tooling that turns validator output into contributor-actionable guidance, improving annotation consistency and cutting review cycles
- Designed the canonical schema, benchmarking pipeline, and structured dataset releases on GitHub and Hugging Face

`Python` `Pandas` `Hugging Face Datasets` `schema design` `LLM evaluation`

### 📊 Adaption Labs AutoScientist Challenge
**2nd place, $1,000** · Data & Visualization track · 2026

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

- **[Finding the Manifold: Where Neural Networks Land](https://vinodanbalagan.substack.com/p/finding-the-manifold-where-neural)** · the geometry of optimization, with a live demo
- **[NeurIPS 2025: The Year We Admitted We Were Lost](https://vinodanbalagan.substack.com/p/neurips-2025-the-year-we-admitted)** · notes on the cracks in scaling orthodoxy
- **[Animals, Ghosts, and Chimeras](https://vinodanbalagan.substack.com/p/animals-ghosts-and-chimeras-the-ai)** · a four-part series on the embodiment debate
- **[Building the Dataset Tamil Farmers Deserve](https://vinodanbalagan.substack.com/p/building-the-dataset-tamil-farmers)** · where AI fails the Global South

---

## 🛠 Skills

| Area | Tools |
| --- | --- |
| **Languages** | Python · SQL · Bash · Go *(learning)* |
| **Research** | JAX · Equinox · PyTorch · probing · causal intervention · experiment design · pre-registration |
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
