<!--
SPDX-FileCopyrightText: Copyright (c) 2024-2025 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
SPDX-License-Identifier: Apache-2.0
-->

# NVIDIA Dynamo
[Dynamo](https://github.com/ai-dynamo/dynamo) is a new modular inference framework designed for serving large language models (LLMs) in multi-node distributed environments. It enables seamless scaling of inference workloads across GPU nodes and the dynamic allocation of GPU workers to address traffic bottlenecks at various stages of the model pipeline.

This GitHub organization hosts repositories for Dynamo's core components and integrations, including:

**[Core Framework](https://github.com/ai-dynamo/dynamo/tree/main/lib/runtime)**

- Distributed inference runtime with Rust-based orchestration
- Python bindings for workflow customization
- Multi-GPU/multi-node serving capabilities

**[LLM Optimized Components](https://github.com/ai-dynamo/dynamo/tree/main/lib/llm)**

- Disaggregated Serving Engine: Decoupling of prefill and decode to optimize for throughput at latency SLOs
- Intelligent Routing System: Prefix-based and load-aware request distribution
- KV Cache Management: Distributed KV Cache management

**[NVIDIA Optimized Transfer Library (NIXL)](https://github.com/ai-dynamo/nixl)**

- Abstracts memory of heterogeneous devices, i.e., CPU, GPU, storage, and enables most efficient and low-latency communication among them
- Integrates with distributed inference servers such as Dynamo. This library will target distributed inference communication patterns to effectively transfer the KV cache in disaggregated LLM serving platform.

## Getting Started

To learn more about NVIDIA Dynamo Inference Serving Platform, please refer to the [Dynamo developer page](TBD) and read our [Quickstart Guide](TBD) for container setup and basic workflows.

## Documentation

User documentation on Dynamo features, APIs, and architecture is located in the [Dynamo documents folder on GitHub](https://github.com/ai-dynamo/dynamo/tree/main/docs).

## Contribution & Support

- Follow [Contribution Guidelines](./CONTRIBUTING.md) (lines 1-94 in CONTRIBUTING.md)
- Report issues via GitHub Discussions
- Enterprise support available through NVIDIA AI Enterprise

## License

Apache 2.0 licensed with third-party attributions documented in [ATTRIBUTIONS.md](./ATTRIBUTIONS.md) (lines 1-2656 in ATTRIBUTIONS.md)

> [!NOTE]
> This project is currently in alpha stage - APIs and components may evolve based on community feedback (lines 34-38 in main README.md)
