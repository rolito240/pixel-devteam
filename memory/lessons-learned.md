# Lessons Learned

## 2026-05-12: DeepSeek V4 Pro Setup
- DeepSeek V4 Pro thinking mode: no separate model ID, use `reasoning_effort="high"` + `extra_body={"thinking": {"type": "enabled"}}`
- Response includes `reasoning_content` field with chain-of-thought
- max_tokens low values (10) all go to reasoning, need 50+ for actual content

## 2026-05-12: Token Optimization
- MiMo infinite loops caused "millions of tokens" consumption - 13 sessions with repeated failed actions
- Smart routing (cheap model for simple tasks) saves 60-80%
- Context compression saves 30-50% on long sessions
- `max_tokens` in config.yaml is IGNORED by Hermes - only `agent.max_turns` works

## 2026-05-10: MCP Configuration
- `${VAR}` shell variable substitution does NOT work in config.yaml env blocks
- Must use literal token values directly
- Workaround: read values from .env programmatically before writing config

## 2026-05-07: GitHub Copilot
- Fine-grained tokens expire - need to regenerate periodically
- Education plan: 300 premium interactions/month, resets 1st of each month
