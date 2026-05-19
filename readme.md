
# BERT-G3CN: SMS Spam Detection

## 📄 Project Inspiration & Credit
**The entire idea, architecture, and methodology for this project are based on the following research paper:**
> Shen, L., Wang, Y., Li, Z., & Ma, W. (2025). *"SMS spam detection using BERT and multi-graph convolutional networks."* International Journal of Intelligent Networks. 
> [Read the full paper here](https://www.sciencedirect.com/science/article/pii/S2666603025000089) 

---

## 📌 Overview 
This project is an independent PyTorch implementation and experimental reproduction of the **BERT-G3CN** model.   

Traditional SMS spam filters struggle with the short, heavily abbreviated, and rapidly evolving nature of SMS text. While Transformer models like BERT are excellent at understanding word context, they miss "big picture" global patterns across an entire dataset. 

This model solves that by combining BERT's deep contextual embeddings with three distinct **Graph Convolutional Networks (GCNs)**:
1. **Co-occurrence Graph:** Captures how often words appear near each other globally.
2. **Heterogeneous Graph:** Captures parts-of-speech (POS), named entities (NER), and structural similarities.
3. **Integrated Syntactic Graph:** Maps grammatical dependency trees.

## 📊 Datasets Used
The model was trained and evaluated on two benchmark datasets to test both highly imbalanced and balanced scenarios:
* **UCI SMS Spam Collection:** Highly imbalanced (86.6% Ham / 13.4% Spam)
* **ExAIS SMS Corpus:** Near-balanced (45.0% Ham / 55.0% Spam)

## 🛠️ Tech Stack & Frameworks
* **Language:** Python
* **Deep Learning:** PyTorch
* **NLP & Transformers:** HuggingFace `transformers`, `spaCy`
* **Environment:** Kaggle (for GPU acceleration)


