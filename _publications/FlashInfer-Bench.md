---
title: "FlashInfer-Bench: Building the Virtuous Cycle for AI-driven LLM Systems"
collection: publications
permalink: /publication/2026-01-flashinfer-bench
# excerpt: ''
date: 2026-01-01
venue: 'MLSys 2026'
# slidesurl: ''
paperurl: 'https://arxiv.org/abs/2601.00227'
# citation: ''
---

Recent advances show that large language models (LLMs) can act as autonomous agents capable of generating GPU kernels, but integrating these AI-generated kernels into real-world inference systems remains challenging. FlashInfer-Bench establishes a standardized framework with several key components: FlashInfer Trace (a unified schema for kernel definitions and workloads), a curated dataset built on real serving traces, benchmarking tools that evaluate correctness and performance, and a public leaderboard tracking agent capabilities. The system includes a dynamic substitution mechanism that deploys optimized kernels into production engines like SGLang and vLLM.

We evaluate how well LLM agents perform at GPU programming, examine tradeoffs among different programming languages, and offer guidance for future agent development. FlashInfer-Bench establishes a practical, reproducible pathway for continuously improving AI-generated kernels and deploying them into large-scale LLM inference.
