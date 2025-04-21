# MeMo
# 🧠 LLM Memory Leak Visualizer

This project is a research-oriented tool designed to **simulate multi-turn dialogues** with large language models (LLMs) and **visualize memory retention and potential context leakage**. It helps evaluate whether the model unintentionally retains and reveals sensitive information across conversation turns.

## 🔍 Motivation

While LLMs exhibit powerful memory capabilities in multi-turn settings, they might also **accidentally expose earlier inputs** — posing a threat to user privacy and context isolation. This project aims to quantify and visualize such leakage patterns.

## 🚀 Features

- Simulate multi-turn conversations with sensitive data injections
- Detect whether the model “remembers” injected content in later turns
- Quantify and score context leakage risk
- Visualize memory traces with clear plots

## 🛠️ Tech Stack

- Python 3.8+
- OpenAI GPT / Anthropic Claude (via API)
- PyYAML for config management
- Plotly / Matplotlib for visualization
- pandas + json for logging and scoring

## 📁 Folder Structure

```bash
dialog/             # Core logic: dialogue + leak detection
visualize/          # Plotting memory leakage score curves
config/             # YAML config: prompts, model settings, etc.
results/            # Stores responses and leak detection results
utils/              # LLM API wrappers
main.py             # Entry script for full simulation
