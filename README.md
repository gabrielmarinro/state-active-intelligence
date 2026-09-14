# State-Active Intelligence

## Intelligence that does more than observe or predict state

State-Active Intelligence is a research and architecture framework for a class of AI systems that operate on changing state.

The central question is:

> **What happens when intelligence does more than observe and predict a system, and its own interventions can change the state being modeled?**

A human is a dynamic system rather than a static profile.

Experience, behavior, cognition, context, constraints and environment can change over time. The same person may therefore behave differently under different conditions, and historical patterns may lose predictive relevance.

This creates a different intelligence problem.

The system must reason about:

**state → context → uncertainty → prediction → decision → intervention → consequence → new state**

The intervention can affect the system.

The environment can change the system.

The system can change independently of the intervention.

The resulting state can change what becomes likely next.

## Research direction

State-Active Intelligence explores the architectural and epistemic requirements for intelligence systems operating within evolving systems.

The research focuses on questions involving:

- changing human state
- changing environments
- uncertainty and incomplete observability
- human agency
- intervention effects
- consequences and feedback
- temporal adaptation
- reproducible and auditable decision processes

The work distinguishes what is known, observed, inferred and subsequently observed to preserve epistemic discipline as state evolves.

## The Shift

Traditional intelligence can be represented as:

**observe → infer → predict**

State-active intelligence asks what happens when the loop continues:

**observe → understand → predict → act → observe again → learn**

The important distinction is that action can influence the state being modeled.

## Design Principles

The research follows a small set of principles:

1. **Model the real human**  
   Humans are dynamic rather than static profiles.

2. **Separate epistemic states**  
   Observation, inference, prediction, decision and outcome remain distinct.

3. **Preserve human agency**  
   Recommendation, intervention and human decision are different concepts.

4. **Model uncertainty explicitly**  
   Unknown and uncertain states remain explicit.

5. **Account for change**  
   Human behavior and environments evolve over time.

6. **Close the loop**  
   New state becomes evidence for subsequent reasoning.

7. **Treat intervention as part of the system**  
   Intelligence can influence the state it is attempting to understand.

## Research Boundary

This repository describes the research problem, conceptual framework, principles and open questions.

It intentionally does not publish implementation-specific architectures, proprietary decision logic, protected research artifacts or unpublished mechanisms.

## Open Questions

The repository documents unresolved questions around:

- how human state should be represented as it changes
- how changing environments should be incorporated
- how historical patterns should be reconciled with current evidence
- how intervention effects should be evaluated
- how human agency should constrain intervention
- how uncertainty should propagate through closed decision loops
- how such systems should remain auditable as both the human and the environment evolve

## Status

State-Active Intelligence is an active research and architecture effort.

Conceptual material published here should be understood as a research direction rather than as a claim that all proposed capabilities have been empirically validated.

## Public Research

This repository contains the public research layer of the work, including:

- the problem definition
- the conceptual shift
- design principles
- research questions
- selected concepts
- research boundaries
- thought experiments
- public references
