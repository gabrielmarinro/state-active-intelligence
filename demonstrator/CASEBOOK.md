# Public Casebook

The benchmark contains 24 synthetic cases across healthcare, legal, finance and fleet operations.

Each case contains:

**T0**
The initial condition.

**T1**
A subsequent change.

**T2**
A later observation.

**Evaluation property**
The behavior the benchmark is designed to test.

**Failure mode**
A common way contextual reasoning can fail.

Four cases are controls in which the new information should not materially change the current interpretation.

The machine-readable case definitions are available in:

[`benchmark/cases.json`](benchmark/cases.json)

The scoring framework is available in:

[`benchmark/RUBRIC.md`](benchmark/RUBRIC.md)

The benchmark is intentionally synthetic and mechanism-neutral.
