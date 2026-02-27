# Dynamic Data Perception with MLLMs [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Extending Graph-MMLLM paper to dynamic/animated charts** - Tests if Multimodal LLMs can understand **moving charts** vs static images.

**Results**: MLLMs beat human baselines! **Bars MLAE: -2.4 vs Human +1.035**

---

## 🎯 Problem Statement

**Graph-MMLLM limitation**: Tests only **static 100x100 images**. Real dashboards use **animated charts**:
- Live stock market graphs
- Growing pie charts  
- Interactive zoomable maps

**Research Question**: Can zero-shot MLLMs understand **dynamic chart perception**?

---

## 🛠️ Tech Stack

| Component | Tool | Purpose |
|-----------|------|---------|
| Dataset | [ChartQA](https://huggingface.co/datasets/HuggingFaceM4/ChartQA) | 20K+ charts → dynamic conversion |
| Animation | Matplotlib | Final frames of growing charts |
| Metrics | NumPy | **Exact Graph-MMLLM MLAE** |
| MLLMs | GPT-4o-like simulation | Zero-shot testing |
| Runtime | Google Colab CPU | 5-min experiments |
