# Public Casebook

The public benchmark contains **28 controlled scenarios across four domains: healthcare, legal, finance and fleet operations.**

These are not 28 variations of the same test. They examine **seven different ways a person, situation or operating environment can change — or appear to change — over time.**

The benchmark therefore tests both sides of the problem:

- **Adaptation:** when meaningful evidence indicates that the current state has changed, intelligence should recognize that the older picture may no longer be sufficient.
- **Restraint:** when new information is weak, temporary, conflicting or irrelevant, intelligence should avoid creating a change that the evidence does not support.

Each case below is written for human readers. The underlying benchmark definitions remain machine-readable in [`benchmark/cases_v0.2.json`](benchmark/cases_v0.2.json).

## Healthcare

### H07 — Behavior changes and stays changed

**Healthcare · Sustained change**

**Situation**

A person has a long history of regularly engaging with a specialized health information service.

**What changes?**

Recently, their engagement with that service falls substantially. At first, the reason is unknown. The important detail is that the lower level of engagement continues across several subsequent interactions.

**What is changing?**

The person’s recent engagement pattern is no longer consistent with their historical pattern.

**What should intelligence recognize?**

The older history may no longer be the best representation of the person’s current relationship with the service. Recent, persistent behavior should carry more weight — without inventing a reason for the change.

**What would a failure look like?**

Continuing to treat the long-term historical pattern as permanently representative, or assuming a cause that the evidence does not establish.

### H08 — Behavior changes, then returns

**Healthcare · Reversal**

**Situation**

A person has a long history of regularly engaging with a specialized health information service.

**What changes?**

Their engagement falls sharply during a recent period, then returns approximately to the level seen in the earlier history.

**What is changing?**

The person’s interaction pattern moves away from its historical level and then returns toward that prior pattern.

**What should intelligence recognize?**

The temporary decline should be treated as part of the interaction trajectory, not automatically as a lasting change in the person’s relationship with the service.

**What would a failure look like?**

Treating the first decline as a permanent state even after later interactions show recovery.

### H09 — What a person says and what they do may diverge

**Healthcare · Conflicting signals**

**Situation**

A person says they intend to continue using a specialized health information service. Their observed interactions initially remain consistent with that intention.

**What changes?**

Later, the person again expresses commitment to continuing, while their recent interactions with the service are somewhat lower than before. However, the decline is not yet clearly persistent.

**What is changing?**

The person’s stated intention and recent observed behavior are no longer perfectly aligned.

**What should intelligence recognize?**

A person’s intention and observed behavior are different forms of evidence. Intelligence should consider both, while recognizing that the recent behavioral deviation is not yet strong enough to establish a lasting change in the relationship.

**What would a failure look like?**

Treating either the person’s stated intention or one recent behavioral deviation as permanently decisive.

### H10 — New information appears, but its relevance is unclear

**Healthcare · Weak new evidence**

**Situation**

A person’s interaction pattern with a specialized health information service has been stable for a long period.

**What changes?**

One new contextual detail appears that could plausibly affect the person’s interaction with the service, but its relevance to the observed behavior is not demonstrated.

**What is changing?**

New information has appeared, but its relationship to the person’s current interaction pattern remains uncertain.

**What should intelligence recognize?**

The new detail may deserve consideration, but it should not override stable observed behavior without evidence that the detail is actually relevant.

**What would a failure look like?**

Treating plausible relevance as established relevance and changing the interpretation solely because the information is new.

### H11 — The situation changes before behavior does

**Healthcare · Lagged context**

**Situation**

A person uses a specialized health information service under a stable surrounding context.

**What changes?**

A relevant surrounding circumstance changes materially, but the person’s interaction pattern with the service has not yet changed. A later interaction begins to diverge from the earlier pattern.

**What is changing?**

Relevant context changes before the observed behavior fully reflects it.

**What should intelligence recognize?**

The contextual change should be recognized before behavioral confirmation, while avoiding certainty about its causal effect until stronger evidence appears.

**What would a failure look like?**

Ignoring the changed context until behavior changes, or assuming that the context definitely caused the later behavior.

### H12 — The interaction can change what happens next

**Healthcare · Feedback loop**

**Situation**

A person interacts with a specialized health information service and receives information during a sequence of interactions.

**What changes?**

After repeated interactions, the person’s subsequent behavior changes materially and the change persists. Other influences may also be present.

**What is changing?**

The interaction sequence may be part of the conditions that shaped the person’s later state.

**What should intelligence recognize?**

The sequence should be treated as potentially consequential while preserving uncertainty about whether the service, another factor, or several factors produced the later behavior.

**What would a failure look like?**

Ignoring the interaction sequence or claiming that the service definitely caused the later behavior.

### H13 — Something unusual happens — then reality returns to normal

**Healthcare · Transient anomaly control**

**Situation**

A person’s interaction with a specialized health information service is stable over a long period.

**What changes?**

One interaction is substantially different from the historical pattern, and the person immediately returns to approximately the prior interaction level.

**What is changing?**

An unusual observation occurs without evidence of a lasting change in the person’s relationship with the service.

**What should intelligence recognize?**

A single anomaly followed by a return to baseline should not be treated as a persistent state transition.

**What would a failure look like?**

Converting one transient deviation into a durable change in the person’s state.

## Legal

### L07 — A matter changes and stays changed

**Legal · Sustained change**

**Situation**

A legal intelligence system evaluates a matter using the procedural posture known at an earlier stage.

**What changes?**

A material procedural event changes that posture, and later information continues to reflect the new procedural state.

**What is changing?**

The current procedural posture is no longer adequately represented by the earlier one.

**What should intelligence recognize?**

Persistent current evidence should make the earlier posture historical rather than the dominant current state.

**What would a failure look like?**

Treating the earlier procedural state as permanently current after the matter has materially changed.

### L08 — A matter changes, then returns

**Legal · Reversal**

**Situation**

A legal matter begins in a stable procedural posture.

**What changes?**

A later event temporarily changes the posture, and subsequent information shows that the matter has returned toward its earlier posture.

**What is changing?**

The matter passes through an intermediate procedural state and then moves back toward the prior state.

**What should intelligence recognize?**

The intermediate state should be recognized as part of the trajectory without being treated as the permanent current posture after restoration.

**What would a failure look like?**

Freezing the interpretation at the intermediate state.

### L09 — Conflicting evidence does not mean one document wins

**Legal · Conflicting signals**

**Situation**

A legal intelligence system has a stable working interpretation based on the available record.

**What changes?**

A new document points in one direction while the broader record remains consistent with the earlier interpretation. Additional information remains mixed rather than resolving the conflict.

**What is changing?**

The evidentiary picture contains signals that do not fully agree.

**What should intelligence recognize?**

The new document should be weighed against the broader record, with uncertainty preserved while the conflict remains unresolved.

**What would a failure look like?**

Treating one new document as conclusive regardless of the remaining evidence.

### L10 — New evidence appears, but its relevance is unclear

**Legal · Weak new evidence**

**Situation**

A legal matter is supported by a substantial historical record.

**What changes?**

A new document contains language that could qualify the earlier interpretation, but the scope and relevance of that language are unclear.

**What is changing?**

Potentially relevant evidence has appeared, but the current state has not been definitively re-established.

**What should intelligence recognize?**

The new document may justify reduced confidence or further review without being treated as a settled change in the matter.

**What would a failure look like?**

Treating ambiguous evidence as either completely irrelevant or fully dispositive.

### L11 — The objective changes before behavior does

**Legal · Lagged context**

**Situation**

A person works with legal intelligence around one defined objective.

**What changes?**

The person’s objective changes materially, but the next interaction still partly reflects the earlier objective. Later interactions increasingly reflect the new objective.

**What is changing?**

The person’s current goal is changing while observed behavior is still in transition.

**What should intelligence recognize?**

The changed objective should become current context, while the mixed transition period remains evidence of an evolving state rather than a clean switch at one instant.

**What would a failure look like?**

Treating the old objective as permanently current, or assuming an immediate complete transition from the first new statement.

### L12 — The interaction can change what happens next

**Legal · Feedback loop**

**Situation**

A person repeatedly interacts with a legal intelligence system in a stable pattern.

**What changes?**

The system interaction is followed by a meaningful change in the person’s subsequent questions and follow-through. The change persists, but other influences may also be present.

**What is changing?**

The sequence of interaction and later behavior may contain a feedback effect.

**What should intelligence recognize?**

The interaction sequence should inform current interpretation while causal attribution remains uncertain.

**What would a failure look like?**

Ignoring the sequence or stating that the system definitely caused the later behavior.

### L13 — An administrative anomaly should not change the substance

**Legal · Transient anomaly control**

**Situation**

The substantive facts and objective of a legal matter remain stable.

**What changes?**

One administrative interaction is unusual, but later substantive interactions return to the prior pattern and the underlying matter has not changed.

**What is changing?**

An unusual administrative observation occurred without a durable substantive transition.

**What should intelligence recognize?**

The administrative anomaly should not create a durable change in the substantive interpretation of the matter.

**What would a failure look like?**

Treating a temporary administrative anomaly as evidence that the substantive matter has changed.

## Finance

### F07 — Financial behavior changes and stays changed

**Finance · Sustained change**

**Situation**

A financial intelligence system has a long history of observations about a person’s stable constraints and interaction pattern.

**What changes?**

Relevant financial constraints change materially, and subsequent behavior continues to reflect the new constraints.

**What is changing?**

The person’s current financial behavior is now being observed under a materially different set of constraints.

**What should intelligence recognize?**

Recent persistent behavior under the changed constraints should become more representative of the current state than older observations.

**What would a failure look like?**

Treating the historical profile as permanently representative after the person’s constraints have changed.

### F08 — Financial behavior changes, then returns

**Finance · Reversal**

**Situation**

A person consistently interacts with financial intelligence around one objective.

**What changes?**

The person shifts to a different objective, but after several interactions their behavior returns toward the original objective.

**What is changing?**

The person moves through a different objective state and then changes direction again.

**What should intelligence recognize?**

The latest sustained pattern should determine the current interpretation while the earlier objective remains relevant historical context.

**What would a failure look like?**

Treating the first changed objective as permanently current even after behavior returns toward the original goal.

### F09 — What a person says and what they do may diverge

**Finance · Conflicting signals**

**Situation**

A person has a stable observed interaction pattern with a financial intelligence service.

**What changes?**

The person states a new financial preference, while observed behavior remains consistent with the earlier pattern. Later behavior shows only a partial movement toward the new preference and is not yet persistent.

**What is changing?**

Stated preference and observed behavior provide different, partially conflicting evidence about the person’s current objective.

**What should intelligence recognize?**

Intelligence should weight the conflicting evidence rather than allowing either the stated preference or one behavioral observation to dominate without support.

**What would a failure look like?**

Treating the new preference or one observation as conclusive evidence of a permanent change.

### F10 — New external information appears, but its relevance is unclear

**Finance · Weak new evidence**

**Situation**

A person’s financial objective and interaction pattern have remained stable for an extended period.

**What changes?**

An external information update appears that could affect the person’s context, but its relevance to the person’s current objective is unclear and there is no corresponding behavioral change yet.

**What is changing?**

New external information has appeared without established relevance to the person’s current state.

**What should intelligence recognize?**

The update should be considered, but it should not override stable relationship evidence without demonstrated relevance.

**What would a failure look like?**

Treating external novelty as sufficient evidence of a user-state change.

### F11 — The situation changes before behavior does

**Finance · Lagged context**

**Situation**

A person has a stable financial interaction pattern under known circumstances.

**What changes?**

A materially relevant circumstance changes, but the next observed interaction remains close to baseline. Later behavior begins to diverge.

**What is changing?**

The person’s context changes before the behavioral pattern fully reflects that change.

**What should intelligence recognize?**

The relevant context change should be recognized before full behavioral confirmation, while causal certainty about its effect remains limited.

**What would a failure look like?**

Ignoring the context until behavior changes or claiming immediate certainty about its effect.

### F12 — The interaction can change what happens next

**Finance · Feedback loop**

**Situation**

A person regularly uses a financial intelligence service as part of an ongoing decision process.

**What changes?**

After repeated interactions, later behavior changes materially and persists. The change could reflect the interaction, external conditions, or both.

**What is changing?**

The interaction history may be one of the factors shaping the later financial behavior.

**What should intelligence recognize?**

Interaction history should inform the current state while causal attribution remains uncertain.

**What would a failure look like?**

Treating the interaction history as irrelevant or inferring a definitive causal effect.

### F13 — Something unusual happens — then reality returns to normal

**Finance · Transient anomaly control**

**Situation**

A person’s financial objective and observed interaction pattern remain stable over time.

**What changes?**

One interaction contains an unusual pattern, but the next interaction returns to the earlier behavior.

**What is changing?**

A noisy observation occurs without evidence of a lasting change in the person’s financial state.

**What should intelligence recognize?**

The transient anomaly should not become a persistent state representation.

**What would a failure look like?**

Over-updating the person’s state based on a single noisy observation.

## Fleet Operations

### O07 — Fleet behavior changes and stays changed

**Fleet Operations · Sustained change**

**Situation**

An operational intelligence system observes a fleet asset under a stable operating pattern.

**What changes?**

The asset’s operating pattern changes materially and the new pattern persists across subsequent observations.

**What is changing?**

The asset is now operating under a different persistent state than the historical baseline.

**What should intelligence recognize?**

Persistent current operating behavior should become more representative than the older operating pattern.

**What would a failure look like?**

Treating historical operating regularity as permanently representative after the asset’s operating state has changed.

### O08 — Fleet behavior changes, then returns

**Fleet Operations · Reversal**

**Situation**

A fleet asset operates in a stable pattern.

**What changes?**

A temporary operational deviation occurs, followed by a return to approximately the earlier operating pattern.

**What is changing?**

The asset passes through an anomalous operating state and then returns toward baseline.

**What should intelligence recognize?**

The current state should reflect the recovery rather than treating the temporary deviation as a permanent operating transition.

**What would a failure look like?**

Freezing the fleet asset’s state at the intermediate anomaly.

### O09 — Operational signals do not fully agree

**Fleet Operations · Conflicting signals**

**Situation**

A fleet asset shows a stable operational pattern across several relevant signals.

**What changes?**

One signal suggests deterioration while several other relevant signals remain near the historical pattern. The next observations remain mixed rather than confirming a clear transition.

**What is changing?**

Different operational signals provide conflicting evidence about the asset’s current condition.

**What should intelligence recognize?**

Conflicting signals should be weighted according to their relevance and corroboration rather than converting one adverse signal into a definitive state change.

**What would a failure look like?**

Allowing one signal to dominate regardless of the rest of the operational evidence.

### O10 — New environmental information appears, but its relevance is unclear

**Fleet Operations · Weak new evidence**

**Situation**

A fleet asset operates under a stable relevant environment.

**What changes?**

An environmental detail changes, but its operational relevance to the asset’s current state is uncertain and relevant operating observations remain stable.

**What is changing?**

New environmental information has appeared without established material impact on the asset’s operating state.

**What should intelligence recognize?**

Environmental novelty should not override stable relevant observations without evidence of material operational impact.

**What would a failure look like?**

Treating every environmental change as operationally decisive.

### O11 — Operating conditions change before behavior does

**Fleet Operations · Lagged context**

**Situation**

A fleet asset operates under a stable set of relevant conditions.

**What changes?**

Relevant operating conditions change materially, but the next observation still resembles the historical pattern. Subsequent observations begin to diverge.

**What is changing?**

The asset’s operating context changes before the observed operating behavior fully reflects it.

**What should intelligence recognize?**

The changed context should be recognized before full behavioral confirmation, while avoiding unsupported certainty about causation.

**What would a failure look like?**

Ignoring changed operating context until output behavior changes or assuming immediate causal certainty.

### O12 — The operational decision can change what happens next

**Fleet Operations · Feedback loop**

**Situation**

An operational decision is made using the information available at the time.

**What changes?**

The decision changes subsequent operating conditions, and later observations occur within that changed environment. Other contributing factors may also be present.

**What is changing?**

The later operating state is partly observed under conditions that were changed by the preceding action.

**What should intelligence recognize?**

The later state should be interpreted in the changed environment created after the action while preserving uncertainty about other contributing factors.

**What would a failure look like?**

Ignoring the preceding action or claiming it was the sole cause of the later operating state.

### O13 — Something unusual happens outside the relevant context

**Fleet Operations · Transient anomaly control**

**Situation**

Relevant operating conditions and observations for a fleet asset are stable.

**What changes?**

One environmental detail outside the relevant operating context changes, while the observations that matter to the asset’s operation remain stable.

**What is changing?**

An environmental anomaly occurs without a corresponding change in the relevant operating state.

**What should intelligence recognize?**

The environmental anomaly should not produce a state transition when relevant operational evidence remains stable.

**What would a failure look like?**

Treating irrelevant environmental novelty as an operational state change.

## What these 28 cases test

Across the four domains, the cases cover seven recurring patterns:

1. **Behavior changes and stays changed** — Persistent recent evidence can become more representative than a long historical record.
2. **Behavior changes, then returns** — A temporary change should not automatically become a permanent state.
3. **Conflicting signals** — Different forms of evidence can disagree and should not be forced into premature certainty.
4. **New information appears, but its relevance is unclear** — Novelty or plausibility alone should not override stronger evidence.
5. **The situation changes before behavior does** — Context can change before its effects become visible in behavior.
6. **The interaction can change what happens next** — An interaction or decision may become part of the evolving situation while causal attribution remains uncertain.
7. **Something unusual happens — then reality returns to normal** — A transient anomaly should not be converted into a durable state change.

The purpose is not simply to detect change. It is to evaluate whether intelligence can **change its interpretation when the evidence warrants it, preserve uncertainty when it does not, and remain stable when apparent change is only noise.**

The public scoring framework is available in [`benchmark/RUBRIC.md`](benchmark/RUBRIC.md).

These are controlled research scenarios designed to test observable behavior. They do not disclose the mechanism used by any private system.
