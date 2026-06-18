# Leveraging AI for Indigenous Language Preservation and Revitalization

**Institution:** Thompson Rivers University  
**Program:** Undergraduate Research Experience Award Program (UREAP)  
**Status:** In Progress - Expected completion August 30, 2026

---

## Project Overview

This project explores how artificial intelligence can assist in the digital preservation and revitalization of Indigenous languages in Canada. It does not aim to replace Elders, teachers, or community-led instruction. Instead, it investigates how AI systems can generate beginner-level educational materials using ethically sourced and publicly available linguistic data.

---

## Target Languages

| Language | Region | Approx. Speakers |
|---|---|---|
| Plains Cree (nêhiyawêwin) | Prairie provinces | 87,875 |
| Ojibwe (Anishinaabemowin) | Ontario, Manitoba | 26,165 |
| Inuktitut | Nunavut | 41,675 |

---

## AI System Architecture

Two open-source models are being fine-tuned for low-resource settings:

**1. Speech Recognition (ASR)**
- Base model: Whisper-small (244M parameters)
- Fine-tuned on NRC and CommonVoice audio data
- Task: Convert Indigenous language audio to text
- Metric: Word Error Rate (WER)

**2. Text Generation (LLM)**
- Base model: LLaMA 3.2-3B-Instruct
- Fine-tuned using LoRA (Low-Rank Adaptation) with 4-bit quantization
- Task: Generate beginner educational materials (vocabulary lists, stories, pronunciation guides, quizzes, dialogues)
- Metric: Human evaluation rubric + BLEU score

---

## Data Sources

All datasets are publicly available or community-authorized. No private or culturally sensitive materials are used without explicit community permission.

| Source | Language | License |
|---|---|---|
| Bloomfield Plains Cree Texts (1934) | Plains Cree | Public Domain |
| Bloomfield Sacred Stories (1930) | Plains Cree | Public Domain |
| Faries Dictionary (1938) | Cree | Public Domain |
| Watkins Dictionary (1865) | Cree | Public Domain |
| Howse Grammar (1844) | Cree | Public Domain |
| Baraga Dictionary Part I (1878) | Ojibwe | Public Domain |
| Baraga Dictionary (1853) | Ojibwe | Public Domain |
| Baraga Grammar (1878) | Ojibwe | Public Domain |
| Jones & Michelson Ojibwa Texts (1917) | Ojibwe | Public Domain |
| EdinburghNLP Nunavut Hansard++ | Inuktitut | CC BY 4.0 |

---

## Repository Structure

```
indigenous-language-ai/
├── data/
│   ├── sources.md               # Dataset inventory and license audit
│   └── indigenous_language_training_data.jsonl  # Final training dataset
├── notebooks/                   # Google Colab pipeline notebooks
├── docs/                        # Development plan, ethics statement
├── src/                         # Model training and evaluation scripts
└── README.md
```

---

## Ethical Framework

This project follows Indigenous data sovereignty principles including FPIC (Free, Prior and Informed Consent) and OCAP (Ownership, Control, Access, Possession). All publicly available datasets comply with their respective platform terms. No sacred, restricted, or culturally sensitive materials are used without explicit community permission.

---

## Current Progress

- [x] Dataset collection and inventory
- [x] Text extraction pipeline (PyMuPDF + Tesseract OCR)
- [x] Language-specific text cleaning and normalization
- [x] Training data formatted as JSONL (9,235 examples)
- [ ] Ethics and FPIC compliance statement
- [ ] Baseline model testing (Whisper-small, LLaMA 3.2-3B)
- [ ] ASR fine-tuning
- [ ] LLM fine-tuning
- [ ] Evaluation and community validation
- [ ] Final report

---

## Environment

- Google Colab (free tier, T4 GPU)
- Python 3.12
- Key libraries: `transformers`, `datasets`, `torch`, `whisper`, `bitsandbytes`, `peft`, `pymupdf`, `pytesseract`
