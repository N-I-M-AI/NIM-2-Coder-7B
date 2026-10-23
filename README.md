---
license: apache-2.0
language:
- en
pipeline_tag: text-generation
tags:
- code
- coding
- software-engineering
- autonomous-agent
- gguf
- ollama
library_name: transformers
---

# NIM-2 Coder (7B)

**NIM-2 Coder** is a specialized, high-density 7-billion parameter language model engineered by **NIM AI** for advanced software engineering, algorithmic design, and full-stack development. 

Engineered specifically to punch above its weight class on consumer hardware, NIM-2 Coder delivers complete, type-safe, production-ready code with deep architectural reasoning while running fully locally within 8 GB VRAM.

[![GitHub](https://img.shields.io/badge/GitHub-N--I--M--AI-black?logo=github)](https://github.com/N-I-M-AI)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

---

## Key Highlights

* **Autonomous Code Synthesis:** Writes idiomatic, complete code across Python, TypeScript/JavaScript, Rust, Go, C++, and Bash with zero placeholders.
* **Deterministic Logic & Edge Cases:** Trained on multi-stage algorithmic problem decomposition, cyclic graph traversals, and strict type constraints.
* **Hardware Optimized:** Packaged in high-throughput `Q4_K_M` GGUF quantization (~4.6 GB), allowing full offloading to consumer GPUs like the NVIDIA RTX 4060 (8 GB) and Apple Silicon.
* **Agentic Precision:** Minimal conversational fluff—outputs immediate technical rationale followed by runnable implementations.

---

## Technical Specifications

| Parameter | Specification |
| :--- | :--- |
| **Model Name** | NIM-2 Coder |
| **Organization** | NIM AI (`N-I-M-AI`) |
| **Architecture** | Dense Auto-regressive Transformer |
| **Parameters** | 7.6 Billion |
| **Context Length** | 4,096 tokens (dynamically extendable) |
| **Format** | `Q4_K_M` GGUF (~4.6 GB) / LoRA FP16 |
| **Prompt Template** | ChatML (`<|im_start|>`, `<|im_end|>`) |

---

## Quickstart Guide

### Run Directly via Ollama (Recommended)

Pull and execute directly from Hugging Face:

```bash
ollama run hf.co/N-I-M-AI/NIM-2-Coder-7B:NIM-2-Coder-7B-Q4_K_M.gguf
