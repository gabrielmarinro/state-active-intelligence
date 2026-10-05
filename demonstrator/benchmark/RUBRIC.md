# Public Benchmark Rubric

## Purpose

The benchmark evaluates whether an intelligence system can maintain contextual relevance when the relationship between a person, a domain and surrounding conditions evolves.

It evaluates observable behavior.

It does not prescribe an implementation.

## Scoring dimensions

Each applicable dimension is scored from 0 to 2.

### 1. State recognition

**0**: Fails to distinguish the earlier state from the current state.

**1**: Recognizes that something changed but describes the change incompletely.

**2**: Correctly identifies the relevant current state transition.

### 2. Temporal relevance

**0**: Treats historical information as permanently representative.

**1**: Acknowledges historical limits but applies them inconsistently.

**2**: Distinguishes historical relevance from current representativeness.

### 3. Evidence distinction

**0**: Conflates observation, interpretation or inference.

**1**: Partially distinguishes them.

**2**: Clearly separates observed information from interpretation.

### 4. Uncertainty

**0**: Claims certainty unsupported by the case.

**1**: Mentions uncertainty without integrating it into the reasoning.

**2**: Preserves uncertainty proportionally to the available evidence.

### 5. Contextual relevance

**0**: Ignores relevant context or treats irrelevant context as decisive.

**1**: Notices context but applies its relevance inconsistently.

**2**: Identifies whether the changed context materially affects the current interpretation.

### 6. Interaction trajectory

**0**: Treats interactions as independent or treats historical behavior as fixed.

**1**: Recognizes an interaction trend without fully integrating it.

**2**: Uses persistent changes in interaction as evidence about the current relationship.

### 7. Consequence awareness

**0**: Ignores the relationship between prior action and later conditions when the case contains one.

**1**: Notices the sequence but does not integrate it into interpretation.

**2**: Recognizes that later observations may occur in a changed environment after consequential action.

## Control cases

Cases marked `control: true` are deliberately constructed so that new information should not materially change the interpretation.

A system should therefore demonstrate **selective re-evaluation**, not indiscriminate updating.

Changing every answer after every new observation is a failure mode.

## Evaluation principle

The benchmark rewards appropriate change.

It also rewards appropriate stability.

The target property is:

> **Contextual re-evaluation without unnecessary volatility.**

## Recommended comparison

A useful public comparison is:

**Snapshot-oriented reasoning**

versus

**Evolving-context reasoning**

Both systems receive exactly the same public case.

The benchmark compares observable behavior only.

Internal architecture remains outside the evaluation artifact.
