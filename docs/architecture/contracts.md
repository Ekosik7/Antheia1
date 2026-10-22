# Planned service contracts

Interface notes only, not implemented endpoints or a completed OpenAPI specification. Original architecture paths are illustrative.

| Interaction | Proposed input | Proposed output |
| --- | --- | --- |
| Client → Go preferences/closet | Scoped user/guest context; explicit fields/item edits | Validated state or field errors |
| Client → Go style request | Occasion, sizes/region, budget/currency, optional prompt | Editable interpreted filters; ambiguity feedback |
| Client → Go recommendations | Context, filters, snapshot, optional corrected palette | Outfits, owned/purchase labels, subtotal, reasons, timestamps/warnings |
| Go → Python palette estimate | Validated consented image/private handle | Quality flags, tentative colors, optional season, uncertainty |
| Client → Go photo deletion | Scoped artifact reference | Confirmed deletion or explicit failure |
| Authorized import → Go catalog | Approved records and source/schema version | Snapshot or rejected-record report |

Source example paths include `POST /style-requests`, `POST /palette-estimates`, `POST /recommendations`; none are available now. Closet API naming is undecided.

Go must validate context, consent and constraints server-side. A browser-supplied palette is not evidence of image consent. Image failure returns a recoverable limitation through Go. Never include portrait bytes or credentials in recommendation payloads, or guess stock/prices. Authentication, timeouts, error format and versioning need specification later.