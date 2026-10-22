# Proposed architecture

Status: documentation only. The original `ANTHEIA_Architecture_and_3_Diagrams.docx` is retained unchanged in this folder. The following stack mapping is a new proposal.

React Frontend → Go Backend → PostgreSQL.

Go Backend → optional Python AI Service for consented image quality and tentative palette estimation.

Go contains preference/profile, closet, request validation, catalog adapters, candidate retrieval, outfit composition, scoring/ranking, final hard-constraint validation and feedback modules. Recommendation Engine is a logical Go module, not another deployed service. Permitted catalog feeds/snapshots supply products; external retailer websites handle checkout.

## Planned journeys

1. Manual: Style DNA → My Closet / Add Item if desired → occasion/budget → closet/catalog retrieval → compose outfits → rank → final validation → explanations → My Shop comparison / retailer link.
2. Optional photo: consent → validate/private temporary processing → Python quality/palette estimate → user correction → optional ranking signal. Failure preserves manual recommendations.
3. Catalog: authorized import → source permission/provenance check → normalized variants/offers → immutable snapshot → retrieval. No live feed or merchant agreement is assumed.

## Storage and failure boundaries

PostgreSQL is planned for structured data. Photo bytes require a private temporary storage decision; do not assume public files or database blobs. The client talks only to Go; Python and PostgreSQL remain private. Missing catalog data cause explicit limitations, not invented offers. Image-service failure affects optional assistance only.

[Decisions](decisions.md), [data model](data-model.md), [contracts](contracts.md), [privacy](privacy-and-data.md), [ranking](recommendation-logic.md) and [diagrams](../diagrams/README.md).