# CLAUDE.md — NewsNook Web App v2

## Project Overview
[TBD]

### Tech Stack: [TBD]

### Architecture
[TBD]

## Product Vision & Requirements
For product vision, positioning, and base requirements, see **`agent_docs/PRODUCT_VISION.md`**. That document is the source of truth for what we are building and why; use it as context when making product or scope decisions.

## Context (progressive disclosure)
Detailed context lives in **`agent_docs/`**. Read the relevant file(s) when working on that area:

| When you need… | Read |
|-----------------|------|
| Install, build, env, local run | **`agent_docs/building_the_project.md`** |
| Tests: commands, coverage, CI, strategy, mocking | **`agent_docs/testing.md`** |
| Style, typing, structure, naming | **`agent_docs/code_conventions.md`** |
| System design, domain model, services, boundaries | **`agent_docs/service_architecture.md`** |
| Tables, relationships, query patterns, migrations, seeding | **`agent_docs/database_schema.md`** |
| APIs: REST, versioning, auth; service-to-service patterns | **`agent_docs/api_conventions.md`** |
| CI/CD, env vars per env, feature flags | **`agent_docs/deployment_workflow.md`** |
| OWASP, input validation, security rules | **`agent_docs/security_checklist.md`** |

## Workflow
- Always run document format tooling before finishing any task
- Run single tests targeting the changed module, not the full suite
- Use Plan Mode for any change touching more than 2 files
- Create a git commit after each logical unit of work (don't batch unrelated changes)
- When compacting, always preserve the list of modified files and pending test commands