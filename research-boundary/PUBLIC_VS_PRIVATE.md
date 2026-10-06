# Public vs Private

This repository is a public research layer, not a technical disclosure of the underlying system.

The goal is to make the research problem understandable while keeping the implementation that solves it private.

## Public

Public material may include:

- problem framing
- conceptual distinctions
- high-level principles
- comparative reasoning
- thought experiments
- research questions
- references
- broad statements about the research direction
- public benchmark fixtures and aggregate evidence

## Private

Private material may include:

- implementation architecture
- formal schemas and internal representations
- proprietary mechanisms
- internal decision procedures
- internal scoring or thresholds
- operational workflows
- private datasets
- evaluation datasets and internal benchmarks
- experimental results that reveal mechanisms
- safety and governance implementation details
- integration specifics
- internal nomenclature whose meaning reveals system structure
- combinations of individually harmless details that materially improve reconstructability

## Disclosure test

For every proposed publication, ask:

> **Could a technically capable reader combine this information with the rest of the repository and derive a materially similar implementation path?**

If the answer approaches yes, the material belongs outside the public repository.

The boundary is based on reconstructability, not on whether one sentence looks harmless by itself.

## Research principle

The public layer should make the intellectual problem understandable.

The private layer should retain the mechanisms that solve it.
