# 🤖 Spittoon-Study: Multi-LLM Narrative Generation Experiment

[![Online Tool](https://img.shields.io/badge/Try%20Online-Limited%20Time-brightgreen)](https://spittoon-scribe.oragenai.com/)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> An experimental comparison of narrative generation capabilities across 6 leading LLM models using OpenRouter

## 🌟 Overview

This repository showcases an experiment in AI-powered narrative generation, where **the same story was written 6 times** using different state-of-the-art language models. By using identical input (a LoreBook) and the same narrative framework, we can compare how different models approach creative writing, storytelling, and world-building.

**Try the tool online (limited time availability):** [https://spittoon-scribe.oragenai.com/](https://spittoon-scribe.oragenai.com/)

## 🧪 The Experiment

### Methodology

- **Input Source**: [`the-last-machine.md`](the-last-machine.md) - A compelling short story about the last machine on Earth, used as a LoreBook to establish narrative context, themes, and world-building elements
- **Generation Framework**: NSL (Narrative Specification Language) for structured story generation
- **Provider**: OpenRouter API for unified access to multiple LLM providers
- **Output**: Each model generated a complete narrative with associated bucket files (RAG store, generated pages, NSL bucket file)

### What's Included

Each output folder contains:
- **Narrative Bucket** (`.zip`) - RAG store with contextual information
- **Generated Story** (`.zip`) - The complete generated narrative
- **NSL File** (`.nsl`) - Narrative structure specification

## 💰 Cost & Performance Analysis

| Metric | Finding |
|--------|---------|
| **Cost Range** | $0.01 - $0.03 per generation |
| **Most Economical** | DeepSeek v3.2 (~$0.01) |
| **Fastest** | Grok-4-Fast |
| **Most Expensive** | Claude Haiku 4.5 (10x cost premium) |

All generations were run with the same parameters and input, making this a fair comparison of model capabilities at different price points.

## 🎯 Models Used

Six cutting-edge language models were selected for this experiment:

| Model | Provider | Output Folder |
|-------|----------|---------------|
| **IBM Granite 4.0 H Micro** | IBM | [`outputs/granite40/`](outputs/granite40/) |
| **Claude Haiku 4.5** | Anthropic | [`outputs/haiku45/`](outputs/haiku45/) |
| **Llama 3.3 Nemotron Super 49B v1.5** | NVIDIA | [`outputs/Llama33-nemotronSuper/`](outputs/Llama33-nemotronSuper/) |
| **Cydonia 24B v4.1** | TheDrummer | [`outputs/cydonia41/`](outputs/cydonia41/) |
| **DeepSeek v3.2 Exp** | DeepSeek | [`outputs/deepseek32/`](outputs/deepseek32/) |
| **Grok-4-Fast** | X.AI | [`outputs/grok4fast/`](outputs/grok4fast/) |

Full model identifiers can be found in [`openrouter-models.md`](openrouter-models.md).

## 📂 Repository Structure

```
outputs/
├── cydonia41/
│   ├── rememberingcydonia-bucket.zip
│   ├── rememberingcydonia-story.zip
│   └── rememberingcydonia.nsl
├── deepseek32/
│   ├── remeberingdeepseek32-bucket.zip
│   ├── remeberingdeepseek32-story.zip
│   └── remeberingdeepseek32.nsl
├── granite40/
│   ├── rememberinggranite-bucket.zip
│   ├── rememberinggranite-story.zip
│   └── rememberinggranite.nsl
├── grok4fast/
│   ├── remeberinggrok4fast-bucket.zip
│   ├── remeberinggrok4fast-story.zip
│   └── remeberinggrok4fast.nsl
├── haiku45/
│   ├── theremembering-bucket.zip
│   ├── theremembering-story.zip
│   └── theremembering.nsl
└── Llama33-nemotronSuper/
    ├── therememberingnemo-bucket.zip
    ├── therememberingnemo-story.zip
    └── therememberingnemo.nsl
```

## 📖 NSL Specification

For more information about the Narrative Specification Language (NSL) used in this project, see:
- [NSL Specification Documentation](#) *(to be filled)*

## 🔍 Key Observations

This experiment reveals fascinating differences in how various models approach:
- **Narrative coherence** and story structure
- **World-building** detail and consistency
- **Character development** and emotional depth
- **Stylistic choices** and prose quality
- **Thematic interpretation** of the source material

Each model brings unique strengths to creative writing tasks, and this repository serves as a reference for researchers, developers, and AI enthusiasts interested in comparative LLM performance for creative applications.

## 🚀 Getting Started

1. Clone this repository
2. Explore the [`outputs/`](outputs/) directory to compare different model generations
3. Review [`the-last-machine.md`](the-last-machine.md) to understand the source material
4. Try the online tool at [https://spittoon-scribe.oragenai.com/](https://spittoon-scribe.oragenai.com/) (limited availability)

## 📚 Citation

### Academic Citation

If you use this codebase in your research or project, please cite:

```bibtex
@software{spittoon_study,
  title = {Spittoon-Study: Multi-LLM Narrative Generation Experiment},
  author = {Drift Johnson},
  year = {2025},
  url = {https://github.com/MushroomFleet/Spittoon-Study},
  version = {1.0.0}
}
```

## 💖 Support This Work

If you find this project useful or interesting, consider supporting future experiments:

[![Ko-Fi](https://cdn.ko-fi.com/cdn/kofi3.png?v=3)](https://ko-fi.com/driftjohnson)

---

**Note**: This is an experimental research project. Results may vary based on model versions, prompt engineering, and API parameters at the time of generation.
