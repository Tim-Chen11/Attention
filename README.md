# 🔍 Attention Mechanisms

This repository contains notes, code, and experiments on various **Attention Mechanisms** used in deep learning, especially in transformers and large language models.

---

## 📖 Table of Contents

1. [Attention](#1-attention)
2. [Self and Cross Attention](#2-self-and-cross-attention)
3. [Sparse and Linear Attention](#3-sparse-and-linear-attention)
4. [KV Cache](#4-kv-cache)
5. [MHA, MQA, GQA, MHLA](#5-mha-mqa-gqa-mhla)
6. [DCA & S² Attention](#6-dca--s²-attention)

---

## 1. Attention

- Scaled Dot-Product Attention
- Query, Key, Value concepts
- Softmax-based weighting
- Used to focus on relevant parts of the input

---

## 2. Self and Cross Attention

- **Self-Attention**: Attention within the same sequence (e.g. encoder).
- **Cross-Attention**: Attention across different sequences (e.g. decoder attending to encoder output).

---

## 3. Sparse and Linear Attention

- **Sparse Attention**: Limits attention to a subset (local/global) to reduce complexity.
- **Linear Attention**: Replaces softmax with kernel functions for linear time/memory complexity.

---

## 4. KV Cache

- Stores Key and Value tensors during inference.
- Speeds up autoregressive generation by reusing previous states.
- Common in models like GPT-3, LLaMA, and others.

---

## 5. MHA, MQA, GQA, MHLA

- **MHA (Multi-Head Attention)**: Standard attention with multiple parallel heads.
- **MQA (Multi-Query Attention)**: One Key/Value shared across all heads (faster inference).
- **GQA (Grouped Query Attention)**: Keys/Values shared across groups of query heads.
- **MHLA (Multi-Head Local Attention)**: Applies attention to local windows (efficient for long sequences).

---

## 6. DCA & S² Attention

- **DCA (Dynamic Contextual Attention)**: Adjusts attention dynamically based on input.
- **S²-Attention (Shifted-Window or Spatial Attention)**: Often used in vision transformers to capture spatial context.

---

## 🚀 Getting Started

```bash
git clone https://github.com/yourusername/attention-mechanisms.git
cd attention-mechanisms
