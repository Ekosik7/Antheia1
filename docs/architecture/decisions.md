# Architecture decision log

All decisions are proposed from the current task; team/supervisor review remains pending.

| ID | Decision | Reason / consequence |
| --- | --- | --- |
| ADR-01 | One Go application backend with modular ranking | Small MVP with separately testable retrieval, compatibility and ranking |
| ADR-02 | React client and PostgreSQL structured data | Requested stack; contracts/schema remain future work |
| ADR-03 | Optional private Python image service | Isolates image experiments and permits photo-free operation |
| ADR-04 | Start with deterministic filtering/scoring | No interaction history or demonstrated need for advanced ML |
| ADR-05 | Approved, attributed versioned catalog snapshots | Live access and freshness are unverified |
| ADR-06 | Plan Docker Compose | Small local topology; runtime files deferred |
| ADR-07 | Preserve baseline and document scope delta | Keeps source provenance while adding closet features |

Open: guest/account lifetime, image retention/deletion policy, catalog permissions and two-source pilot, scoring weights, image limits, test hardware, budget UX, approval and actual YouTrack URL.