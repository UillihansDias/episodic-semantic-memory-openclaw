# Episodic Memory

## Definition
An episodic memory is a meaningful occurrence within a particular temporal and contextual setting. It preserves experience rather than general truth.

## Capture
Record what happened, when (or temporal uncertainty), actors, relevant scope/context, result, and source. Distinguish event time from observation time. Do not invent missing details.

## Granularity
Prefer one meaningful event per record. Split sequences when individual steps matter independently, and group low-level events when the useful memory is their aggregate outcome. Avoid copying exhaustive logs into episodic memory.

## Categories
Decision, action, observation, interaction, milestone, failure, correction, discovery, and outcome are useful optional tags.

## Causality
Separate sequence, stated cause, observed cause, and hypothesised cause. Chronological proximity alone is not causal evidence.

## Deduplication
Merge equivalent descriptions only when they refer to the same event; similar episodes occurring on different dates remain distinct.

## Retrieval
Use chronological episode retrieval for historical questions, decision reconstruction, previous attempts, outcome analysis, and project evolution.

## Example
A deployment returns a missing-configuration error. Record the attempted deployment and observed failure. Do not conclude that the entire deployment platform is unreliable.
