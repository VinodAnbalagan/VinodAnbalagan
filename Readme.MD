<h1 align="center">Vinod Anbalagan</h1>

<p align="center">ML engineer and independent researcher · Toronto</p>

<p align="center">
  <a href="https://vinodanbalagan.vercel.app/"><img src="https://img.shields.io/badge/Website-1f2328?style=flat-square" alt="Website"></a>
  <a href="https://www.linkedin.com/in/vinod-anbalagan/"><img src="https://img.shields.io/badge/LinkedIn-1f2328?style=flat-square" alt="LinkedIn"></a>
  <a href="https://huggingface.co/vinod-anbalagan"><img src="https://img.shields.io/badge/Hugging%20Face-1f2328?style=flat-square" alt="Hugging Face"></a>
  <a href="https://substack.com/@vinodanbalagan"><img src="https://img.shields.io/badge/The%20Meta%20Gradient-1f2328?style=flat-square" alt="The Meta Gradient"></a>
</p>

<p align="center"><i>I study what models actually learn, and what they need to remember.</i></p>

---

I build and evaluate ML systems: multilingual benchmarks, RAG pipelines, fine-tuned vision-language models, and audits of what training really changed. The question underneath all of it is whether a result means what it appears to. Right now I'm working on world models that plan for robots, and the leanest memory that keeps them reliable.

Before ML, I spent ten years forecasting demand in warehouses and grocery stores, a crude way of modelling a world that keeps surprising you. I learned machine learning trying to understand why those models failed.

**Open to** ML engineer, AI engineer, research engineer, and applied scientist roles, and to research internships and funded MS/PhD positions, especially in world models, robot learning, and model-based RL.

## Now

**[Notch](https://github.com/VinodAnbalagan/notch)** · what should a robot remember? · *in progress*

A robot that acts only on its current camera frame fails as soon as the frame stops showing what it needs. Notch compares five rules for what a world-model planner writes into a small, fixed memory: time, chance, the model's own surprise, whether an observation changed the plan, and the two combined. Plan change is a signal only a planner can measure about itself. Task success and planning time are measured together, against baselines from no memory to full history. Simulation first, then a robot arm. Progress is logged in the [Lab](https://vinodanbalagan.vercel.app/lab).

## Recent

- **Nov 2026** · [Where Does Forgotten Knowledge Go?](https://huggingface.co/spaces/vinod-anbalagan/where-forgotten-knowledge-goes), an unlearning audit for the Lexsi Labs AI Safety Hackathon
- **Oct 2026** · [A Multicultural Benchmark of Riddles](https://arxiv.org/abs/2610.29968) on arXiv, to be presented at MRL 2026
- **Sep 2026** · [Freezing the Noise](https://vinodanbalagan.substack.com/p/freezing-the-noise), how one line of algebra made sampling differentiable

## Selected work

**[CulturalRiddles](https://github.com/Cohere-Labs-Community/CulturalRiddles)** · multilingual LLM benchmark<br>
<sub>Cohere Labs Open Science Community · co-first author & cross-team lead · MRL 2026 · under review at TACL</sub><br>
6,191 native-written cultural riddles across 51 languages. I built the data and release infrastructure: a CI-validated contribution pipeline, the open Hugging Face release, and the interactive results dashboard.<br>
[Paper](https://arxiv.org/abs/2610.29968) · [Dashboard](https://huggingface.co/spaces/CohereLabsCommunity/CulturalRiddles) · [Code](https://github.com/Cohere-Labs-Community/CulturalRiddles)

**[Where Does Forgotten Knowledge Go?](https://huggingface.co/spaces/vinod-anbalagan/where-forgotten-knowledge-goes)** · auditing machine unlearning in English and Tamil<br>
<sub>Lexsi Labs AI Safety Hackathon · Nov 2026</sub><br>
Taught Tiny Aya 96 facts about invented people, unlearned 24 with SafeTune on layers chosen by CircuitKIT, then checked whether they were really gone. All 34 facts forgotten in English were still answered in Tamil, and unlearned models avoid answers in a detectable way. 2,022 blind human labels (κ 0.96), every run pre-registered.<br>
[Article](https://substack.com/@vinodanbalagan/note/p-224966557) · [Code](https://github.com/VinodAnbalagan/unlearn-audit-tiny-aya) · [Models](https://huggingface.co/collections/vinod-anbalagan/where-does-forgotten-knowledge-go-models-6af482145d0cf8e6a2efd8f9) · [Data and logs](https://huggingface.co/collections/vinod-anbalagan/where-does-forgotten-knowledge-go-data-and-logs-6af48214756c4d246ff2ef18)

**Gridline & Prism** · what does a win rate actually measure?<br>
<sub>Adaption Labs AutoScientist Challenge · 2nd place</sub><br>
LoRA fine-tunes of Gemma-3-27B and Qwen3.5-9B for chart QA, trained on correct-by-construction data. With the base model fixed, win rate fell from 62% to 24% as test difficulty rose, so part of the metric measures how easy you made your own test set. Diffing the platform's data rewrites also showed 31.6% of answers had been changed.<br>
[Gridline](https://huggingface.co/vinod-anbalagan/gridline) · [Prism](https://huggingface.co/vinod-anbalagan/prism) · [Dataset v1](https://huggingface.co/datasets/vinod-anbalagan/gridline-chartqa) · [Dataset v2](https://huggingface.co/datasets/vinod-anbalagan/adaption-charts-p2-gold)

**[DocuNative](https://github.com/docunative-AI/docunative)** · offline cross-lingual document QA<br>
<sub>Cohere Expedition Hackathon · pipeline lead, 7-person team</sub><br>
Ask about a foreign-language document in your own language and get answers with source quotes and a hallucination trust score, with nothing leaving the device. BGE-M3, ChromaDB, Tiny Aya via llama.cpp, and mDeBERTa verification. 9,000+ evaluations showed embedding quality, not the LLM, was the bottleneck.

**Datasets and models**

- [chart-reasoning-verified](https://huggingface.co/datasets/vinod-anbalagan/chart-reasoning-verified) · 7,500 chart-reasoning rows rendered from known ground truth, with an independent verifier and abstention cases
- [Tamil Agricultural Advisory QA](https://huggingface.co/datasets/vinod-anbalagan/tamil-agri-advisory-qa) · 187 curated records, Grade A (9.4/10), honorary recognition from Sara Hooker
- [Indian Agricultural Advice, 11 languages](https://huggingface.co/datasets/vinod-anbalagan/indian-agri-advice-multilingual) · 718 records filtered with regex plus LLM-as-judge
- [Llama-3.2-3B table QA](https://huggingface.co/vinod-anbalagan/Llama-3.2-3B-marketing-spend-revenue-qa) · LoRA fine-tune for table-grounded question answering

## Writing

[The Meta Gradient](https://substack.com/@vinodanbalagan) · building and breaking AI systems to understand them, with the philosophical bits left in.

- [The Architecture of Dreams](https://vinodanbalagan.substack.com/p/the-architecture-of-dreams-how-neural) · how neural networks learned to imagine
- [Freezing the Noise](https://vinodanbalagan.substack.com/p/freezing-the-noise) · how one line of algebra made sampling differentiable
- [Finding the Manifold](https://vinodanbalagan.substack.com/p/finding-the-manifold-where-neural) · where neural networks land, with a live demo

## Toolkit

| Area | Tools |
| :--- | :--- |
| Languages | Python · SQL · Bash |
| ML and research | PyTorch · JAX · Transformers · LoRA/PEFT · VLM fine-tuning · state space models · probing · activation patching |
| Evaluation and data | benchmark design · LLM/VLM evaluation · LLM-as-judge · dataset curation · data validation |
| LLM applications | RAG · embeddings · ChromaDB · llama.cpp · multilingual NLP |
| Systems | Docker · FastAPI · GitHub Actions · Weights & Biases · MLflow · AWS · Linux |
| Robot learning *(learning)* | MuJoCo · LeRobot · imitation learning · VLAs · latent world models and planning |

## Background

MASc, Electronic & Computer Science Engineering, University of Windsor · BE, Electronics & Communication Engineering, Anna University · Machine Learning Foundations, University of Toronto (2025)

<sub>Cohere Labs ML Summer School 2026 · Wolfram ML Statistical Foundations · NVIDIA AI Infrastructure & Operations · Stanford Online ML Specialization · Azure AI-900 · OpenEDG Python Institute</sub>

---

<p align="center"><sub>Understanding by implementing. Measuring before concluding.</sub></p>
