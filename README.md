# State-Active Intelligence

## A research direction for intelligence operating on evolving systems

State-Active Intelligence is a public research layer exploring a class of AI problems that emerge when the object of reasoning changes over time and intelligence can become part of the conditions that shape what happens next.

A static representation can describe a system at one moment. A useful intelligence system must also remain epistemically disciplined as observations accumulate, conditions change and consequences become new evidence.

The research therefore examines the relationship among:

**observation → interpretation → prediction → decision → action → consequence → changed conditions**

The sequence is conceptual. Implementation remains private.

## Why this matters

Many intelligence systems are evaluated as though the target were stable enough for a forecast to remain meaningful after it is produced. Many real systems violate that assumption.

People change. Organizations change. Environments change. Constraints change. Intentions change. An action can also alter the conditions that later observations describe.

This creates a deeper problem than prediction accuracy:

> **How should intelligence reason when the system being modeled evolves and intelligence may influence that evolution?**

The answer requires more than better models. It requires explicit treatment of evidence, uncertainty, time, agency, change and consequences.

## Public research scope

This repository documents the public conceptual layer of the research:

- problem framing
- epistemic distinctions
- high-level principles
- comparative positioning
- thought experiments
- research questions
- public references
- explicit boundaries around unpublished work

The repository is designed to make the intellectual direction inspectable while keeping implementation-specific mechanisms private.

## Epistemic discipline

A central concern is maintaining the distinction among:

**what is established → what was observed → what is inferred → what is predicted → what was decided → what subsequently occurred**

These categories can interact. They remain conceptually distinct.

A claim becoming plausible does not make it observed. Repeated observation does not establish causality by itself. A prediction followed by an outcome does not establish that the prediction caused the outcome.

That discipline becomes increasingly important as intelligence moves from passive analysis toward action.

## Human systems

Human behavior is especially challenging because a person can change across time, context and circumstance.

Historical behavior can remain informative while becoming less representative. A declared intention can differ from observed behavior. An intervention can influence attention or behavior. External conditions can change independently.

The research therefore treats human-centered intelligence as an evolving-system problem rather than a static-profile problem.

## Research boundary

This repository deliberately excludes unpublished implementation details that could make the underlying system reconstructible.

That includes proprietary mechanisms, formal internal representations, operational procedures, decision criteria, private evaluation artifacts, implementation architecture, internal datasets and other material whose disclosure would materially reduce the separation between the public research layer and the private system.

The public layer communicates **what problem is being explored, why it matters and which conceptual distinctions are useful**.

It leaves the private **how** outside the repository.

## Status

State-Active Intelligence is an active research direction.

Published material should be read as conceptual research and hypothesis formation. It does not imply that every capability described here has been implemented or empirically validated.

## Repository map

- [THE_PROBLEM.md](THE_PROBLEM.md): problem framing
- [THE_SHIFT.md](THE_SHIFT.md): conceptual shift
- [DESIGN_PRINCIPLES.md](DESIGN_PRINCIPLES.md): public design principles
- [OPEN_QUESTIONS.md](OPEN_QUESTIONS.md): unresolved research questions
- [REFERENCES.md](REFERENCES.md): public research trail
- [comparative/](comparative/): neighboring paradigms
- [concepts/](concepts/): public conceptual vocabulary
- [thought-experiments/](thought-experiments/): boundary cases and implications
- [research-boundary/PUBLIC_VS_PRIVATE.md](research-boundary/PUBLIC_VS_PRIVATE.md): disclosure boundary
