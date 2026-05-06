# devops-platform

Operational deployment assets for the Sports Betting platform.

## Scope

- Shared platform runtime components (`platform/`)
- Environment-specific deployment state (`environments/`)
- Load and smoke testing assets (`loadtests/`)
- Operational automation scripts (`scripts/`)

## Out of Scope

- Microservice application source code
- Observability dashboards/rules (moved to `observability-platform`)

## Promotion Model

Use environment promotion flow:

`dev -> stage -> perf -> prod`

## Repository Layout

- `platform/` shared runtime components (gateway/auth/messaging)
- `services/` service deployment templates and shared manifests
- `environments/` overlays and runtime config for `dev`, `stage`, `perf`, `prod`
- `loadtests/` k6 and Python load/smoke testing scripts
- `pipelines/` promotion and release gate workflows
- `policies/` policy-as-code and validation rules
- `runbooks/` operational procedures
- `scripts/` utility scripts used by operations
