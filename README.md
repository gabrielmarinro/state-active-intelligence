# State-Active Intelligence (SAI)

## Every failed decision has a human state behind it. SAI finds it before failure.

AI is becoming very good at knowing things.

It can specialize in medicine, law, finance, operations and many other fields. It can analyze large amounts of information, find patterns, make predictions and recommend actions.

A different problem appears when **the person or system being analyzed changes while the intelligence is still using what it learned before**.

A patient can change. A customer can change. A business can change. A fleet can operate under different conditions tomorrow than it did yesterday.

State-Active Intelligence explores what intelligence needs to do when **what was true before may no longer be the best description of what is true now**.

## The idea

A conventional intelligence system can be thought of as:

**observe → understand → predict**

State-Active Intelligence asks what happens when the loop continues:

**observe → understand → predict → act → observe again**

The important difference is that what happens next can change because of the person, the environment, the decision or the action itself.

The research therefore focuses on:

- changing human and system state
- changing context
- uncertainty and incomplete information
- human agency
- intervention and its consequences
- feedback over time
- when historical information stops being representative

## Why this matters

Knowing more about someone does not automatically mean understanding them better.

Historical behavior can remain useful while becoming less representative. A prediction can be correct and still fail because the person changes. An intervention can change the conditions that the intelligence was originally trying to understand.

The research question is therefore simple:

> **How should intelligence reason when the thing it is trying to understand keeps changing?**

## Public research

This repository is the public research layer.

It explains the problem, the conceptual shift, the research questions, selected concepts, comparisons, thought experiments and public evaluation work.

It does not publish the implementation-specific mechanisms of the underlying private system.

## Public demonstrator

The repository includes a public demonstrator across healthcare, legal, finance and fleet operations.

It tests a simple distinction:

**When something important changes, does the intelligence recognize that it should reconsider its interpretation? And when the new information is only noise, does it know when not to change?**

See [demonstrator/README.md](demonstrator/README.md), [demonstrator/CASEBOOK.md](demonstrator/CASEBOOK.md) and [demonstrator/RESULTS.md](demonstrator/RESULTS.md).

## Status

State-Active Intelligence is an active research direction.

The public material describes research questions and public evidence. It should not be interpreted as a claim that every capability described here has been independently validated in production.

## Repository map

- [THE_PROBLEM.md](THE_PROBLEM.md): why changing people and systems create a different intelligence problem
- [THE_SHIFT.md](THE_SHIFT.md): the move from static prediction to reasoning across change
- [DESIGN_PRINCIPLES.md](DESIGN_PRINCIPLES.md): public principles
- [OPEN_QUESTIONS.md](OPEN_QUESTIONS.md): unresolved research questions
- [REFERENCES.md](REFERENCES.md): public research trail
- [comparative/](comparative/): related intelligence paradigms
- [concepts/](concepts/): public conceptual vocabulary
- [thought-experiments/](thought-experiments/): cases that expose the limits of conventional reasoning
- [research-boundary/PUBLIC_VS_PRIVATE.md](research-boundary/PUBLIC_VS_PRIVATE.md): disclosure boundary
