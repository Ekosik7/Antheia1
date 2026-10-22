# Technology comparison and selection rationale

Status: proposed engineering rationale for the requested stack. No performance/cost benchmark or library versions have been established.

| Area | Selected | Alternative | Rationale / trade-off |
| --- | --- | --- | --- |
| Client | React | Server-rendered templates | Planned interactive closet/filter flows; API/state integration required |
| Backend | Go | Python-only backend | One application service; a separate language boundary for images |
| Data | PostgreSQL | Files / SQLite | Planned relations across closet, profiles and offers; database operations required |
| Image analysis | Python service | Go image pipeline | Isolates experimentation; private contract required |
| Deployment | Docker Compose | Kubernetes | Small MVP topology; production hosting undecided |
| Ranking | Filtering and weighted scoring in Go | Collaborative / graph models | Initial baseline without interaction history; usefulness must be tested |

This is design reasoning, not benchmarked evidence. Java and Microsoft authentication from AITU_Awards are not adopted.
