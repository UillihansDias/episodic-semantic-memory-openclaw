# Memory Architecture

## Actual OpenClaw target
The inspected runtime offers memory search, bounded exact-path memory excerpts, sanitised session search/history, and authorised workspace file editing. No general-purpose memory record write API was found. The canonical stores are `USER.md` (stable user directives with observed/status metadata), `MEMORY.md` (durable facts/decisions), and `memory/YYYY-MM-DD.md` (dated notes). Apply the host workspace policy, which takes precedence. Logical records below describe reasoning only, not files or database tables that must be created.

## Logical layers
1. Intake: conversations, actions, tools, documents, observations.
2. Classification: relevance, entity identity, time, privacy, memory type.
3. Storage: episodic events, semantic assertions, relationships, lifecycle metadata.
4. Maintenance: deduplication, consolidation, validation, supersession, retention.
5. Retrieval: scoped search, ranking, reconciliation, evidence-aware application.

These are logical stages, not necessarily separate services.

## Memory categories
- Episodic: meaningful occurrences, historically contextualised.
- Semantic: reusable assertions, relations, preferences, concepts, and procedures.
- Working context: transient task information, not automatically persisted.
- External authoritative data: maintained by another system and rechecked for freshness.

## Lifecycle
Candidate → Classified → Validated → Persisted → Active → Disputed / Superseded / Expired / Invalid → Archived or Deleted.

Rejected candidates should not persist merely to preserve the fact of rejection.

## Identity and provenance
Use stable identifiers for records, entities, sources, and workspaces. Do not conflate similarly named entities. Provenance includes origin, source reference, speaker if relevant, observation time, and evidence type. Honor access controls on all source links.

## Storage options
Relational, document, graph, or indexed-file storage may be used. Embeddings and search indexes are optional derived views; they are not an authoritative source of truth. Use atomic or idempotent writes when supported; detect partial writes and index inconsistency.

## Storage discovery
Establish available storage APIs, read/write permissions, guarantees, limits, and retention policies before taking action. Do not invent tools or capabilities.
