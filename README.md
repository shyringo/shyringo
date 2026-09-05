<h1 align="center">shyringo</h1>

<p align="center">
  <strong>On AI.</strong><br>
  关注 AI，也动手做 AI —— 训练、推理、评测，以及开源生态。
</p>

<p align="center">
  LLM training · inference engines · model evaluation · open-source AI
</p>

<p align="center">
  <a href="https://shyringo.github.io/shyringo/"><strong>Open the Laptop LLM Finder</strong></a>
</p>

## Featured projects

### [Qwen3.8-Flash-Next in C](https://github.com/shyringo/qwen3.8-flash-next-in-c)

Run the **best model under 200B** on a single laptop CPU with a purpose-built
native C inference engine. The practical minimum is **12 GB RAM**; no GPU,
Python, PyTorch, model conversion or external inference runtime is required.
Measured performance reaches **9.89 positions/s** for exact batch-4 verification
and **5.03 token/s** in resident single-conversation chat. Runtime optimizations
add no approximation beyond the selected quantized GGUF.

### [DeepSeek-V4-Flash-0731 in C](https://github.com/shyringo/deepseek-v4-flash-0731-in-c)

Run the native **284B-A13B DeepSeek-V4-Flash-0731** checkpoint on one laptop
CPU. The pure C engine streams cold MoE experts from disk, has a tested **8 GB
RAM** path, needs no GPU or Python, and reaches **1.12 token/s** in its best
documented prompt-lookup workload. It supports terminal chat and a resident
local OpenAI-compatible API with live token streaming, parallel function calls,
and matched tool-result replay.

<p align="center">
  <a href="https://github.com/shyringo/deepseek-v4-flash-0731-in-c">
    <img src="https://repository-images.githubusercontent.com/1336167566/9659b555-d233-44e5-b3f4-5a90670c3e3f" alt="DeepSeek-V4-Flash-0731 in C — native inference on a laptop CPU">
  </a>
</p>

### [Qwen3.8-27B in C](https://github.com/shyringo/qwen3.8-27b-in-c)

Run **Qwen3.8-27B** locally on one laptop CPU with a native C engine, direct
GGUF loading, an **8 GB RAM** tested path and measured generation up to **2.52
token/s**. Chat in the terminal or connect local apps through its resident
OpenAI-compatible API with parallel function calls and tool-result replay.
Runtime speedups preserve byte-identical full logits
against the native baseline for the same GGUF.

<p align="center">
  <a href="https://github.com/shyringo/qwen3.8-27b-in-c">
    <img src="https://repository-images.githubusercontent.com/1345107493/adcd759d-84c1-463d-affe-7e4aab08c9a7" alt="Qwen3.8-27B in C — native inference on a laptop CPU">
  </a>
</p>

## What I work on

- **Training**: RL-scaling post-training frameworks for LLMs, plus training
  experiments that fit on a laptop CPU — with benchmark evidence
- **Inference**: native engines (pure C) that bring large open models to
  ordinary hardware, with reproducible performance and correctness evidence
- **Evaluation**: probing what models truly believe — profiling the ideology
  of any foundation model
- **Open-source AI**: curating and maintaining resources across LLM inference,
  local AI, small language models, Chinese LLMs and AI developer tools