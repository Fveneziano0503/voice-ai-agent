# Manual test plan

These are acceptance scenarios, not claimed test results. Run in a private, authorized test environment.

| Scenario | Expected behavior |
|---|---|
| Browser test | Conversation begins; no phone identity invented |
| Beginner asks about AI | Short plain-language explanation |
| Person interrupts | Assistant stops and listens |
| Receptionist offers transfer | Routing noted; no completed transfer claimed without confirmation |
| Prospect states a challenge | Record captures only stated challenge |
| Product mentioned without interest | Presented product not marked as interested |
| Requests email | Explicit permission recorded; no sending claimed |
| Requests meeting with no booking tool | Meeting requested, not confirmed |
| Declines | Respectful ending |
| Opt-out | Explicit flag and no further pitch |
| Missing information | Optional fields absent |
| Hostile response | Calm ending |

Measure interruption latency, extraction accuracy, incorrect action claims, and opt-out handling across annotated test calls. Establish a baseline before reporting improvements.
