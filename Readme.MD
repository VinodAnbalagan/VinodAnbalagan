# Hi, I'm Vinod 👋

**I study what models actually learn. When a model succeeds, has it learned the structure of the problem, or cues that happen to correlate with it? I build datasets, evaluations, and probes to find out, and I'm now taking that question into world models and model-based RL.**

🔬 **I'm looking to join a research group or team working on world models, representation learning, or evaluation, as a research engineer, research assistant, intern, or funded MS/PhD student.** If you think my work might fit, I'd be glad to hear from you.

📍 Toronto, Canada · [Website](https://vinodanbalagan.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/vinod-anbalagan/) · [Hugging Face](https://huggingface.co/vinod-anbalagan) · [The Meta Gradient](https://substack.com/@vinodanbalagan)

I spent ten years forecasting demand in warehouses and grocery stores, which is a crude way of modelling a world that keeps surprising you. I learned machine learning trying to understand why those models failed, and I am still on that question with better tools.

---

## 🔭 Now

**[Reverie](https://vinodanbalagan.vercel.app/research): does a world model represent what it cannot see?** · *pre-registered, in progress*
Testing whether recurrent state-space world models trained on video keep a decodable, causally used representation of objects behind occluders, or just extrapolate in straight lines. Linear and MLP probes, activation patching, and hidden collisions as the control. Built in JAX.

**Learning model-based RL from the ground up** · *ongoing*
Working through *Deep Reinforcement Learning Hands-On* (Lapan, 3rd ed.) and implementing the pieces myself, one small measured experiment at a time, in the [Lab](https://vinodanbalagan.vercel.app/lab).

**Multicultural Riddles Benchmark** · Cohere Labs Open Science Community · *first author* · presenting at **MRL 2026**, under review at **TACL**, arXiv preprint coming soon

---

## 📌 Selected work

### 🌍 Multicultural Riddles Benchmark
Cohere Labs Open Science Community · **First author & cross-team lead** · Apr 2026 to present · MRL 2026 · under review at TACL · *(repo private until publication)*

A cultural-reasoning benchmark of **~6,100 natively written, human-evaluated riddles across 51 languages and 61 communities**, built with ~100 contributors. Riddles are a setting where surface fluency and genuine understanding come apart sharply: a model can produce perfect Tamil and still miss what a Tamil riddle is actually about.

- Owned data integrity across 30 evaluated models: caught scoring-definition and coverage issues that were inflating results, added automated reconciliation checks, and ran an annotation audit that led to re-validating a community whose scores were unreliable.
- Built the self-serve contribution pipeline: fork-based submissions auto-validated on each pull request via GitHub Actions, plus a one-command publisher that ships versioned releases to Hugging Face with contributor credits and ISO language codes.
- Built a public results dashboard on Hugging Face Spaces with per-model, per-culture, difficulty, and error-type views, every figure reconciled to the human-evaluation source data.

`Python` `Pandas` `Hugging Face Datasets` `GitHub Actions` `LLM evaluation`

### 📊 Gridline & Prism: what does a win rate actually measure?
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
| **ML / DL** | Transformers · LoRA/PEFT · vision-language fine-tuning · state space models · scikit-learn · XGBoost · probability calibration |
| **Evaluation & data** | benchmark construction · LLM/VLM evaluation · LLM-as-judge · dataset curation · schema design · data validation |
| **NLP & retrieval** | Hugging Face · embeddings · RAG · ChromaDB · multilingual NLP |
| **Systems** | Docker · FastAPI · GitHub Actions · llama.cpp · Weights & Biases · MLflow · AWS · Git · Linux |
| **Visualization** | Matplotlib · Seaborn · Plotly · Marimo · Tableau |

---

## 🎓 Background

- **MASc, Electronic & Computer Science Engineering** · University of Windsor, 2010–2012
  *Thesis: FPGA implementation of face recognition using Eigenfaces*
- **BE, Electronics & Communication Engineering** · Anna University, 2004–2008
- **Machine Learning Foundations** · University of Toronto, 2025

Cohere Labs ML Summer School (2026) · Wolfram ML Statistical Foundations · NVIDIA AI Infrastructure & Operations · Stanford Online ML Specialization · Azure AI-900 · OpenEDG Python Institute

Before all of this: ten years in supply chain operations, procurement analysis, and process optimization.

---

*Understanding by implementing. Measuring before concluding.*
