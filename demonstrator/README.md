# Human-Context-Aware Intelligence

## Public Demonstrator

### From specialized AI to intelligence that can understand the person behind the problem

AI can already specialize in medicine, legal, finance or fleet operations. It can analyze information, detect patterns, diagnose, recommend or predict risk.

**But knowing the right decision does not mean knowing whether the person will actually carry it out.** A medical AI can identify the right treatment and the patient can still stop it.

State-Active Intelligence seeks to add that missing dimension: **understanding the person, what they are going through, how their behavior is changing and what factors may cause them to make — or stop making — a particular decision.**

In medicine, for example, the question becomes not only:

**“What treatment does this patient need?”**

but also:

**“Will they finish it? What will make them stop? When will the warning signs appear? What could prevent that?”**

That is the distinction this public demonstrator begins to test.

## Public evidence

The demonstrator covers healthcare, legal, finance and fleet operations.

Across **28 controlled scenarios**, it tests both sides of the problem:

- when something important changes, intelligence should recognize that it matters;
- when new information is only noise, intelligence should not change unnecessarily.

When a scenario required adaptation because something important had changed, the evaluated capability reached **98.6% of the available score**.

When the new information should not materially change the interpretation, it reached **91.7%**.

In other words:

**when reality changed, it usually changed its response; when reality had not meaningfully changed, it usually did not.**

The full methodology and evidence are available in [RESULTS.md](RESULTS.md), [benchmark/JUDGE_AGREEMENT_V0_2.md](benchmark/JUDGE_AGREEMENT_V0_2.md), [benchmark/ADJUDICATION_SUMMARY_V0_2.md](benchmark/ADJUDICATION_SUMMARY_V0_2.md) and [REPRODUCIBILITY_V0_2.md](REPRODUCIBILITY_V0_2.md).

## Methodological note

The public benchmark uses controlled research scenarios across four domains. It is intended to make the research question and observable evaluation behavior inspectable; it is not a claim of production validation.

## Public boundary

The demonstrator intentionally does not publish the private implementation mechanisms, internal representations, prompts, evaluator implementation, raw runs, private datasets or system-specific operational workflows.

The research question is public.

The mechanism remains private.
