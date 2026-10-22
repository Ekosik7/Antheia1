# Recommendation design

Status: proposed simple baseline; no ML or ranking code is implemented.

## Inputs and precedence

Inputs: explicit preferences, occasion, budget/currency, closet items, attributed product data and optional user-reviewed image-derived colors. Explicit dislikes and corrections take precedence over inferred palettes. Photo-free users retain the full outfit-discovery flow.

## Planned stages

1. Validate request; preserve editable occasion, sizes, region and budget.
2. Retrieve candidates from closet and a named catalog snapshot. Hard-filter disliked colors, known size/region mismatches and unavailable variants. Unknown size/stock is not a confirmed match.
3. Compose outfits with compatible category roles. Provisional templates include top + bottom + shoes or dress + shoes; validate these with users rather than defining all fashion outfits this way.
4. Score style match, color compatibility, occasion match and explicit preference match; rank eligible combinations and return Top-K distinct outfits.
5. Recheck outfit-level constraints before display. Explain actual matches and limitations; provide an honest empty state when nothing qualifies.

Conceptual score = w_style × StyleMatch + w_color × ColorMatch + w_occasion × OccasionMatch + w_preference × PreferenceMatch.

Weights, normalization, signal definitions and K remain undecided. Missing signals need a documented omission/reweighting policy. Optional image colors are a supporting feature, not an automatic seasonal veto.

## Hard constraints and prices

Individual price ≤ budget is only early pruning. Final eligibility requires **sum of new purchase offer prices ≤ strict budget**, in one declared currency. Owned pieces have no new purchase charge and are labelled owned; unknown purchase prices cannot count as zero. Do not guess exchange rates. Shipping/tax remain explicitly unknown or excluded when unavailable.

Source example: KZT 18,000 + 15,000 + 20,000 = KZT 53,000; reject under a KZT 50,000 cap. Constraint compliance is separate from subjective relevance.

## Future evaluation

Compare preferences-only, preferences + compatibility and the same baseline + optional corrected palette on fixed candidates. Measure hard rules independently of user ratings. Feedback learning, fit accuracy and photo benefit require evidence before any claims.