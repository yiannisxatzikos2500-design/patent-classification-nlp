# Patent Classification using Fine-Tuned Language Models

This repository contains the final portfolio for the Deep Learning course. The project focuses on improving the classification of patent data by transitioning from a frozen-embedding baseline to a fully optimized system using advanced fine-tuning strategies.

## 👥 Authors
* Timo Philipse
* Ioannis Chatzikos
* Kristjana Prifti
* Álvaro Buendía
* Víctor Carmona

**Date:** 04/03/2026

## 📖 Project Overview
The core objective was to evaluate whether progressively advanced fine-tuning strategies and an agentic workflow architecture could produce a superior **PatentSBERTa-based** classification model. 

The project tracks the evolution of model performance through four major assignments, moving from basic embeddings to sophisticated techniques like **QLORA**, **Multi-Agent Systems (MAS)**, and **Human-in-the-Loop (HITL)** refinement.

## 📊 Performance Evolution
We measured success using the **F1 Score** on a consistent evaluation set. The results demonstrate that task-specific fine-tuning is the primary driver of performance.

| Model Version | Training Strategy | F1 Score |
| :--- | :--- | :--- |
| **Baseline** | Frozen Embeddings (No Fine-tuning) | 0.7813 |
| **Assignment 2** | Fine-tuned on Silver + Gold (Simple LLM) | 0.8078 |
| **Assignment 3** | Advanced Fine-tuning Techniques | 0.8089 |
| **Final Model** | QLORA-Powered MAS + Targeted HITL | **0.8099** |

## 🛠️ Key Technologies
* **Base Model:** PatentSBERTa
* **Libraries:** `transformers`, `scikit-learn`, `pandas`, `numpy`, `matplotlib`
* **Techniques:** QLORA, Multi-Agent Debate (Skeptic vs. Advocate), HITL Refinement.

## 📂 Repository Structure
* `deep_learning_group_final.ipynb`: The complete codebase covering Assignments 1 through 4, including data preprocessing, model training, and evaluation.
* `DL Report .pdf`: A detailed technical report analyzing the results, challenges, and conclusions of the project.

## 💡 Key Insights
1.  **Fine-Tuning is King:** The largest performance jump (+0.026) occurred during initial task-specific fine-tuning.
2.  **Diminishing Returns:** While MAS and HITL improved the score, the gains were incremental compared to the initial fine-tuning.
3.  **Data Quality over Complexity:** The project confirmed that high-quality data and effective fine-tuning remain more impactful than increasing architectural complexity.

## 🔗 Resources & Datasets
* **Final Fine-Tuned Model:** [TimoPh/final-patent-as4-model](https://huggingface.co/TimoPh/final-patent-as4-model)
* **50k Green Patent Dataset:** [TimoPh/patent-claims-50k-green](https://huggingface.co/datasets/TimoPh/patent-claims-50k-green)
* **Multi-Agent Debate Dataset:** [TimoPh/as4-multi-agent-debate-gold](https://huggingface.co/datasets/TimoPh/as4-multi-agent-debate-gold)

---
*This project was developed as a final submission for the Deep Learning Portfolio.*
