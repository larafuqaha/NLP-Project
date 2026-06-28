# TruthfulQA — Paper Presentation & Core Mechanism Reproduction
### ENCS5342 — Information Retrieval with Applications of NLP | Track 2

**Team:** Taymaa Nasser (1222640) · Tawba Abdallah (1221002) · Lara Fuqaha (1220071)  
**Paper:** Lin, Hilton & Evans (2021) — *TruthfulQA: Measuring How Models Mimic Human Falsehoods*  
**arXiv:** https://arxiv.org/abs/2109.07958

---

## What This Project Does

This repository contains our Track 2 paper presentation for ENCS5342. We explain
the TruthfulQA benchmark and reproduce its central mechanism from scratch: we
fine-tune GPT-2 on a small dataset of common misconceptions and show that the
model's likelihood preferences shift from true answers toward false ones...
demonstrating imitative falsehoods in a controlled setting.

## How to Run

1. Open `TruthfulQA_Track2_final.ipynb` in [Google Colab](https://colab.research.google.com)
2. Set runtime to **T4 GPU** (Runtime → Change runtime type)
3. Uncomment the `pip install` line in the Environment Setup cell
4. Run all cells top to bottom

**Dependencies:** `transformers`, `torch`, `pandas`, `matplotlib`, `numpy`

## Key Results

- Fine-tuning GPT-2 on 36 misconceptions drops its truth-preference rate
  significantly on trained questions
- The effect partially survives paraphrasing — the model learned a belief-level
  association, not just surface memorization
- The effect does not generalize to unseen misconceptions — fine-tuning installed
  specific falsehoods, not a general disposition toward untruthfulness

## Extra Credit

- 🎥 **Interview video** — real people asked the same questions, answers compared
  live during the presentation
- 🌐 **Interactive website** — browse all 817 TruthfulQA questions by category
