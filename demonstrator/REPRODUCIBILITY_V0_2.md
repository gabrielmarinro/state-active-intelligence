# Reproducibility Description — Version 0.2

## What another researcher can inspect

Version 0.2 makes the public research method inspectable through:

- the controlled benchmark scenarios
- the public rubric
- the evaluation protocol
- the scoring scale
- the applicable-dimension rule
- the aggregate calculation
- judge-agreement reporting
- adjudication reporting

This makes the public research fixtures and scoring interpretation available for methodological replication.

## Evaluation flow

At the public methodological level:

1. the same case set is presented to a model or system;
2. one response is obtained for each case;
3. only dimensions applicable to that case are scored;
4. each applicable dimension receives 0, 1 or 2 points;
5. awarded points are compared with the total possible points;
6. results from two judge configurations are compared;
7. disagreements are reviewed against the public rubric;
8. aggregate adjudicated results are reported.

## What is not reproduced

The public repository intentionally does not publish:

- internal prompts
- generation harnesses
- evaluator implementation
- raw model outputs
- raw evaluation runs
- local execution traces
- private experiments
- implementation-specific mechanisms

Those materials remain outside the public research boundary.

## What reproducibility means here

This release supports **methodological replication**, not bit-for-bit reproduction of the private execution environment.

The objective is to make the public question, fixtures, evaluation criteria and evidence structure inspectable without exposing an implementation path that could materially reproduce proprietary mechanisms.
