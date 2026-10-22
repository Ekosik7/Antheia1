# Scope alignment and proposed additions

Status: proposed interpretation of the current task. Originals remain unchanged; supervisor approval is pending.

| Area | Supplied baseline | Current design interpretation |
| --- | --- | --- |
| Topic | Earlier titles use styling / image-personalization variants | Use the full topic from the task in new documents; retain original titles in originals |
| Technology | Logical, technology-agnostic architecture | React client, Go application modules, PostgreSQL structured records, Python optional image service |
| Wardrobe | Focus includes catalog-based outfit discovery | Add explicit My Closet and Add Item requirements below |
| AI Stylist | FR-11 includes natural-language input | Structured filters are the initial baseline; prompt interpretation remains planned with editable confirmation, no assumed LLM |
| Accounts | FR-01 guest path; FR-02/10 conditional accounts | Guest flow remains required; cross-session persistence awaits a storage/account decision |
| Catalogs/admin | FR-14/17/29 permitted sources and restricted management | Retain two-source pilot target; when only source-shaped fixtures are feasible, disclose the real-data gap; no public admin UI is assumed |
| Photo | FR-05–09 require safeguards when processing is offered | User photo use stays optional; safeguards are required if enabled |
| Budget | FR-22–24 require source-offer subtotal | Separate new purchase subtotal from owned pieces; unknown purchase prices cannot count as zero |

## Proposed requirements awaiting formal identifiers

Local P- labels are documentation references, not replacements for official FR or UC identifiers.

| Local label | Proposed behavior | Future acceptance check |
| --- | --- | --- |
| P-CLOSET-01 | List/edit/remove owned garments in My Closet | Add makes the item visible; edit affects later candidates; deletion removes it from future selections |
| P-CLOSET-02 | Add Item supports manual category, color and optional size/style | Valid manual entry works without an image; unknown optional values stay unknown |
| P-CLOSET-03 | Distinguish owned garments from new offers | Owned labels are visible; only selected purchase offers enter the purchase subtotal |
| P-CLOSET-04 | Scope private closet data to the user/guest context | Another context cannot read or edit items; guest lifetime is documented |

Provenance, strict budgets, deletion, explicit preference precedence, unknown-data states and external checkout remain intact. Prototype assets, retention, catalog permissions, scoring weights and final sign-off remain open.