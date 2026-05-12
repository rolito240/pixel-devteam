# DevTeam Studio

## Team Members

| Agent | Role | Model | Cost Tier |
|-------|------|-------|-----------|
| Coordinator | Orquestador Principal | deepseek-v4-pro | Medio |
| Frontend Dev | UI/UX, React, Next.js, Tailwind | deepseek-v4-flash | Bajo |
| Backend Dev | APIs, Node, Python, Go | deepseek-v4-pro | Medio |
| Mobile Dev | Flutter, React Native | deepseek-v4-flash | Bajo |
| AI Engineer | Agentes, RAG, Fine-tuning | deepseek-v4-pro | Medio |
| DB Architect | SQL, NoSQL, Supabase, MongoDB | deepseek-v4-pro | Medio |
| Security Auditor | OWASP, Pentest, Hardening | deepseek-v4-pro | Medio |
| DevOps | Docker, CI/CD, Cloud | deepseek-v4-flash | Bajo |
| QA Tester | E2E, Unit, Playwright | mimo-v2-pro | Minimo |
| Data Analyst | Power BI, SQL, DAX | deepseek-v4-flash | Bajo |
| UI Designer | Figma, Design Systems | deepseek-v4-flash | Bajo |

## How to invoke agents

All agents are invoked through `delegate_task` by the Coordinator.

```python
# Example: delegate frontend work
delegate_task(
    goal="Implement React component X per spec",
    context="Spec: specs/active/project/component-X.md\nStack: React + TypeScript + Tailwind",
    toolsets=['terminal', 'file'],
)
```

## Cost Strategy

- **MiMo (mimo-v2-pro)**: Ultra-cheap. QA testing, simple lookups, formatting.
- **DeepSeek V4 Flash**: Cheap+fast. Frontend, mobile, DevOps, data analysis.
- **DeepSeek V4 Pro**: Medium cost. Backend, AI, DB, security, complex logic.
- **Copilot GPT-5**: Expensive. Reserve for critical code generation only (300 interactions/month).
