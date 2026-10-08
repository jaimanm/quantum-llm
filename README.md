# quantum-llm

Research project exploring **LLM-oriented representations for quantum programming**.

The core question is whether a quantum programming representation can let an LLM focus on the intended quantum computation instead of spending generation effort on framework-specific imports, setup, API conventions, execution plumbing, and other boilerplate.

## Approach

We plan to:

1. Select framework-independent quantum programming tasks from **Qiskit HumanEval (QHE)**.
2. Implement the same tasks in Qiskit, PennyLane, Cirq, and OpenQASM where applicable.
3. Measure how much framework-specific overhead each representation exposes to the model.
4. Determine whether an existing representation such as OpenQASM is sufficient.
5. If needed, design a compact quantum language/DSL optimized for LLM generation.
6. Build a parser/compiler/runtime that handles framework-specific setup and execution.
7. Compare representations using functional correctness, token usage, error types, and repairability.
8. Run ablations to identify which language-design choices actually help.

The current focus is **representation design**, not modifying an LLM tokenizer or training a new model.

See [RESEARCH_PLAN.md](RESEARCH_PLAN.md) for the full research plan.

## Anchor References

- **Qiskit HumanEval: An Evaluation Benchmark For Quantum Code Generative Models** (2024)  
  https://arxiv.org/abs/2406.14712
- **QuanBench+: A Unified Multi-Framework Benchmark for LLM-Based Quantum Code Generation** (ICLR 2026)  
  https://arxiv.org/abs/2604.08570

## Status

Early-stage research and benchmarking.
