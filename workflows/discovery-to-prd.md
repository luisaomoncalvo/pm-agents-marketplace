---
description: Full workflow from discovery to PRD. Chains /discovery → assumption mapping → /prd. Use when starting a new feature from scratch with no spec yet. Triggers on /discovery-to-prd.
---

# Workflow: Discovery → PRD

This workflow chains three steps into a single end-to-end process: from identifying the opportunity to having a production-ready PRD.

**Estimated time:** 30-60 minutes of guided work
**Output:** Complete PRD ready for engineering review

---

## Step 1 — Discovery Session (`/discovery`)

Run a full discovery session to define the opportunity.

**Input:** Business goal or problem area
**Output:** Opportunity Solution Tree + ranked opportunities

→ Follow the full `/discovery` skill.

**Checkpoint:** Before moving to Step 2, confirm:
- [ ] We have selected one opportunity to pursue
- [ ] We have a clear desired outcome
- [ ] We understand the primary user segment

---

## Step 2 — Assumption Prioritization

Before writing the PRD, surface and rank the riskiest assumptions.

**From the discovery output, extract:**

| Assumption | Category | Why risky | Test needed before PRD? |
|-----------|---------|-----------|------------------------|
| [Assumption] | Value/Usability/Viability/Feasibility | [Reason] | Yes / No |

**Decision gate:**
- If any **Value assumptions** are unvalidated and high-risk → recommend running a quick experiment before writing the PRD
- If assumptions are low-risk or already validated → proceed to PRD

Ask the user: "Do you want to proceed to the PRD or first validate [highest-risk assumption]?"

---

## Step 3 — PRD Writing (`/prd`)

Write the full PRD using the selected opportunity as the foundation.

**Input:**
- Selected opportunity from Step 1
- Validated assumptions from Step 2
- Any additional context the user provides

**Output:** Complete PRD (all 10 sections)

→ Follow the full `/prd` skill, pre-filling known information from Steps 1-2.

---

## Workflow Output Summary

At the end, produce a summary card:

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
DISCOVERY → PRD COMPLETE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Opportunity selected: [Name]
Target user: [Segment]
Primary metric: [Metric]
PRD status: Draft — ready for review
Key risks: [Top 2 assumptions to watch]
Suggested next: /user-story to break into sprints
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---
*Part of PM Agents Marketplace — github.com/luisaomoncalvo/pm-agents-marketplace*
