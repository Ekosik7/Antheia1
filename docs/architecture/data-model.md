# Logical data model

Conceptual design only: no SQL, migrations or database schema exists.

| Entity | Proposed responsibility / relationship |
| --- | --- |
| User / GuestContext | Owns private profile/closet; guest lifetime undecided |
| PreferenceProfile | Styles, colors, dislikes, sizes, region; explicit choices separate from inference |
| ClosetItem | Owner/context, category, colors, optional size/style and private image reference |
| Product / ProductVariant | Product metadata with distinct color/size variants |
| RetailerOffer | Source, variant, URL, price/currency, stock state and as-of metadata |
| CatalogSnapshot | Immutable source/version/permission metadata for evaluation |
| RecommendationRequest | Context, preferences, occasion, constraints and snapshot |
| Outfit / OutfitItem | Roles referencing owned items or specific offers |
| SavedOutfit / Feedback | Conditional scoped persistence, no trained adaptation implied |
| PhotoArtifact / Consent | Private opaque reference, purpose, expiry/deletion state and consent |

Products can have multiple variants/offers. An owner can have multiple closet items. Outfits may mix owned items and purchases; preserve this distinction for price computation. Identifiers, constraints and ERD need later review. [ERD placeholder](../diagrams/erd/README.md).