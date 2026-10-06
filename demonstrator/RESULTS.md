# Public Results

## Version 0.2

The current public benchmark contains **28 controlled scenarios** across healthcare, legal, finance and fleet operations.

It includes:

- **24 change-sensitive scenarios**
- **4 stability-control scenarios**
- **8 public evaluation dimensions**
- **7 temporal and contextual patterns**

The benchmark tests both sides of the capability:

**recognize meaningful change — and resist unnecessary change.**

## What the numbers mean

When a situation genuinely changed and the intelligence needed to adapt, the evaluated capability reached **98.6% of the available score**.

When new information should not materially change the interpretation, it reached **91.7%**.

Across the complete evaluation, it reached **97.6%** of the available score after disagreement review.

In plain terms:

> **When reality changed, it usually changed its response. When reality had not meaningfully changed, it usually did not.**

## Evaluation design

The same fixed generated response set was evaluated using two separate judge configurations and the public rubric.

Each applicable dimension received a score from 0 to 2.

Aggregate performance is:

**total awarded points / total applicable points × 100**

Before adjudication:

| Evaluation | Judge A | Judge B |
|---|---:|---:|
| Overall | 94.9% | 96.7% |
| Change-sensitive scenarios | 95.8% | 99.0% |
| Stability-control scenarios | 89.6% | 83.3% |

After disagreement review:

| Evaluation | Adjudicated |
|---|---:|
| Overall | **97.6%** |
| Change-sensitive scenarios | **98.6%** |
| Stability-control scenarios | **91.7%** |

## What the evaluation suggests

The strongest public evidence is that the evaluated responses were able to recognize several forms of change while preserving uncertainty.

The benchmark also shows where the task becomes harder: distinguishing evidence quality, deciding whether context is actually relevant, weighting evidence and interpreting consequences.

Those harder areas are useful because they prevent the benchmark from becoming a simple test of whether the system notices that something changed.

## Judge agreement

Two separate judge configurations agreed exactly on **90.4% of the 167 applicable ratings**.

The remaining disagreements were reviewed against the public rubric and case expectations.

This is a consistency check on the evaluation process, not independent scientific validation.

## What this does not establish

The benchmark does not establish production performance or prove that one architecture, model or implementation is superior.

It also does not publish private prompts, internal representations, evaluator implementation, raw runs, private datasets or proprietary mechanisms.
