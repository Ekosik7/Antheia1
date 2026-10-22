# ANTHEIA

An intelligent personal styling and fashion recommendation system.

**Diploma topic:** Development of an Intelligent Recommendation System for Personal Image and Style Personalization Based on Image Analysis and User Preferences.

## Current status

This project contains the folder structure, supplied research and requirements, proposed architecture, and placeholders for future implementation. No application code, trained model, database migrations, executable workflows or deployed services exist. System performance and usefulness have not been measured. Git has not been initialized.

## Problem and goal

Coordinating clothes, reusing a wardrobe and finding relevant products within a budget can take time. ANTHEIA aims to combine explicit preferences, personal closet items, product data and optional image-derived color signals into explainable complete outfits. The supplied four-interview study provides preliminary qualitative evidence; it does not establish population-wide demand or proven effectiveness.

Target users are people seeking everyday or occasion-based styling, wardrobe reuse and transparent shopping alternatives, including users who decline photographs or registration.

## Proposed MVP and features

- **Style DNA:** editable styles, preferred/disliked colors, sizes and region.
- **My Closet:** list, edit and remove personally owned garments.
- **Add Item:** manual garment entry with an optional item image.
- **AI Stylist:** occasion/budget requests, filtering, compatibility scoring and Top-K outfit ranking. This name does not imply an implemented generative model.
- **Recommendation Results:** outfit roles, explanations, owned/purchase labels, prices and purchase subtotals.
- **My Shop:** product discovery, Product / Price comparison and attributable external retailer links.
- **Optional Photo Analysis:** consented image-quality checks and tentative, editable palette suggestions with uncertainty.
- Save/rate recommendations and cross-session account persistence are conditional planned features; adaptive learning is unproven.

The full recommendation journey must work without a portrait. Virtual try-on, exact body measurements, fit prediction, internal checkout and unrestricted live store scraping are outside the MVP.

## Planned stack

| Layer | Technology | Responsibility |
| --- | --- | --- |
| Frontend | React | User interactions and screens |
| Backend | Go | API, profiles, closet, catalogs and ranking modules |
| Database | PostgreSQL | Structured records |
| Optional image service | Python | Quality checks and tentative palette signals |
| Deployment | Docker / Docker Compose | Future service packaging |

Libraries and versions have not been selected. Recommendation Engine is a logical module in Go, not another deployed service.

## Folder structure

```text
Antheia/
  .github/workflows/  Future CI placeholder
  backend/           Go service skeleton
  frontend/          React client skeleton
  ai-service/        Optional Python image service skeleton
  docs/              Academic sources, requirements, design and evaluation plans
  docs-for-us/       Team navigation and handoff notes
  infra/             Deployment planning
  .env.example       Proposed configuration names only
  .gitignore         Future Git exclusions
```

## Documentation

- [Documentation index](docs/README.md) and [source provenance](docs/source-register.md)
- [Requirements](docs/requirements/README.md) and [scope alignment](docs/requirements/scope-alignment.md)
- [Architecture](docs/architecture/overview.md), [ranking](docs/architecture/recommendation-logic.md) and [diagrams](docs/diagrams/README.md)
- [UX](docs/ux/README.md) and [verification plan](docs/verification/plan.md)
- [Work plan](docs/project-management/work-plan.md), [risks](docs/project-management/risks.md) and [supervisor feedback template](docs/project-management/supervisor-feedback.md)
- [Team handbook](docs-for-us/README.md)
- [Complete folder tree, file inventory and packaging checks](docs/project-management/deliverables.md)

## Setup

Not yet implemented. There are no dependency manifests, entrypoints, migrations, Dockerfiles or Compose configuration. There is no application build or launch command. Service READMEs describe future responsibilities. `.env.example` documents proposed names only; no service reads it yet.

## Team and coordination

| Role | Verified name |
| --- | --- |
| Team member 1 | [To be supplied] |
| Team member 2 | [To be supplied] |
| Additional members | [To be supplied if applicable] |
| Supervisor | [To be supplied] |

YouTrack project: [URL to be supplied]. No tracker tasks, authorship history or supervisor approvals are claimed. [Suggested future commit plan](docs/project-management/suggested-commits.md).
