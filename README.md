# DevTeam Studio

**Multi-Agent Development Agency** powered by Hermes Agent + DeepSeek V4 Pro.

## What is this?

This is the headquarters of an AI-powered development team. Each "team member" is a specialized sub-agent invoked via `delegate_task`, with the right model for the job.

## Quick Start

```
# Check task board
cat tasks/BOARD.md

# View team members
cat TEAM.md

# Check conventions
cat CONVENTIONS.md
```

## Architecture

- **Coordinator**: Hermes Agent (deepseek-v4-pro) - orchestrates everything
- **Specialists**: Frontend, Backend, Mobile, AI, DB, Security, DevOps, QA, Data, UI
- **Models**: deepseek-v4-pro (complex), deepseek-v4-flash (fast), mimo-v2-pro (cheap)

## Stack

- Hermes Agent (orchestration)
- DeepSeek V4 Pro / V4 Flash (main models)
- GitHub (version control)
- Supabase (database)
- Playwright (testing)
- Figma (design)

## Contact

- Telegram: @HermesAgent
- GitHub: Mariamm240
