# Delivery inventory

Prepared on 20 October 2026. This is a documentation scaffold, not an implemented application.

## Major folders

| Folder | Purpose |
| --- | --- |
| backend/ | Future Go service: cmd/, internal/, tests/ |
| frontend/ | Future React source in src/ |
| ai-service/ | Future optional Python image service: app/, tests/ |
| docs/ | Preserved academic materials, proposed requirements/architecture, diagrams, UX and evaluation plans |
| docs-for-us/ | Team navigation to canonical documentation and future working notes |
| infra/ | Deployment planning only |
| .github/workflows/ | Empty placeholder for future CI |

## Completion status

**Prepared documentation:** root/service READMEs, organized original sources, source provenance, working proposal, technology rationale, scope alignment, architecture/contract/data/ranking/privacy notes, current diagram definitions, UX flows, verification plan, risk register, work plan and suggested commits. These are working drafts, not supervisor-approved academic conclusions.

**Placeholders:** service source/test directories; CI; ERD; visual UX prototype; presentation; supervisor feedback; evaluation results; team names, supervisor and YouTrack URL. The future note folders in docs-for-us contain navigation only.

**Future implementation:** React screens, Go API and ranking, PostgreSQL schema/migrations, Python image pipeline/models, catalog ingestion, authentication if selected, Docker/Compose and automated tests. All are absent. Manual Git initialization/publication is deferred.

**Diagram limitation:** supplied baseline drawings/exports are unchanged. New Mermaid/PlantUML definitions reflect the requested stack and closet scope; their rendering/visual review remains future work.

## Packaging checks

- All 17 supplied document/archive entries match their original SHA-256 hashes.
- No application source, package manifests, migrations, deployment files or executable CI workflows found.
- No .git directory exists; no Git commands were run.
- Seven empty .gitkeep placeholders preserve future code/test/workflow folders.
- All 96 local Markdown links were verified after generating this inventory.
- These checks do not test future application behavior or validate research findings.

## Full folder tree

```text
Antheia/
├── .github/
│   └── workflows/
│       └── .gitkeep
├── ai-service/
│   ├── app/
│   │   └── .gitkeep
│   ├── tests/
│   │   └── .gitkeep
│   └── README.md
├── backend/
│   ├── cmd/
│   │   └── .gitkeep
│   ├── internal/
│   │   └── .gitkeep
│   ├── tests/
│   │   └── .gitkeep
│   └── README.md
├── docs/
│   ├── architecture/
│   │   ├── ANTHEIA_Architecture_and_3_Diagrams.docx
│   │   ├── contracts.md
│   │   ├── data-model.md
│   │   ├── decisions.md
│   │   ├── overview.md
│   │   ├── privacy-and-data.md
│   │   └── recommendation-logic.md
│   ├── diagrams/
│   │   ├── context/
│   │   │   ├── 01_system_context.drawio
│   │   │   └── system-context.mmd
│   │   ├── erd/
│   │   │   └── README.md
│   │   ├── exports/
│   │   │   ├── 01_system_context.png
│   │   │   ├── 01_system_context.svg
│   │   │   ├── 02_use_case.png
│   │   │   ├── 02_use_case.svg
│   │   │   ├── 03_component.png
│   │   │   ├── 03_component.svg
│   │   │   └── README.md
│   │   ├── uml/
│   │   │   ├── 02_use_case.drawio
│   │   │   ├── 03_component.drawio
│   │   │   ├── components.mmd
│   │   │   └── use-cases.puml
│   │   ├── ANTHEIA_All_3_Diagrams.drawio
│   │   └── README.md
│   ├── evidence-of-relevance/
│   │   ├── Evidence_of_Relevance_Preliminary_Analysis(2).docx
│   │   └── README.md
│   ├── existing-systems/
│   │   ├── Existing_Systems_Comparison.docx
│   │   └── README.md
│   ├── literature-review/
│   │   ├── Fashion_Recommendation_Literature_Review.docx
│   │   └── README.md
│   ├── presentation/
│   │   └── README.md
│   ├── project-management/
│   │   ├── ANTHEIA_YouTrack_Requirements_Backlog.csv
│   │   ├── deliverables.md
│   │   ├── README.md
│   │   ├── risks.md
│   │   ├── suggested-commits.md
│   │   ├── supervisor-feedback.md
│   │   └── work-plan.md
│   ├── project-proposal/
│   │   └── README.md
│   ├── requirements/
│   │   ├── ANTHEIA_Requirements_Specification.docx
│   │   ├── README.md
│   │   └── scope-alignment.md
│   ├── technology-comparison/
│   │   └── README.md
│   ├── ux/
│   │   └── README.md
│   ├── verification/
│   │   ├── plan.md
│   │   └── results-template.md
│   ├── README.md
│   ├── source-package-README.txt
│   └── source-register.md
├── docs-for-us/
│   ├── architecture/
│   │   └── README.md
│   ├── diagrams/
│   │   └── README.md
│   ├── presentation/
│   │   └── README.md
│   ├── requirements/
│   │   └── README.md
│   ├── research/
│   │   └── README.md
│   ├── services/
│   │   ├── ai-service.md
│   │   ├── backend.md
│   │   └── frontend.md
│   ├── testing/
│   │   └── README.md
│   ├── ux/
│   │   └── README.md
│   ├── project-overview.md
│   └── README.md
├── frontend/
│   ├── src/
│   │   └── .gitkeep
│   └── README.md
├── infra/
│   └── README.md
├── .env.example
├── .gitignore
└── README.md
```

## All files

74 files, including this inventory.

- `.env.example`
- `.github/workflows/.gitkeep`
- `.gitignore`
- `ai-service/app/.gitkeep`
- `ai-service/README.md`
- `ai-service/tests/.gitkeep`
- `backend/cmd/.gitkeep`
- `backend/internal/.gitkeep`
- `backend/README.md`
- `backend/tests/.gitkeep`
- `docs-for-us/architecture/README.md`
- `docs-for-us/diagrams/README.md`
- `docs-for-us/presentation/README.md`
- `docs-for-us/project-overview.md`
- `docs-for-us/README.md`
- `docs-for-us/requirements/README.md`
- `docs-for-us/research/README.md`
- `docs-for-us/services/ai-service.md`
- `docs-for-us/services/backend.md`
- `docs-for-us/services/frontend.md`
- `docs-for-us/testing/README.md`
- `docs-for-us/ux/README.md`
- `docs/architecture/ANTHEIA_Architecture_and_3_Diagrams.docx`
- `docs/architecture/contracts.md`
- `docs/architecture/data-model.md`
- `docs/architecture/decisions.md`
- `docs/architecture/overview.md`
- `docs/architecture/privacy-and-data.md`
- `docs/architecture/recommendation-logic.md`
- `docs/diagrams/ANTHEIA_All_3_Diagrams.drawio`
- `docs/diagrams/context/01_system_context.drawio`
- `docs/diagrams/context/system-context.mmd`
- `docs/diagrams/erd/README.md`
- `docs/diagrams/exports/01_system_context.png`
- `docs/diagrams/exports/01_system_context.svg`
- `docs/diagrams/exports/02_use_case.png`
- `docs/diagrams/exports/02_use_case.svg`
- `docs/diagrams/exports/03_component.png`
- `docs/diagrams/exports/03_component.svg`
- `docs/diagrams/exports/README.md`
- `docs/diagrams/README.md`
- `docs/diagrams/uml/02_use_case.drawio`
- `docs/diagrams/uml/03_component.drawio`
- `docs/diagrams/uml/components.mmd`
- `docs/diagrams/uml/use-cases.puml`
- `docs/evidence-of-relevance/Evidence_of_Relevance_Preliminary_Analysis(2).docx`
- `docs/evidence-of-relevance/README.md`
- `docs/existing-systems/Existing_Systems_Comparison.docx`
- `docs/existing-systems/README.md`
- `docs/literature-review/Fashion_Recommendation_Literature_Review.docx`
- `docs/literature-review/README.md`
- `docs/presentation/README.md`
- `docs/project-management/ANTHEIA_YouTrack_Requirements_Backlog.csv`
- `docs/project-management/deliverables.md`
- `docs/project-management/README.md`
- `docs/project-management/risks.md`
- `docs/project-management/suggested-commits.md`
- `docs/project-management/supervisor-feedback.md`
- `docs/project-management/work-plan.md`
- `docs/project-proposal/README.md`
- `docs/README.md`
- `docs/requirements/ANTHEIA_Requirements_Specification.docx`
- `docs/requirements/README.md`
- `docs/requirements/scope-alignment.md`
- `docs/source-package-README.txt`
- `docs/source-register.md`
- `docs/technology-comparison/README.md`
- `docs/ux/README.md`
- `docs/verification/plan.md`
- `docs/verification/results-template.md`
- `frontend/README.md`
- `frontend/src/.gitkeep`
- `infra/README.md`
- `README.md`

## Suggested future commits

See [the proposed commit plan](suggested-commits.md). It groups structure, proposal, evidence, research, requirements, architecture, UX/verification and management. Use real issue IDs only; no commits have been created.
