<!--
SPDX-FileCopyrightText: Copyright (c) 2024-2025 NVIDIA CORPORATION & AFFILIATES. All rights reserved.
SPDX-License-Identifier: Apache-2.0
-->

# Dynamo
[Dynamo](https://github.com/ai-dynamo/dynamo) is an inference serving framework optimized for data center scale deployments with the flexibility needed to meet the complex use cases of Generative AI.

This GitHub organization hosts repositories for Dynamo's core components and integrations, including:

**Core Framework**
- Distributed runtime system with Rust-based orchestration
- Python bindings for workflow customization
- Multi-GPU/multi-node serving capabilities

**Key Components**
- Disaggregated Serving Engine: Decoupling of prefill and decode to optimize for throughput at latency SLOs
- Intelligent Routing System: Prefix-based and load-aware request distribution
- KV Cache Management: Distributed KV Cache management

## Getting Started
For initial setup and local deployment:
1. Use containerized builds with Docker
2. Choose between monolithic or disaggregated deployments
3. Leverage pre-configured components to build your own inference workflows 

Refer to our [Quickstart Guide] for container setup and basic workflows.

## Documentation
- [Architecture Deep Dive](./lib/runtime/README.md) (lines 17-116 in lib/runtime/README.md)
- [API Reference](./lib/bindings/python/README.md) (lines 18-108 in python bindings README)
- [Production Deployment Guidelines](./deploy/Kubernetes/README.md) (lines 60-84 in values.yaml)

## Key Tools
- **llmctl**: Model management CLI for HTTP endpoints (lines 97-202 in tensorrt_llm/README.md)
- **KV Router**: Prefix-aware request distribution system
- **Model Navigator**: Containerized model optimization pipeline

## Contribution & Support
- Follow [Contribution Guidelines](./CONTRIBUTING.md) (lines 1-94 in CONTRIBUTING.md)
- Report issues via GitHub Discussions
- Enterprise support available through NVIDIA AI Enterprise

## License
Apache 2.0 licensed with third-party attributions documented in [ATTRIBUTIONS.md](./ATTRIBUTIONS.md) (lines 1-2656 in ATTRIBUTIONS.md)

> [!NOTE]
> This project is currently in alpha stage - APIs and components may evolve based on community feedback (lines 34-38 in main README.md)