# Temporal Reasoning and Memory Conflicts

## Four temporal dimensions
- Event time: when something occurred.
- Observation time: when the agent learned about it.
- Valid time: when an assertion applied in the world.
- Update time: when a memory record changed.

Never substitute one for another. Use bounded uncertainty if exact time is unknown.

## Conflict detection
Claims genuinely contradict only where meaning, subject, scope, and valid time overlap. “Used SQLite in January” and “uses PostgreSQL in April” may both be true.

## Resolution
1. Parse both claims precisely.
2. Resolve entities without unwarranted conflation.
3. Compare project and contextual scope.
4. Compare event, observation, and validity periods.
5. Assess source authority and independence.
6. Determine whether circumstances changed or an earlier record was wrong.
7. Resolve only if warranted; otherwise mark disputed.
8. Link new knowledge to superseded records and retain justified history.

## Correction versus change
A correction establishes that an earlier assertion was inaccurate. A change establishes that an earlier assertion applied then but not now. These require different historical treatments.

## Example
A March decision chooses architecture A; a June decision switches to architecture B. The current semantic state is B, while historical episode retrieval still answers that A was selected in March.
