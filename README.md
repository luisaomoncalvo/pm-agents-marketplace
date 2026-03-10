# PM Agents Marketplace

A curated collection of AI agents, sub-agents, skills, and workflows for senior Product Managers — built for Claude Code.

Built by [Luis Moncalvo](https://github.com/luisaomoncalvo) — Senior PM in fintech & payments.

---

## What's inside

| Type | Count | Description |
|------|-------|-------------|
| **Skills** | 10 | Slash commands for core PM tasks |
| **Agents** | 3 | Autonomous agents for complex PM work |
| **Workflows** | 3 | Chained multi-step PM processes |

---

## Skills — Slash Commands

| Skill | Trigger | What it does |
|-------|---------|-------------|
| Discovery | `/discovery` | Runs a full discovery session with JTBD and assumption mapping |
| PRD | `/prd` | Generates a production-ready PRD from a brief |
| OKR | `/okr` | Brainstorms and aligns OKRs for a product area |
| Interview | `/interview` | Creates a user interview script and analyzes transcripts |
| Competitive | `/competitive` | Produces a competitive analysis and battlecard |
| Roadmap | `/roadmap` | Builds an outcome-based roadmap |
| GTM | `/gtm` | Designs a go-to-market strategy |
| Retro | `/retro` | Runs a structured sprint retrospective |
| User Story | `/user-story` | Generates user stories and acceptance criteria |
| Metrics | `/metrics` | Reviews product metrics and surfaces insights |

---

## Agents — Autonomous

| Agent | What it does |
|-------|-------------|
| Discovery Agent | Analyzes user interviews, maps assumptions, generates opportunity solution trees |
| PRD Agent | Takes a brief and autonomously writes a full PRD with all sections |
| Competitive Agent | Monitors competitors and produces structured battlecards |

---

## Workflows — Chained

| Workflow | Steps |
|----------|-------|
| Discovery → PRD | Discovery session → Assumption mapping → PRD draft |
| Interview → Stories | Interview script → Transcript analysis → User stories |
| Research → GTM | Competitive analysis → ICP → GTM strategy → Launch plan |

---

## How to install

### Option 1 — Use in Claude Code (recommended)
Copy any `.md` file into your project's `.claude/commands/` folder:
```bash
cp skills/prd.md your-project/.claude/commands/prd.md
```
Then invoke with `/prd` inside Claude Code.

### Option 2 — Use directly with Claude
Open any `.md` file and paste the content as a system prompt or first message.

### Option 3 — Add all skills at once
```bash
mkdir -p your-project/.claude/commands
cp skills/*.md your-project/.claude/commands/
```

---

## Philosophy

- **Outcome-focused**: Every skill drives toward a business result, not just a document
- **Framework-backed**: JTBD, OST (Teresa Torres), OKRs, RICE, ICPs — built in
- **Fintech-aware**: Includes compliance, KYC, API, and payments context where relevant
- **Composable**: Skills chain into workflows; workflows feed agents

---

*Part of the [AI PM Toolkit](https://github.com/luisaomoncalvo/ai-pm-toolkit)*
