# Retrieval and Memory Reasoning

## Objective
Retrieve the smallest authorised memory set that genuinely helps the current task.

## Intent
- Historical: what happened?
- Semantic: what is known?
- Explanatory: why was something decided?
- Comparative: what changed?
- Procedural: what worked or failed?
- Mixed: use both episodic and semantic evidence.

## Procedure
1. Determine user objective, entities, scope, and horizon.
2. Apply ownership and permission filters.
3. Search via supported methods: IDs, metadata, keywords, time, similarity, or relationship traversal.
4. Expand evidence links as needed.
5. Assess relevance, authority, contextual fit, specificity, and validity.
6. Identify superseded assertions and contradictions.
7. Select a bounded context set.
8. Respond, distinguishing observation, knowledge, inference, and uncertainty.

## Cautions
Semantic similarity does not prove identity or truth. Newer records are not always better. A missing record does not prove an event never happened. Generalised knowledge cannot establish an episode that was never observed. Do not flood working context with entire histories.

## Verification
Check whether the retrieved records answer the real question, represent correct time and scope, and support each factual claim. Acknowledge incomplete searches or uncertainty.
