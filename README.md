# devops-platform

Operational deployment assets for the Sports Betting platform.

## Scope

- Infrastructure and runtime configuration (`infra/`)
- Local and loadtest deployment compose files
- Operational scripts and load/performance scripts (`scripts/`)

## Out of Scope

- Microservice application source code
- Observability dashboards/rules (moved to `observability-platform`)

## Promotion Model

Use environment promotion flow:

`dev -> stage -> perf -> prod`
