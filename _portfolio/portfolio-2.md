---
title: "Nimbus: Burst-Resilient Hybrid Inference for LLMs"
excerpt: "Routing algorithm for real-world LLM services—balancing TTFT SLOs and cost via selective API offload."
collection: portfolio
permalink: /portfolio/nimbus
---

LLM traffic spikes force teams to either overprovision GPUs or miss SLOs. Nimbus predicts TTFT from queue state and uses a budget-aware (knapsack-style) policy to offload the right requests to APIs.

* Queue-state TTFT predictor for admission/offload decisions.
* Cost/SLO-aware routing over a compute budget.
* Deployed in production settings with 25% cost savings under bursty traffic.