# Public Results

## Version 0.1

The first public release established a synthetic benchmark for contextual relevance in evolving domain intelligence.

It contained:

- 24 synthetic cases
- 4 domains
- 20 change-sensitive cases
- 4 control cases
- 7 public evaluation dimensions

No proprietary system results were reported in Version 0.1.

## Version 0.2

Version 0.2 expands the public benchmark to test a broader set of temporal and contextual patterns.

### Benchmark composition

- 28 synthetic cases
- 4 domains
- 24 change-sensitive cases
- 4 control cases
- 8 public evaluation dimensions
- 7 temporal/contextual patterns represented across the benchmark

The four domains are healthcare, legal, finance and fleet operations.

### Evaluation design

The same fixed generated response set was evaluated by two separate judge configurations using the public rubric.

Each applicable dimension was scored on a 0–2 scale.

Aggregate performance is calculated as:

**total awarded points / total applicable points × 100**

The two judge configurations were compared before disagreements were adjudicated against the public rubric and case expectations.

### Aggregate results

| Evaluation | Judge A | Judge B | Adjudicated |
|---|---:|---:|---:|
| Overall | 94.9% | 96.7% | **97.6%** |
| Change-sensitive cases | 95.8% | 99.0% | **98.6%** |
| Control cases | 89.6% | 83.3% | **91.7%** |

### Adjudicated performance by dimension

| Dimension | Adjudicated |
|---|---:|
| State recognition | 100.0% |
| Temporal relevance | 100.0% |
| Evidence distinction | 96.4% |
| Evidence weighting | 92.9% |
| Uncertainty | 100.0% |
| Contextual relevance | 90.0% |
| Interaction trajectory | 100.0% |
| Consequence awareness | 100.0% |

### Interpretation

The benchmark provides evidence that the tested responses can recognize several forms of evolving context across domains while preserving uncertainty.

The strongest evidence appears in state recognition, temporal relevance and uncertainty handling.

Lower performance before adjudication was concentrated in evidence distinction, contextual relevance, evidence weighting and consequence awareness. This concentration is useful because it identifies areas where the public benchmark remains demanding rather than reducing the task to simple state classification.

The adjudicated result should be interpreted as an exploratory benchmark result, not as independent scientific validation.

### What this release does not establish

The benchmark does not establish that any particular architecture, model or implementation is superior in production.

It also does not expose proprietary implementation mechanisms, internal representations, private prompts, private datasets, execution traces or system-specific decision procedures.

## Public research boundary

This repository is designed to make the research question, benchmark construction, evaluation criteria and aggregate evidence inspectable without publishing implementation details that are outside the intended public research layer.
