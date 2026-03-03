# Repo Agent Context Template

A **template repository** for giving AI coding agents (e.g. Cursor, Claude) and human contributors a consistent, structured context so they can work effectively in your codebase.

## Purpose

When an AI agent or a new developer joins a project, they need the right information at the right time—without drowning in irrelevant docs. This template provides:

- **One entry point** for agents: `CLAUDE.md` (or your agent’s root instruction file)
- **Progressive disclosure**: a small table that points to detailed docs only when needed (build, tests, APIs, security, etc.)
- **Structured agent docs** in `agent_docs/` that you fill in once and keep updated as the project evolves

Use this repo as a **GitHub template** to create new projects, or copy its structure into an existing repo. Then replace the placeholders with your project’s specifics.

## What’s in this repo

| Item | Description |
|------|-------------|
| **`CLAUDE.md`** | Root context for the AI: project overview, tech stack, and a “when you need X → read Y” table. Agents are directed here first. |
| **`agent_docs/`** | Modular docs that agents (and humans) open only when relevant: |

- **`PRODUCT_VISION.md`** — What you’re building and for whom (e.g. press-release style).
- **`building_the_project.md`** — Install, build, env, local run.
- **`testing.md`** — Test commands, coverage, CI, strategy, mocking.
- **`code_conventions.md`** — Style, typing, structure, naming.
- **`service_architecture.md`** — System design, domain model, services, boundaries.
- **`database_schema.md`** — Tables, relationships, migrations, seeding.
- **`api_conventions.md`** — REST, versioning, auth, service-to-service patterns.
- **`deployment_workflow.md`** — CI/CD, env vars per environment, feature flags.
- **`security_checklist.md`** — OWASP, input validation, security rules.

The doc files contain section headers and optional placeholder comments. Fill them in for your stack and product; the structure stays the same so agents know where to look.

## How to use this template

1. **Create a repo from this template**  
   On GitHub: **Use this template** → Create a new repository.

2. **Customize the root context**  
   Edit `CLAUDE.md`: set project name, tech stack, and architecture. Keep the table that points into `agent_docs/`.

3. **Fill in `agent_docs/`**  
   Start with `PRODUCT_VISION.md` and `building_the_project.md`, then add testing, conventions, architecture, database, API, deployment, and security as you need them.

4. **Keep it updated**  
   Treat these docs as the source of truth. When build steps, APIs, or security rules change, update the corresponding file so agents and contributors stay aligned.

## Why it helps

- **Agents** get a single entry point and clear pointers to the right doc, so they don’t hallucinate project structure or conventions.
- **Humans** get the same map and can onboard or switch tasks without hunting for scattered notes.
- **Progressive disclosure** keeps context small until a task requires build, DB, or API details—then the right file is one click away.

---

*Replace the example product vision in `agent_docs/PRODUCT_VISION.md` with your own when you use this template.*
