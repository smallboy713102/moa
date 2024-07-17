# Mixture of Agents Implementation using Llama APIs

This project demonstrates a loose implementation of the "Mixture of Agents" concept using Llama APIs. The approach involves creating multiple instances of a Llama model to independently generate responses (`proposer` models) and then aggregating these responses into a single, coherent answer using another Llama model (`aggregator`). Each layer progressively refines the response by taking the initial user query and the previous layer's output.

## Features

- **Layered Architecture**: Uses multiple layers to refine responses through deeper reasoning.
- **Proposer Models**: Three instances of Llama models that independently generate responses.
- **Aggregator Model**: Aggregates the responses from proposer models into a single, high-quality response.

## Requirements

- Python 3.x
- Llama API
