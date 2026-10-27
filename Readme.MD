# Hi, I'm Vinod 👋

**ML engineer and independent researcher. I study what models actually learn, and what they need to remember. Right now: world models that plan for robots, and the leanest memory that keeps them reliable.**

🔬 **Open to ML engineer, research engineer, and applied scientist roles, and to research assistant, internship, or funded MS/PhD positions, especially on teams working on world models, robot learning, or model-based RL.** If you think my work might fit, I'd be glad to hear from you.

📍 Toronto, Canada · [Website](https://vinodanbalagan.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/vinod-anbalagan/) · [Hugging Face](https://huggingface.co/vinod-anbalagan) · [The Meta Gradient](https://substack.com/@vinodanbalagan)

I spent ten years forecasting demand in warehouses and grocery stores, which is a crude way of modelling a world that keeps surprising you. I learned machine learning trying to understand why those models failed, and I am still on that question with better tools.

---

## 🔭 Now

**[Keepsake](https://github.com/VinodAnbalagan/keepsake): can a robot remember only what surprises it?** · *in progress, preprint planned for December 2026*
Most robot foundation models act on the current camera frame alone, which breaks on long tasks where the frame does not show how far along you are. Keepsake tests whether a fast latent world-model planner can fill a small, fixed memory using its own surprise, writing only when its prediction fails, and measures task success and planning time per decision together, against no memory, frame stacking, a recurrent state, full history and an oracle. Simulation first, then a low-cost robot arm. Progress, step by step, in the [Lab](https://vinodanbalagan.vercel.app/lab).

**Learning RL and robot learning from the ground up** · *ongoing*
Berkeley's CS 185/285 (Deep RL), the University of Alberta RL specialization, and *Deep Reinforcement Learning Hands-On* (Lapan, 3rd ed.), alongside Princeton's ROB 345/549 (Introduction to Robotics), ETH Zürich's Robot Learning (2026), and Russ Tedrake's Robotic Manipulation and Underactuated Robotics. In practice: imitation learning (BC, ACT, Diffusion Policy) and vision-language-action models in simulation with MuJoCo and LeRobot, one small measured experiment at a time.


---

## 📌 Selected work

### 🌍 [Cultural Riddles Benchmark](https://github.com/Cohere-Labs-Community/CulturalRiddles)
Cohere Labs Open Science Community · **Co-first author & cross-team lead** · Apr 2026 to present  
- Presenting: 6th Workshop on Multilingual Representation Learning (MRL) · under review at TACL · [arxiv](https://arxiv.org/abs/2610.29968)
- [Dashboard](https://huggingface.co/spaces/CohereLabsCommunity/CulturalRiddles)

Data and release infrastructure for CulturalRiddles: a community-built multilingual benchmark of 6,191 cultural riddles, with a CI-validated contribution pipeline, open Hugging Face release, and interactive results dashboard.

### 📊 Gridline & Prism: what does a win rate in AutoScientist actually measure?
Adaption Labs AutoScientist Challenge · **2nd place, $1,000** · Data & Visualization track · 2026

LoRA fine-tunes of vision-language models (Gemma-3-27B, Qwen3.5-9B) for short-answer chart QA, trained on two correct-by-construction datasets (one visual style for Gridline, ten for Prism) where every answer is computed from seeded values *before* the chart is drawn, plus a hand-authored hardset from real StatCan, BLS, ECB, and WHO charts.

- **The metric rewards easy exams.** With the base model fixed, pairwise win rate fell from 62% to 24% as perceptual difficulty and visual variety rose. Part of what the number measures is how easy you made your own test set.
- **The data platform was corrupting answers.** Maximal enhancement settings made models *worse* than their base (31 to 35% win rate). Diffing the platform's rewrites against the source found 31.6% of answers changed even under explicit guard instructions, including 41 altered numbers.
- **Perceptual, not arithmetic, difficulty.** Eight mechanics, such as truncated and log axes, unlabeled gridline values, near-ties, near-identical colours, and dual axes, target what VLMs actually struggle with: reading the value in the first place.

Datasets: [v1, one style](https://huggingface.co/datasets/vinod-anbalagan/gridline-chartqa) · [v2, ten styles](https://huggingface.co/datasets/vinod-anbalagan/adaption-charts-p2-gold) · Models: [Gridline](https://huggingface.co/vinod-anbalagan/gridline) · [Prism](https://huggingface.co/vinod-anbalagan/prism) · also a [Llama-3.2-3B LoRA](https://huggingface.co/vinod-anbalagan/Llama-3.2-3B-marketing-spend-revenue-qa) for table-grounded QA

`LoRA/PEFT` `vision-language models` `synthetic data` `evaluation design`

### 🧾 [chart-reasoning-verified](https://huggingface.co/datasets/vinod-anbalagan/chart-reasoning-verified)
7,500 chart-reasoning rows generated from an explicit latent dataset, so the image is a rendering of known ground truth rather than the source of it. Family-disjoint splits, an independent verifier on every answer, and abstention rows produced by reading axis limits back off the rendered figure: when a value falls outside the drawn area, the correct answer is to decline and say why.

### 📄 [DocuNative](https://github.com/docunative-AI/docunative)
Cohere Expedition Hackathon · **Pipeline lead**, 7-person team

Fully offline cross-lingual document QA for newcomers and migrants: ask about a foreign-language document in your own language and get answers with source quotes and a hallucination trust score. Nothing leaves the user's machine.

- End-to-end RAG: PDF extraction → BGE-M3 embeddings → ChromaDB retrieval → Tiny Aya via llama.cpp → mDeBERTa hallucination verification
- 9,000+ automated evaluations across Chinese, Hindi, and Polish
- Finding: cross-lingual **embedding** quality, not LLM capability, was the primary retrieval bottleneck

`Python` `RAG` `ChromaDB` `BGE-M3` `llama.cpp` `Gradio`

### 🌾 [Tamil Agricultural Advisory Dataset](https://huggingface.co/datasets/vinod-anbalagan/tamil-agri-advisory-qa)
Adaption Labs Uncharted Data Challenge · **Grade A (9.4/10)** · [repo](https://github.com/VinodAnbalagan/tamil-agri-dataset-)

187 curated Tamil Q&A records across 48 crops and 20 categories, built from public-sector sources (Kisan Call Centre, TNAU, ICAR) over 10 iterative submissions. Honorary recognition from Sara Hooker. Follow-up: an [11-language Indian agricultural dataset](https://huggingface.co/datasets/vinod-anbalagan/indian-agri-advice-multilingual) (718 records, 14 agro-climatic zones) filtered with a layered regex plus local LLM-as-judge pipeline.

`dataset engineering` `multilingual NLP` `data validation`

---

## ✍️ Writing: [The Meta Gradient](https://substack.com/@vinodanbalagan)

Building and breaking AI systems to understand them, with the philosophical bits left in.

- **[The Architecture of Dreams: How Neural Networks Learned to Imagine](https://vinodanbalagan.substack.com/p/the-architecture-of-dreams-how-neural)**
- **[Freezing the Noise](https://vinodanbalagan.substack.com/p/freezing-the-noise)** · how one line of algebra made sampling differentiable
- **[Finding the Manifold: Where Neural Networks Land](https://vinodanbalagan.substack.com/p/finding-the-manifold-where-neural)** · the geometry of the loss landscape, with a live demo

---

## 🛠 Skills

| Area | Tools |
| --- | --- |
| **Languages** | Python · SQL · Bash |
| **Research** | JAX · PyTorch · probing · activation patching · experiment design |
| **Robot learning** *(learning)* | MuJoCo · LeRobot · imitation learning · VLAs · latent world models and planning |
| **ML / DL** | Transformers · LoRA/PEFT · vision-language fine-tuning · state space models · scikit-learn · XGBoost · probability calibration |
| **Evaluation & data** | benchmark construction · LLM/VLM evaluation · LLM-as-judge · dataset curation · schema design · data validation |
| **NLP & retrieval** | Hugging Face · embeddings · RAG · ChromaDB · multilingual NLP |
| **Systems** | Docker · FastAPI · GitHub Actions · llama.cpp · Weights & Biases · MLflow · AWS · Git · Linux |
| **Visualization** | Matplotlib · Seaborn · Plotly · Marimo · Tableau |

---

## 🎓 Background

- **Machine Learning Foundations** · University of Toronto, 2025
- **MASc, Electronic & Computer Science Engineering** · University of Windsor, 2010–2012
    - *Thesis: FPGA implementation of face recognition using Eigenfaces*
- **BE, Electronics & Communication Engineering** · Anna University, 2004–2008


Cohere Labs ML Summer School (2026) · Wolfram ML Statistical Foundations · NVIDIA AI Infrastructure & Operations · Stanford Online ML Specialization · Azure AI-900 · OpenEDG Python Institute

Before all of this: ten years in supply chain operations, procurement analysis, and process optimization.

---

*Understanding by implementing. Measuring before concluding.*
