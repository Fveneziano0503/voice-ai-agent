# Voice AI Agent — Victoria — Business Voice Assistant

A portfolio case study of a conversational business assistant that introduces the business, listens to questions, routes through receptionists, qualifies business needs, and structures call information for human review.

**Created by Federico Veneziano · Project #3**

## Business problem
Routine business conversations can consume time while leaving inconsistent notes, unclear follow-up expectations, and missed handoffs. This project explores a repeatable voice workflow with concise conversation and factual records.

## What I designed
- A short introduction followed by questions appropriate to the person's AI familiarity.
- Receptionist routing, interruption handling, and respectful call endings.
- Separation of products presented from products the prospect actually asks about.
- Structured records for outcomes, objections, contact details, and explicit follow-up preferences.
- Human review before downstream action; proposed meetings remain unbooked until a scheduling tool succeeds.

## Implementation status
| Component | Status |
|---|---|
| Vapi browser voice test | Completed in private development; reported by the builder |
| Conversation behavior | Designed; public prompt example included |
| Post-call structured output | Existing private setup documented; public schema included |
| Public portfolio interface | Runnable local demo with synthetic data |
| Telephone campaigns / live transfers | Not demonstrated in this repository |
| CRM sync, scheduling, automatic suppression | Future integrations; not implemented here |

This is a **sanitized case study and configuration starter**, not a production calling service. No performance improvement or conversion rate is claimed. Production credentials, recordings, phone numbers, and customer records are excluded.

## View the demo
Download or clone this repository and open `demo/index.html` in a browser. Select the six workflow views. The interface is illustrative and does not connect to a live voice service.

## Portfolio screenshots
All six are **illustrative workflow visuals rendered from synthetic demo content**, not live application or Vapi dashboard screenshots. The same six views are available in the included HTML demo.

### Agent overview
![Agent overview](screenshots/01-agent-overview.png)

### Conversation flow
![Conversation flow](screenshots/02-conversation-flow.png)

### Receptionist routing
![Receptionist routing](screenshots/03-receptionist-routing.png)

### Lead qualification
![Lead qualification](screenshots/04-lead-qualification.png)

### Structured call record
![Structured call record](screenshots/05-structured-call-record.png)

### Follow-up review
![Follow-up review](screenshots/06-follow-up-review.png)

## Architecture
```mermaid
flowchart TD
    A[Browser voice test] --> B[Vapi conversation runtime]
    B --> C[Victoria prompt]
    C --> D{Conversation outcome}
    D --> E[Routing or qualification]
    D --> F[Polite exit or opt-out]
    E --> G[Post-call structured extraction]
    F --> G
    G --> H[Human review]
    H -. Planned .-> I[CRM or scheduling integration]
```

## Repository guide
- `prompts/victoria-system-prompt.md`: public conversation prompt.
- `config/call-record.schema.json`: JSON Schema for post-call records.
- `examples/synthetic-call-record.json`: clearly synthetic example.
- `docs/architecture.md`: implementation boundaries and design decisions.
- `docs/test-plan.md`: reproducible test scenarios; no fabricated pass results.
- `docs/setup.md`: manual configuration checklist.
- `docs/case-study.md`: problem, approach, lessons, and measurement plan.

## Skills demonstrated
Applied AI workflow design · conversational UX · prompt engineering · structured information capture · business process design · human review and escalation.
