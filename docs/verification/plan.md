# Verification and evaluation plan

Status: future plan only. No application tests, user study, benchmark or model evaluation has run. Retain AT-01–AT-13 and NFR identifiers from the source requirements; none are passed.

| Area | Planned check | Evidence to record |
| --- | --- | --- |
| Photo-free | AT-01: preferences to results/empty-state without photo/account | Inputs, outputs and UI evidence |
| Privacy | AT-02/03/04/10: consent, uncertainty, correction, deletion | Artifact/access/deletion observations |
| Prices | AT-05/06: exact sum, cap boundaries, currency, unknown fees | Offers and expected arithmetic |
| Catalog | AT-07/08/09/11: variants, sources, empty/degraded states | Snapshot/source IDs, timestamps, real-data gaps |
| Authorization | AT-12: profile/closet isolation and restricted admin | Rejected unauthorized requests |
| Closet | P-CLOSET-01–04: CRUD, manual entry, owned costs, isolation | Before/after candidate selection and scope checks |
| Relevance | AT-13: preferences vs compatibility vs optional palette | Independent ratings and candidate definitions |
| Usability | Style DNA, Add Item, stylist and comparison tasks | Completion, difficulties and consented feedback |
| Accessibility | Keyboard labels, contrast and planned viewport widths | Later audit evidence |
| Performance | Replay defined requests, isolate photo latency | Hardware, samples, p50/p95 and failures |

Source targets, not results: up to 5,000 offers; recommendation p95 ≤3 seconds across at least 100 requests; accepted ≤3 MB photo p95 ≤8 seconds across at least 30 images. Confirm feasibility after baseline measurement.

Freeze catalog snapshots, candidates, scoring definitions and settings. Define recruitment, consent, data splits and rating rubric before collection. Keep tuning feedback separate from independent assessment. Ranking metrics require explicit relevance labels and candidate definitions. Repeat-photo and lighting tests measure a different property from outfit usefulness.

[Results template](results-template.md) stays blank. Packaging checks on documentation do not constitute passing application acceptance tests.