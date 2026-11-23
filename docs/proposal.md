# CircuitSide proposal

**Course:** CSC 4360 Mobile App Development  
**Topic:** TropicaGuide Travel Planner  
**Milestones:** Proposal November 22, 2026. Final application December 13, 2026.

CircuitSide helps Formula 1 travelers plan and share a race weekend. The group starts with fixed race sessions, fits local activities around them, tracks estimated spend in one currency, and assigns packing and checklist tasks. The initial release targets Android with labeled demo race schedules and no payments.

## Functional scope

| Workflow | Acceptance target |
| --- | --- |
| Auth and profiles | Verify sign-in, persistence, profile isolation, and expired or repeated invitations. |
| Trip and itinerary | Persist trip and activity changes, validate dates and costs, and prevent overlap around fixed sessions. |
| Discovery | Filter by location, budget and category. Explain missing results, closed venues, stale data and provider failures. |
| Collaboration | Synchronize two accounts and enforce owner, editor and viewer access. |
| Reusable checklists | Copy a template, assign tasks, and reset or restore a checklist without affecting its source. |
| Packing | Prevent normalized duplicate names and make completion retries idempotent. |
| Recommendations | Return explainable suggestions and preview before saving. Compare with a time-and-budget baseline on 12 fixed cases. |

The shared itinerary must support accessible drag-and-drop, live snapshots, nested trip documents, and versioned conflict resolution. Evidence will include linked issues and commits, emulator tests, two-device demonstrations, and review by the feature owner. The full submission packet contains the visual wireframes, complete evaluation table, and signatures.
