# Engineering Rules

## Scope
- Implement only the explicitly assigned task.
- Do not add product functionality outside the task.
- Do not make architectural changes without documenting the reason.
- Prefer the smallest maintainable implementation.

## Security
- Never commit secrets, API keys, tokens, passwords, or private credentials.
- Keep server-only secrets out of client code.
- Treat all external and AI-generated data as untrusted input.
- Enforce authorization at the server boundary for tenant-scoped data.

## AI
- AI output is never the source of truth.
- Validate model output against an explicit schema before persistence or external actions.
- No autonomous external customer communication without explicit human approval in the product design.

## Quality
- Every task must have explicit acceptance criteria.
- Run relevant tests, type checks, and linting before declaring a task complete.
- Do not hide failing checks or weaken tests merely to make a task pass.
- Avoid unnecessary dependencies.

## Workflow
- Keep implementation changes traceable to a task.
- Record important architectural decisions in project documentation.
- Independent review is required before major architecture changes or implementation gates are approved.
