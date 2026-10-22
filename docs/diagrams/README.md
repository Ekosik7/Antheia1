# Architecture diagrams

Two sets are intentionally distinguished:

- **Supplied baseline:** original `.drawio` sources in `context/` and `uml/`, original SVG/PNG exports in `exports/`, and the combined three-page drawing in this folder. They are unchanged and accompany the original architecture DOCX.
- **Current proposed design:** new Mermaid/PlantUML definitions below add the requested stack and explicit closet concepts. They are documentation, not application code; newly rendered exports and approval are pending.

| Required diagram | Current definition | Original source |
| --- | --- | --- |
| System Context | [Mermaid](context/system-context.mmd) | [drawio](context/01_system_context.drawio) |
| Use Case | [PlantUML](uml/use-cases.puml) | [drawio](uml/02_use_case.drawio) |
| Component | [Mermaid](uml/components.mmd) | [drawio](uml/03_component.drawio) |

Recommendation Engine stays inside Go. Use-case associations show user goals; optional-photo consent is a precondition. New labels do not renumber the original UC identifiers.

[Exports](exports/README.md) documents baseline images. [ERD](erd/README.md) remains a placeholder. New definitions have not been rendered or visually reviewed; baseline exports must not be presented as updated stack/closet diagrams.