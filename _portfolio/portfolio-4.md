---
title: "Agentic AI & LLM Infrastructure"
excerpt: "Evaluated and deployed LLM agents using ReAct and tool-calling strategies, improving task success rates by ~20% with optimized multi-model vLLM serving.<br/>"
collection: portfolio
---

I built and evaluated an agentic AI infrastructure centered on large language model agents, benchmarking reasoning and task-completion capabilities across Qwen3 models ranging from 4B to 32B parameters. The evaluation framework tested agents using both ReAct (reasoning and acting) and tool-calling strategies, surfacing meaningful performance differences across model scales and prompting approaches.

On the infrastructure side, I deployed vLLM for multi-model serving, configuring it for optimized GPU utilization and low-latency inference across concurrent requests. This required profiling and resolving memory and concurrency bottlenecks that emerged under load — improving task success rates by approximately 20% through a combination of better serving configuration and prompt engineering refinements.

The project gave me practical experience with the full LLM deployment stack: from agent architecture and evaluation methodology to inference serving optimization and production-readiness at scale. It also sharpened my understanding of the trade-offs between model size, latency, throughput, and task accuracy in real agentic workloads.
