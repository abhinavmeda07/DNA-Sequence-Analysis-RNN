# 🧬 DNA Sequence Analysis using Bidirectional LSTMs

> **Applied Deep Learning Project** | Weight-3 Deliverable  
> **Domain**: Bioinformatics & Genomic Sequence Analysis

---

## 📌 Project Overview
This repository contains a deep learning pipeline designed for **DNA Promoter Sequence Classification**. Utilizing a **Bidirectional Long Short-Term Memory (BiLSTM)** architecture implemented in TensorFlow/Keras, the model learns complex contextual motifs (such as Pribnow `-10` boxes and consensus `-35` regions) to distinguish functional promoter targets from background genomic DNA.

---

## 🏗️ Model Architecture & Pipeline
- **Input Encoding**: Character-level tokenization mapping nucleotides (`A`, `C`, `G`, `T`) into vector space.
- **Embedding Layer**: 64-dimensional dense representation.
- **Recurrent Core**: Stacked Bidirectional LSTMs ($64$ units $\rightarrow$ $32$ units) to extract forward and reverse sequence context.
- **Regularization**: Integrated Dropout ($0.3$) and Batch Normalization layers to prevent overfitting.
- **Classification Output**: Sigmoid dense output layer for binary crossentropy loss optimization.

---

## 📊 Key Results & Performance
- **Test Accuracy**: **~98.45%**
- **Precision & Recall**: High sensitivity and specificity across promoter detection targets.
- **Convergence**: Optimized using Adam ($lr=0.001$) with Early Stopping and Model Checkpointing.

---

## 📁 Repository Deliverables
- `DNA_Sequence_Analysis_DPLConcept.ipynb` — Complete Google Colab notebook containing code, training analytics, visualization, and interactive live demo UI.
- `Project_Report_DNA_RNN.html.pdf` — Comprehensive IEEE-formatted project report detailing methodology, metrics, and architecture.
- `Genomic Sequence Analysis using Bidirectional LSTMs.pptx` — Presentation slide deck structured for the 12-minute presentation.

---

## 🚀 How to Run locally / Colab
1. Open `DNA_Sequence_Analysis_DPLConcept.ipynb` directly in **Google Colab**.
2. Run all cells sequentially.
3. Use the **Interactive Widget Dashboard** in the final cell to test custom DNA sequence strings or preset examples in real-time.
