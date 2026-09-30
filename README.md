# EmphaBot: Enhancing Accessibility in Mental Health Support using a CoT-RAG-based Language Model

Official implementation repository for **“EmphaBot version 1”**
   
<p align="center">
  <img src="https://img.shields.io/badge/LLM-CoT--RAG-blue" />
  <img src="https://img.shields.io/badge/Domain-Mental%20Health-green" />
  <img src="https://img.shields.io/badge/Framework-PyTorch-orange" />
  <img src="https://img.shields.io/badge/License-MIT-brightgreen" />
</p>

---   

## 🧠 Overview

**EmphaBot** is a conversational AI framework designed to enhance accessibility in mental health support using a **Chain-of-Thought Retrieval-Augmented Generation (CoT-RAG)** architecture. The framework integrates:

- **Large Language Models (LLMs)**
- **Chain-of-Thought (CoT) reasoning**
- **Retrieval-Augmented Generation (RAG)**
- **Therapeutic dialogue grounding**
- **Accessibility-oriented conversational support**

The system aims to generate empathetic, contextually grounded, and semantically consistent therapeutic responses while reducing unsupported or hallucinated outputs.

---

## ✨ Key Features

- 🔹 Fine-tuned **LLaMA 3 8B** and **Gemma 2B** conversational models
- 🔹 CoT-enhanced therapeutic reasoning
- 🔹 Elasticsearch-based BM25 retrieval pipeline
- 🔹 Retrieval grounding using annotated therapeutic transcripts
- 🔹 Multi-metric evaluation framework
- 🔹 Accessibility-aware conversational response generation
- 🔹 Comparative evaluation of:
  - Basic
  - Basic-RAG
  - CoT
  - CoT-RAG architectures

---

## 🏗️ System Architecture

The EmphaBot pipeline consists of the following stages:

| Stage | Description |
|---|---|
| Dataset Preparation | Cleaning and structuring empathetic and therapeutic dialogue datasets |
| Fine-Tuning | Domain adaptation of LLaMA and Gemma models |
| RAG Indexing | Elasticsearch BM25 indexing of therapeutic conversations |
| Retrieval | Retrieval of contextually relevant therapeutic dialogue |
| CoT Integration | Step-by-step reasoning during response generation |
| Inference | Generation of grounded therapeutic responses |
| Evaluation | Automatic and semantic evaluation of generated responses |

---

## 📚 Datasets

The framework utilizes multiple conversational and therapeutic datasets, including:

- Empathetic Dialogues Dataset
- Mental Health Conversational Dataset
- Annotated Therapeutic Dialogue Transcripts
- Custom Context–Response Therapeutic Corpora

---

## 🤖 Base Models

```python

### LLaMA Models
MODEL_CANDIDATES = [
    "unsloth/llama-3-8b-bnb-4bit",
    "unsloth/llama-3-8b-Instruct-bnb-4bit",
]

### Gemma Models
MODEL_CANDIDATES = [
    "unsloth/gemma-2b-bnb-4bit",
    "unsloth/gemma-2-2b-it-bnb-4bit",
]
```

---

## 🔎 Retrieval-Augmented Generation (RAG)

EmphaBot employs a sparse retrieval pipeline using Elasticsearch BM25 retrieval.

### Retrieval Configuration
   
| Parameter | Setting |
|---|---|
| Retrieval Engine | Elasticsearch |
| Retrieval Method | BM25 Sparse Retrieval |
| Retrieval Top-k | 3 |
| Query Type | `match` query |
| Indexing Strategy | Context–Response document indexing |

---

## 📊 Evaluation Framework

The EmphaBot framework employs a multi-metric evaluation approach combining quantitative and qualitative assessment of generated therapeutic responses.

<p align="center">
  <img src="./Multi-metric%20Evaluation%20Framework.png"
       alt="Multi-Metric Evaluation Framework"
       width="900">
</p>

**Figure 9.** Multi-metric evaluation framework for assessing EmphaBot across LLaMA 3 and Gemma 2B variants, including quantitative and qualitative evaluation dimensions.

---

## 📊 Evaluation Metrics

The framework was evaluated using both traditional NLP metrics and semantic grounding metrics.

### Automatic Metrics

- BLEU
- ROUGE-1
- ROUGE-2
- ROUGE-L
- ROUGE-S
- ROUGE-SU
- ROUGE-W
- Perplexity (PPL)

### Semantic & Therapeutic Metrics

- BERTScore
- BLEURT
- Semantic Similarity
- Faithfulness (NLI)
- Empathy Intent (NLI)
- Coherence Cosine
- Concordance Correlation Coefficient (CCC)
- MAE

### Efficiency Metrics

- Latency
- Token Processing Efficiency

---

## 🛡️ Ethical Considerations

EmphaBot is intended as a supportive conversational research system and **not** as a replacement for licensed mental health professionals.

The framework incorporates:

- Retrieval grounding
- Semantic consistency evaluation
- Faithfulness assessment
- Context-aware therapeutic response generation


## 🚧 Repository Status

🚧 **Codebase preparation in progress**

The complete implementation, training scripts, evaluation pipelines, and retrieval framework will be released publicly after final repository cleanup and documentation.

---

## 📄 Citation

If you use this work, please cite:

```bibtex
@article{nwokoye2026emphabot,
  title={EmphaBot: Enhancing Accessibility in Mental Health Support using a CoT-RAG-based Language Model},
  author={Nwokoye, Chukwunonso Henry and Iloka, Blessing Oluchi},
  journal={},
  year={2026}
}
```

---

## 📬 Contact

For questions, collaborations, or research discussions:

**Chukwunonso Henry Nwokoye**  
📧 Email: chinonsonwokoye@gmail.com

---


## 🚧 Repository Status

🚧 **Codebase preparation in progress**

The complete implementation, training scripts, evaluation pipelines, and retrieval framework will be released publicly after final repository cleanup and documentation.


