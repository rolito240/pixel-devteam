# Team Conventions

## Code Standards

- **TDD**: test first, code second
- **Commits**: conventional commits (feat:, fix:, docs:, refactor:, chore:)
- **Branches**: feature/nombre-descriptivo
- **PRs**: minimo 1 reviewer antes de merge
- **Linting**: ESLint + Prettier (JS/TS), Ruff (Python)

## Communication

- Tareas SIEMPRE tienen spec escrita en specs/active/
- Agentes dejan notas en tasks/mailbox/ cuando necesitan algo del coordinator
- Coordinator asigna tareas, nunca auto-asignacion
- Cada agente trabaja en su contexto aislado

## Quality Gates

- Code review obligatorio antes de merge
- Security scan en cada PR (agent-safety-review)
- Tests deben pasar antes de merge
- No hardcoded secrets, no API keys en codigo

## Git Workflow

```
main
  └── feature/[task-id]-[description]
  └── hotfix/[issue-description]
```

1. Branch from main
2. Implement + test
3. PR with description
4. Review (Security + QA)
5. Merge to main

## File Organization

- Specs: `specs/active/[project-name]/[spec-name].md`
- Tasks: `tasks/backlog/`, `tasks/in-progress/`, `tasks/done/`
- Reviews: `reviews/[project-name]/[review-type].md`
- Shared: `shared/templates/`, `shared/api-contracts/`
