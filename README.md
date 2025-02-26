# Mixture of Agents Implementation using Llama APIs

The Mixture-of-Agents (MoA) framework represents a groundbreaking advancement in leveraging collaborative interactions among large language models (LLMs) to achieve state-of-the-art performance across multiple benchmarks. By orchestrating a layered architecture where LLMs iteratively refine outputs through an "Aggregate-and-Synthesize" process, MoA demonstrates superior capabilities compared to individual models, including GPT-4 Omni. This repository provides an open-source implementation of MoA, enabling users to harness the collective intelligence of diverse LLMs for advanced text generation tasks.

This project demonstrates a loose implementation of the "Mixture of Agents" concept using Llama APIs. The approach involves creating multiple instances of a Llama model to independently generate responses (`proposer` models) and then aggregating these responses into a single, coherent answer using another Llama model (`aggregator`). Each layer progressively refines the response by taking the initial user query and the previous layer's output.

## Features

- **Layered Architecture**: Uses multiple layers to refine responses through deeper reasoning.
- **Proposer Models**: Three instances of Llama models that independently generate responses.
- **Aggregator Model**: Aggregates the responses from proposer models into a single, high-quality response.

## Requirements

- Python 3.x
- Llama API
