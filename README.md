# agy-marketplace

A personal local marketplace for [Claude Code](https://claude.com/claude-code) plugins.

## Plugins

### agy-subagent

Adds an `agy-worker` subagent that delegates simple search/lookup and repetitive
tasks to the [`agy` CLI](https://antigravity.google/docs/cli/install/) (Google
Antigravity, running on Gemini 3.8 Flash) instead of spending Claude's own
reasoning on them. It intentionally stays out of architecture decisions, code
review, and anything needing careful multi-step judgment — those stay with
Claude.

## Install

```
/plugin marketplace add https://github.com/<owner>/agy-marketplace
/plugin install agy-subagent@agy-marketplace
```

(Replace `<owner>` with this repo's GitHub username once published, or use a
local path instead of the URL for local-only use.)
