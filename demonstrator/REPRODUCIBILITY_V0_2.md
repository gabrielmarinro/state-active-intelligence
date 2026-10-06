# Reproducibility Description — Version 0.2

## Publicly reproducible components

Version 0.2 exposes the following research inputs:

- the synthetic benchmark cases;
- the public rubric;
- the evaluation protocol;
- the scoring scale;
- the applicable-dimension concept;
- the aggregate calculation;
- the judge-agreement reporting method;
- the adjudication reporting method.

The benchmark therefore allows an external reader to inspect the research fixtures and reproduce the public scoring interpretation.

## Evaluation flow

At a methodological level, the evaluation consists of:

1. presenting the same synthetic case set to a model or system;
2. obtaining one response per case;
3. evaluating each response only against dimensions applicable to that case;
4. assigning a 0–2 score per applicable dimension;
5. aggregating awarded points against total possible points;
6. comparing results across two judge configurations;
7. reviewing disagreements against the public rubric;
8. reporting aggregate adjudicated results.

## Scope of reproducibility

This release supports **methodological replication**, not bit-for-bit computational reproduction.

The following execution details are intentionally not published:

- internal prompts;
- generation harnesses;
- evaluator implementation;
- raw model outputs;
- raw evaluation runs;
- local execution traces;
- private experiments;
- implementation-specific mechanisms.

Those materials are retained locally and are outside the public research boundary.

## Why the boundary exists

The purpose of the public repository is to expose the research question, experimental fixtures, evaluation logic and aggregate evidence without exposing an implementation path that could materially reproduce proprietary mechanisms.

Reproducibility is therefore defined here at the level of the public research method and evidence structure, rather than disclosure of the complete internal execution stack.
