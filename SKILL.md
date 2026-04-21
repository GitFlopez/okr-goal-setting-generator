# Skill #67: OKR & Goal Setting Framework Generator

**Category:** Business Operations / Strategy  
**Pricing:** $29 one-time | $9.99/month  
**Status:** Ready for ClawHub submission

---

## What This Skill Does

Generates a complete OKR (Objectives & Key Results) system for companies, teams, and individuals — from company-level strategy through individual contributor goals, weekly check-ins, and annual planning workshops.

Four prompts cover the full OKR lifecycle:

1. **Company + Department OKR Framework** — top-down objective tree with cross-functional alignment (FREE)
2. **Individual + Team OKR Cascade** — manager and IC level with scoring rubric
3. **Weekly Check-in System + Confidence Scoring** — progress cadence, red flags, update templates
4. **Annual Goal-Setting Workshop Kit** — facilitator guide, slide deck outline, breakout exercises, scoring rollup

---

## Prompt 1: Company + Department OKR Framework (FREE TIER)

### Input Variables
- `[COMPANY_NAME]` — company name
- `[COMPANY_STAGE]` — stage (early-stage, growth, enterprise)
- `[HEADCOUNT]` — approximate employee count
- `[TOP_PRIORITY]` — single biggest bet for the quarter (growth, profitability, product, retention)
- `[DEPARTMENTS]` — list of departments (e.g., Engineering, Sales, Marketing, CS)
- `[QUARTER]` — e.g., Q2 2026
- `[REVENUE_TARGET]` — quarterly revenue or ARR goal (or N/A for non-revenue teams)

### Prompt Template
```
You are an OKR coach and strategy consultant. Generate a complete company-level + department-level OKR framework for [COMPANY_NAME].

CONTEXT:
- Stage: [COMPANY_STAGE] | Headcount: [HEADCOUNT]
- Top Priority for [QUARTER]: [TOP_PRIORITY]
- Departments: [DEPARTMENTS]
- Revenue/ARR Target: [REVENUE_TARGET]

OUTPUT FORMAT:

## [COMPANY_NAME] [QUARTER] OKR Framework

### Company-Level OKRs (3 max)

For each company objective, write:
**Objective:** [Inspiring, qualitative direction — 1 sentence, present tense, no numbers]
- KR1: [Specific, measurable, time-bound — include exact metric and target]
- KR2: [Specific, measurable, time-bound]
- KR3: [Specific, measurable, time-bound]
*Why this matters:* [1 sentence connecting to company mission/survival]

### Department OKRs (one per department listed)

For each department:
**[Department Name] — Supporting Company Objective: [Which company O does this cascade from]**
**Objective:** [Department-level objective aligned to company O]
- KR1: [Measurable, owned by this team]
- KR2: [Measurable, owned by this team]
- KR3: [Measurable, owned by this team]
*Cross-functional dependency:* [Which other department must contribute for these KRs to be achievable]

### OKR Health Check
- Coverage: Does every company KR have at least one department KR supporting it? [Yes/No + gaps]
- Stretch: Are KRs set at 70% confidence (not 100% certainty)? [Assessment]
- Clarity: Can every KR be measured with data available today? [Flag any that can't]

### Alignment Matrix
[Simple table: Company Objective rows × Department columns, mark which departments contribute to each O]

RULES:
- Max 3 company objectives, max 5 KRs per objective
- KRs must be outcomes, not outputs (not "launch feature X" — instead "increase activation rate by 15%")
- Each KR needs a specific number, percentage, or binary (yes/no achieved)
- No more than 2 KRs per team should depend on another team
```

---

## Prompt 2: Individual + Team OKR Cascade

### Input Variables
- `[TEAM_NAME]` — team name (e.g., "Growth Engineering")
- `[MANAGER_NAME]` — manager's name and role
- `[TEAM_MEMBERS]` — list of IC names and roles
- `[DEPARTMENT_OKRS]` — paste in the department OKRs from Prompt 1
- `[QUARTER]` — quarter

### Prompt Template
```
You are an OKR coach. Cascade department-level OKRs down to individual contributors for [TEAM_NAME] in [QUARTER].

DEPARTMENT OKRs (to cascade from):
[DEPARTMENT_OKRS]

TEAM:
- Manager: [MANAGER_NAME]
- ICs: [TEAM_MEMBERS]

OUTPUT FORMAT:

## [TEAM_NAME] OKR Cascade — [QUARTER]

### Manager OKRs ([MANAGER_NAME])
[2 objectives max — focused on team health, delivery, and cross-functional outcomes]
**Objective 1:** [Team-level delivery objective]
- KR1: [Team throughput or quality metric]
- KR2: [Stakeholder satisfaction or dependency metric]
- KR3: [Process or velocity metric]

**Objective 2:** [Team development or health objective]
- KR1: [Individual growth metric — e.g., N team members promoted, eNPS ≥ X]
- KR2: [Skill development or retention metric]

### Individual OKRs (for each IC listed)
For each IC:
**[IC Name] — [Role]**
*Supports Department KR:* [Which specific KR from Prompt 1 output]
**Objective:** [Individual's primary contribution this quarter]
- KR1: [Personal output metric tied to team KR]
- KR2: [Quality or reliability metric]
- KR3: [Stretch / learning KR — explicitly marked as stretch]

*OKR Score Rubric (end of quarter):*
| Score | Meaning |
|-------|---------|
| 0.0–0.3 | Failed to make meaningful progress |
| 0.4–0.6 | Made progress but missed target |
| 0.7–0.9 | Delivered — this is the target zone |
| 1.0 | Fully achieved (re-evaluate if too easy) |

### Team Dependency Map
[For each IC's KR that requires another person or team, flag it with: "DEPENDENCY: [IC Name] KR[N] requires [Person/Team] to [action] by [date]"]

### Red Flag Triggers
List 3 specific signals that would indicate OKRs need to be revised mid-quarter:
1. [Specific trigger with threshold]
2. [Specific trigger with threshold]
3. [Specific trigger with threshold]

RULES:
- Individual KRs must be directly ownable by that IC (no "we will" language)
- Every IC gets exactly 1 stretch KR clearly labeled
- No IC should have more than 5 KRs total
```

---

## Prompt 3: Weekly Check-in System + Confidence Scoring

### Input Variables
- `[TEAM_NAME]` — team or individual name
- `[OKRS]` — paste all OKRs (from Prompts 1 or 2)
- `[WEEK_NUMBER]` — current week in quarter (1–13)
- `[UPDATES]` — brief bullet-point status per KR (optional — leave blank for template only)

### Prompt Template
```
You are an OKR coach. Generate a complete weekly OKR check-in system for [TEAM_NAME], Week [WEEK_NUMBER] of the quarter.

OKRs:
[OKRS]

CURRENT STATUS UPDATES (if available — leave blank for template):
[UPDATES]

OUTPUT FORMAT:

## Weekly OKR Check-in — Week [WEEK_NUMBER]/13

### Check-in Template (copy for each team member)
**Name:** ___________  |  **Date:** ___________  |  **Team:** [TEAM_NAME]

For each OKR:
**Objective [N]: [Objective text]**

| Key Result | Target | Current | % Complete | Confidence (1–5) | Status |
|-----------|--------|---------|------------|------------------|--------|
| KR1: [text] | [target] | [fill in] | [calc] | [1-5] | 🟢/🟡/🔴 |
| KR2: [text] | [target] | [fill in] | [calc] | [1-5] | 🟢/🟡/🔴 |

**Confidence Key:**
- 5 = On track, no blockers
- 4 = On track with minor adjustments needed
- 3 = At risk, needs attention
- 2 = Off track, escalation recommended
- 1 = Will not achieve without scope change

**This week's wins (2–3 bullets):**
-
-

**Blockers (requires help from):**
-

**Next week's focus:**
-

---
### Manager Weekly Rollup Template
| IC Name | Avg Confidence | Red KRs | Blocked On | Action |
|---------|---------------|---------|------------|--------|
[One row per IC]

**Team Confidence Score:** [Average of all KR confidence scores]
**Trend vs Last Week:** [Up/Down/Flat]
**Escalations Required:** [List any confidence ≤ 2]

---
### Quarter Pacing Check (Week [WEEK_NUMBER])
Expected % complete at Week [WEEK_NUMBER]: [WEEK_NUMBER/13 × 100]%
[For each KR: flag if actual % < expected % - 15% as "BEHIND PACE"]

### Mid-Quarter Reset Trigger
If 3+ KRs are at confidence 2 or below by Week 7: recommend formal OKR reset meeting.
[If current week ≥ 7 and updates provided: assess whether reset is warranted]

RULES:
- Status emoji: 🟢 = confidence 4-5, 🟡 = confidence 3, 🔴 = confidence 1-2
- Confidence is forward-looking (will we hit this?), not backward-looking (did we do work?)
- Check-in should take < 15 minutes to complete per person
```

---

## Prompt 4: Annual Goal-Setting Workshop Kit

### Input Variables
- `[COMPANY_NAME]` — company name
- `[FACILITATOR_NAME]` — workshop lead
- `[ATTENDEES]` — list of participants and roles
- `[DURATION]` — workshop length (half-day = 4hr, full-day = 8hr)
- `[LAST_YEAR_SUMMARY]` — brief summary of last year's goals and outcomes (or "N/A — first OKR cycle")
- `[STRATEGIC_PRIORITIES]` — 2–3 company priorities for the coming year

### Prompt Template
```
You are an OKR coach and workshop facilitator. Generate a complete annual goal-setting workshop kit for [COMPANY_NAME].

CONTEXT:
- Facilitator: [FACILITATOR_NAME]
- Attendees: [ATTENDEES]
- Duration: [DURATION]
- Last Year Summary: [LAST_YEAR_SUMMARY]
- Strategic Priorities for Coming Year: [STRATEGIC_PRIORITIES]

OUTPUT FORMAT:

## [COMPANY_NAME] Annual Goal-Setting Workshop — Facilitator Kit

### Pre-Workshop (send 1 week before)
**Pre-read document (1 page max):**
[Generate a concise pre-read covering: OKR refresher (5 rules), last year retrospective, 3 strategic priorities for the year, what attendees should come prepared to discuss]

**Pre-work assignment for attendees:**
[3 questions each person should answer in writing before attending]

---
### Workshop Agenda ([DURATION])

[Generate a timed agenda with:
- Opening: Year in Review (wins + misses, no blame) — 30 min
- Strategic Priority Deep-Dive — 45 min per priority
- Company OKR Draft Session (working groups) — 60 min
- Cross-functional Alignment Review — 30 min
- Departmental OKR Breakout — 45 min
- Commitment + Accountability Ritual — 20 min
- Close + Next Steps — 15 min
Adjust timing proportionally for half-day vs full-day]

---
### Facilitation Script (key transitions)

**Opening (verbatim script for facilitator):**
[Write an energizing 3-minute opening that: acknowledges last year, creates psychological safety, sets the tone for ambitious but achievable goals]

**Year in Review exercise (10 min, pairs):**
[Structured debrief questions — 3 wins, 3 misses, 1 "if we could do it again" per person]

**Strategic Priority breakout prompt:**
[For each priority: What does success look like? What must be true? What are we not doing?]

**Cross-functional alignment check script:**
["Read out your top KR. Does anyone in this room need to do something different for you to hit it?" — structured round-robin]

**Commitment ritual:**
[Specific closing exercise — e.g., each leader reads their #1 objective aloud to the group + accountability partner assignment]

---
### Breakout Exercise: OKR Quality Filter
[Generate a 10-question checklist teams use to pressure-test each objective and KR before submitting]

---
### Post-Workshop Next Steps Template
[Generate a follow-up email template: attendee sends to their teams within 24 hours, covering: what we decided, what each team owns, when check-ins start, how to flag concerns]

---
### Annual OKR Calendar
[Generate a quarterly cadence for the full year: OKR setting → mid-quarter check → end-of-quarter scoring → retrospective → next quarter planning. Include specific week numbers and meeting types]

RULES:
- Workshop should feel energizing, not bureaucratic
- Every exercise has a clear output artifact
- No more than 3 company OKRs exit the workshop (force prioritization)
- Psychological safety: frame misses as learning, not failure
- Every attendee leaves knowing their #1 priority for Q1
```

---

## Example Output

See `examples/novatech-q2-2026.md` for a complete worked example:  
- Company: NovaTech Solutions (Series A SaaS, 35 employees, $2.1M ARR)  
- Quarter: Q2 2026  
- All 4 prompts run end-to-end

---

## Pricing Strategy

| Tier | Price | What's Included |
|------|-------|-----------------|
| **Free** | $0 | Prompt 1 only (Company + Department Framework) |
| **OKR Kit** | $29 one-time | All 4 prompts |
| **Monthly** | $9.99/month | All 4 prompts + quarterly updates as OKR best practices evolve |
| **Done-For-You** | $147/workshop | Max runs all 4 prompts for your team, delivers formatted Google Doc |

**DFY Agency Tier:** $397 for annual workshop facilitation kit + 4 quarterly OKR sets (13 weeks of check-in templates)

---

## Target Buyers

- Startup founders and CEOs (Series A–C, 10–200 employees)
- Engineering, Product, Sales, Marketing managers at growing companies
- HR/People ops leads running company-wide goal-setting cycles  
- OKR coaches and management consultants building client deliverables
- MBA students and business school educators

---

## Competitive Edge

| Competitor | Price | What They Do | What We Do Better |
|-----------|-------|--------------|-------------------|
| Lattice | $11/user/month | Platform + templates | We're $29 once — just the prompts, no platform lock-in |
| 15Five | $14/user/month | Check-in platform | Our check-in template is free + more structured |
| Asana Goals | $10.99/user/month | Goal tracking UI | No prompt system, no facilitation kit |
| OKR Coach (human) | $150-300/hr | Custom workshops | Our kit = same output for $147 DFY or $29 DIY |
| Free templates | $0 | Static Google Docs | No prompts, no cascade system, no workshop kit |
