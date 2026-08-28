<h1 align="center">shyringo</h1>

<p align="center">
  <strong>Building local AI systems that bring large open models to laptop CPUs.</strong><br>
  专注于让大模型在普通笔记本 CPU 上真正可用。
</p>

<p align="center">
  Native C · CPU inference · low-memory runtimes · reproducible performance
</p>

<p align="center">
  <a href="https://shyringo.github.io/shyringo/"><strong>Open the Laptop LLM Finder</strong></a>
</p>

## Featured projects

### [DeepSeek-V4-Flash-0731 in C](https://github.com/shyringo/deepseek-v4-flash-0731-in-c)

Run the native **284B-A13B DeepSeek-V4-Flash-0731** checkpoint on one laptop
CPU. The pure C engine streams cold MoE experts from disk, has a tested **8 GB
RAM** path, needs no GPU or Python, and reaches **1.12 token/s** in its best
documented prompt-lookup workload. It supports terminal chat and a resident
local OpenAI-compatible API with live token streaming, parallel function calls,
and matched tool-result replay.

<p align="center">
  <a href="https://github.com/shyringo/deepseek-v4-flash-0731-in-c">
    <img src="https://raw.githubusercontent.com/shyringo/deepseek-v4-flash-0731-in-c/main/docs/assets/terminal-demo.png" alt="DeepSeek-V4-Flash-0731 running through the native C engine on a laptop CPU">
  </a>
</p>

### [Qwen3.8-27B in C](https://github.com/shyringo/qwen3.8-27b-in-c)

Run **Qwen3.8-27B** locally on one laptop CPU with a native C engine, direct
GGUF loading, an **8 GB RAM** tested path and measured generation up to **2.52
token/s**. Chat in the terminal or connect local apps through its resident
OpenAI-compatible API. Runtime speedups preserve byte-identical full logits
against the native baseline for the same GGUF.

<p align="center">
  <a href="https://github.com/shyringo/qwen3.8-27b-in-c">
    <img src="https://raw.githubusercontent.com/shyringo/qwen3.8-27b-in-c/main/docs/assets/terminal-demo.png" alt="Qwen3.8-27B running through the native C engine on a laptop CPU">
  </a>
</p>

## Engineering focus

- Native inference engines instead of wrappers around external runtimes
- Low-bit CPU kernels, bounded memory planning and storage-aware execution
- Reproducible TTFT, TPOT, memory and correctness evidence
- User paths that go from clone to a real conversation without a GPU

