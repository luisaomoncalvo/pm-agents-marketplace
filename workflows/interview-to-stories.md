---
description: Full workflow from user interviews to sprint-ready user stories. Chains /interview → insights synthesis → /user-story. Use after running user interviews and wanting to go straight to dev-ready output. Triggers on /interview-to-stories.
---

# Workflow: Interview → Stories

Takes raw user interview transcripts or notes and turns them into sprint-ready user stories with acceptance criteria.

**Estimated time:** 20-40 minutes
**Output:** Story map + user stories ready for Jira/Linear

---

## Step 1 — Interview Analysis (`/interview` Mode B)

Process all interview transcripts to extract structured insights.

**Input:** Raw interview transcripts or notes (paste them here)
**Output:** JTBD map + unmet needs + key quotes

→ Run `/interview` in Mode B for each transcript.

If multiple transcripts are provided, process them in parallel (as sub-agents) and then synthesize:
- Combine needs that appear in multiple interviews
- Rank by frequency (how many users mentioned it) and pain level

**Synthesis output:**

| Need | Segment | Frequency | Pain | Current workaround |
|------|---------|-----------|------|--------------------|

---

## Step 2 — Insights → Feature Mapping

Bridge the gap between user needs and product features.

For each top-ranked need, define:
- **Feature hypothesis:** "If we build [X], users will be able to [job] without [pain]"
- **Scope:** Minimal version to test the hypothesis
- **Assumption being tested:** What must be true for this to work?

| Need | Feature hypothesis | Scope (S/M/L) | Key assumption |
|------|------------------|--------------|----------------|

Ask the user: "Which of these features should we prioritize for this sprint?"

---

## Step 3 — User Story Generation (`/user-story`)

Convert prioritized features into sprint-ready stories.

**Input:** Selected features from Step 2 + user segments from Step 1
**Output:** Full story map with acceptance criteria

→ Run `/user-story` with the following pre-filled:
- User context from the interviews
- Acceptance criteria derived from the "unmet need" being addressed
- Edge cases from workarounds users described

---

## Workflow Output Summary

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
INTERVIEW → STORIES COMPLETE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Interviews processed: [N]
Unique needs identified: [N]
Stories generated: [N]
  P0 (must have): [N]
  P1 (should have): [N]
  P2 (nice to have): [N]
Top user quote: "[Quote]"
Suggested next: /prd to write the full spec
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---
*Part of PM Agents Marketplace — github.com/luisaomoncalvo/pm-agents-marketplace*
