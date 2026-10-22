# Go backend

Status: folder skeleton only. No Go module, source files, endpoints or database integration exists.

Planned responsibilities: guest preferences and Style DNA, optional authentication/profile persistence, closet management and Add Item, occasion/budget handling, product/catalog access, recommendation requests and ranking, feedback, PostgreSQL integration and communication with the optional Python service.

`cmd/` is reserved for the future entrypoint, `internal/` for application modules and `tests/` for future tests. Ranking remains a module in this service. Guest recommendations must not require registration; catalog administration requires authorization if implemented.

See [architecture](../docs/architecture/overview.md), [contracts](../docs/architecture/contracts.md) and [ranking](../docs/architecture/recommendation-logic.md). Setup and tests: not yet implemented.
