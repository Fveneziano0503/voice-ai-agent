# Architecture and boundaries

The existing private experiment uses Vapi for a browser voice test and a post-call structured-output setup. The prompt defines behavior; extraction converts a completed conversation into a record. A record is evidence for review, not proof that a downstream action occurred.

The public HTML is a separate presentation layer. It simulates six workflow views with static synthetic data and does not implement Vapi connectivity. The JSON Schema is a reduced public example, rather than the complete private configuration.

Planned integrations require authenticated tools, error handling, durable event identifiers, deduplication, and an auditable action result. Explicit opt-outs should block further outreach before another call is queued. Do not equate extracting an opt-out with suppressing it in a real system.
