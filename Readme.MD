# Vinod Anbalagan
**Machine Learning Engineer | Data Analyst | Multilingual NLP, Evaluation, and Efficient ML Systems**

Toronto, ON  
[LinkedIn](https://www.linkedin.com/in/vinod-anbalagan/) · [Hugging Face](https://huggingface.co/vinod-anbalagan) · [Substack](https://substack.com/@vinodanbalagan)

---

## About

I’m a machine learning and data professional with a background in operations, analytics, and process optimization. I’m currently focused on applied AI, multilingual NLP, dataset development, evaluation pipelines, and efficient machine learning systems.

My work spans practical ML engineering, open-source benchmark contributions, data pipeline design, and technical writing. Long term, I’m interested in research on efficient reasoning, sequence modeling, and architectures that do more with less compute.

**Current interests**
- Multilingual NLP and cultural reasoning benchmarks
- Retrieval-augmented generation and evaluation
- Sequence modeling, state space models, and efficient architectures
- Dataset design, schema standardization, and data quality workflows
- Practical ML systems built under real-world constraints

---

## Selected Projects

### Multicultural Riddles Benchmark — Cohere Labs Open Science Community
**Data pipelines, schema design, and benchmarking workflows for a multilingual cultural reasoning benchmark (~37 languages)**

- Built `contributor_feedback.py` to convert validator output into plain-language guidance for non-technical contributors
- Designed and shipped pilot dataset v1 covering 40 communities and 40,000 riddles mapped to a canonical schema
- Contributing to benchmarking workflow design across API and open-weight model settings
- Organizing cleaned data for standardized release on Hugging Face and GitHub

**Tech:** Python, pandas, Hugging Face Datasets, ISO 639-2/3, multilingual data pipelines  
**[Repo](https://github.com/Cohere-Labs-Community/RiddlesBenchmarking)**

---

### Tamil Agricultural Advisory Dataset — Adaption Labs Uncharted Data Challenge
**Tamil-language agricultural instruction dataset built from 679MB of public-sector data**

- Solo-built dataset from Kisan Call Centre, TNAU extension guides, and ICAR contingency plans
- Curated 187 structured rows across 20 categories, 48 crops, and 17 columns with zero null values
- Completed 10 iterative submissions over 6 weeks
- Received Grade A (9.4/10) and honorary recognition from Sara Hooker

**Tech:** Python, pandas, dataset curation, metadata design, Cohere  
**Dataset:** [Hugging Face](https://huggingface.co/datasets/vinod-anbalagan/tamil-agri-advisory-qa)  - **[Repo](https://github.com/VinodAnbalagan/tamil-agri-dataset-.git)**

---

### DocuNative — Cohere Expedition Hackathon
**Fully offline cross-lingual document QA for migrants and newcomers**

- Pipeline lead on a 7-person team
- Built end-to-end RAG pipeline: PDF extraction → BGE-M3 embeddings → ChromaDB retrieval → Tiny Aya 3.35B generation → mDeBERTa hallucination check
- Ran 9,063 automated evaluations across Chinese, Hindi, and Polish
- Key finding: retrieval quality was driven more by cross-lingual embedding mismatch than by LLM capability

**Tech:** Python, PyTorch, BGE-M3, ChromaDB, mDeBERTa, Gradio, llama-server  - **[Repo](https://github.com/docunative-AI/docunative)**

---

### Rethinking RNN *(In Progress)*
**Implementing sequence models from scratch to understand architectural evolution**

- Building RNN, LSTM, Transformer, and Mamba-style models from first principles
- Analyzing gradient flow, computational tradeoffs, and why each architectural step matters

**Tech:** PyTorch, NumPy, comparative benchmarking

---

### Loss Landscape Visualization
**Exploring neural network optimization surfaces and training dynamics**

- Visualizing loss surfaces to compare optimization behavior across model settings
- Studying why some architectures train more reliably than others

**Tech:** PyTorch, matplotlib, 3D visualization

---

## Experience

### Machine Learning Engineer Intern — M2M Tech
- Built and deployed an end-to-end ML pipeline for a client startup using XGBoost
- Worked across data cleaning, feature engineering, training, API deployment, and monitoring
- Stack: Python, FastAPI, Docker, AWS

### Analytics and Operations Experience
- Applied data analysis to inventory systems, forecasting, and process optimization
- Contributed to measurable operational impact, including waste reduction and reporting automation
- Background in translating operational data into business decisions

---

## Technical Skills

**Languages:** Python, SQL, Bash  
**Data:** pandas, NumPy, data cleaning, EDA, dataset curation, schema design  
**Machine Learning:** scikit-learn, XGBoost, PyTorch, model evaluation, feature engineering  
**NLP / LLM:** Transformers, RAG, embeddings, multilingual NLP, Hugging Face, ChromaDB  
**Deployment:** FastAPI, Docker, AWS, Git/GitHub, Linux  
**Visualization:** matplotlib, Seaborn

---

## Education

**M.A.Sc. Electrical Engineering** — University of Windsor  
**B.E. Electronics & Communication** — Anna University

**Recent Training**
- MIT MicroMasters in Statistics and Data Science *(in progress)*
- Machine Learning Specialization — Stanford
- Machine Learning & Data Science Certificate — University of Toronto
- Google Advanced Data Analytics

---

## Writing

I write about machine learning, architectures, and learning from first principles on **[The Meta Gradient](https://substack.com/@vinodanbalagan)**.

---

## Notes

I’m currently seeking opportunities in:
- Data Analysis
- Data Science / ML Internships
- Junior Machine Learning Engineering
- Research-oriented applied AI work

Long term, I’m building toward research in efficient reasoning and sequence modeling.
