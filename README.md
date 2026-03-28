# team-meeting-skill

Multi-role team meeting simulation for solo developers and small teams.

## What it does

Simulates a virtual team of specialists (CEO, Engineer, Product, Designer, Marketing) having structured meetings. Each role speaks from their unique perspective, roles debate and challenge each other, and the meeting produces clear decisions and action items.

## Why

Solo developers make better decisions when they systematically consider multiple viewpoints. This skill forces structured multi-perspective analysis — surfacing blind spots, trade-offs, and risks that a single viewpoint would miss.

## Meeting Types

| Type | Use Case |
|------|----------|
| `progress-sync` | Regular status check-ins |
| `decision` | Choosing between approaches |
| `milestone` | Phase/sprint review |
| `problem-solving` | Bug investigation, incident response |
| `brainstorm` | Feature ideation, creative direction |
| `kickoff` | New project/phase startup |

## Install

```bash
npx skills add Kinghao6666/team-meeting-skill@team-meeting -g -y
```

## Usage

```
/team-meeting progress-sync
/team-meeting decision: Redis vs Memcached for caching
/team-meeting brainstorm: monetization strategies
/team-meeting milestone
```

Or naturally:

```
开个进度会
我们讨论一下这个方案
来个头脑风暴
```

## Custom Teams

Override default roles in your project's `.claude/team.yml`:

```yaml
roles:
  - name: "Alice"
    role: CEO
    style: "Data-driven decision maker"
  - name: "Bob"
    role: Engineer
    style: "Systems thinker, performance-focused"
```

## Compatibility

Works on all platforms supporting the Agent Skills Open Standard (SKILL.md): Claude Code, GitHub Copilot, VS Code Copilot, Cursor, Windsurf, Cline, OpenAI Codex CLI, Gemini CLI, and more.

## License

MIT
