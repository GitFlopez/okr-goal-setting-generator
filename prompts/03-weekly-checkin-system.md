# Prompt 3: Weekly Check-in System + Confidence Scoring

## When to Use
Use at the start of the quarter to generate your check-in templates. Then re-run weekly with current status updates to get pacing alerts and manager rollup.

## Input Variables
- `[TEAM_NAME]` — team name
- `[OKRS]` — paste OKRs from Prompt 1 or 2 output
- `[WEEK_NUMBER]` — current week in the quarter (1–13)
- `[QUARTER]` — e.g., Q2 2026
- `[UPDATES]` — brief bullet-point status per KR (format: "KR name: current value, blocker if any"). Leave blank on first run to generate blank template.

## Prompt

```
You are an OKR coach. Generate a complete weekly check-in system for [TEAM_NAME], Week [WEEK_NUMBER] of [QUARTER].

OKRs:
[OKRS]

CURRENT STATUS UPDATES (leave blank for blank template):
[UPDATES]

GENERATE THE FOLLOWING:

---
## [TEAM_NAME] Weekly OKR Check-in — [QUARTER] Week [WEEK_NUMBER]/13

### SECTION 1: Individual Check-in Template

*(Copy this template for each team member — takes <15 min to complete)*

---
**Check-in Form — [QUARTER] Week [WEEK_NUMBER]**
Name: ___________  |  Date: ___________  |  Team: [TEAM_NAME]

**Objective 1:** [Objective text]

| Key Result | Target | Current | % to Goal | Confidence | Status |
|-----------|--------|---------|-----------|------------|--------|
| KR1: [text] | [target] | _______ | ____% | ☐1 ☐2 ☐3 ☐4 ☐5 | 🟢🟡🔴 |
| KR2: [text] | [target] | _______ | ____% | ☐1 ☐2 ☐3 ☐4 ☐5 | 🟢🟡🔴 |
| KR3: [text] | [target] | _______ | ____% | ☐1 ☐2 ☐3 ☐4 ☐5 | 🟢🟡🔴 |

[Repeat for each objective]

**Confidence Scale:**
5 = On track, clear path to target | 4 = On track, minor adjustments needed
3 = At risk, needs attention | 2 = Off track, escalation recommended | 1 = Will not achieve without scope change

**This week's wins (2–3 bullets):**
•
•

**Active blockers (I need help from):**
•

**Next week's #1 priority:**
•

**Energy check:** ☐ Energized ☐ Steady ☐ Stretched ☐ Burnt out
*(Manager reads this — if "stretched" or "burnt out" for 2+ weeks: conversation needed)*

---
### SECTION 2: Manager Weekly Rollup

*(Compile after receiving individual check-ins)*

**[TEAM_NAME] OKR Rollup — Week [WEEK_NUMBER]/13**

| Person | Avg Confidence | 🔴 KRs | Blocked On | Trend |
|--------|---------------|--------|------------|-------|
[One row per team member — fill from individual check-ins]

**Team Confidence Score (Week [WEEK_NUMBER]):** ___ / 5
**Trend vs Last Week:** ☐ Up ☐ Flat ☐ Down

**Active Escalations (confidence ≤ 2):**
[List any KR at confidence 2 or below, owner, and proposed action]

**Wins to celebrate this week:**
[1–2 team-level wins worth calling out in all-hands or Slack]

---
### SECTION 3: Pacing Alerts

[WEEK_NUMBER]/13 = [WEEK_NUMBER/13 × 100 formatted to 0 decimal]% of quarter elapsed.
Expected completion for any linear KR: [same %]%

For each KR in the OKRs provided, generate:

| KR | Target | Expected Now | Required Pace |
|----|--------|-------------|---------------|
[One row per KR — calculate expected value at current week]

**Pacing Flags:** [List any KR where actual current value (if provided in UPDATES) is more than 15% behind expected pace. Mark as ⚠️ BEHIND PACE]

[If UPDATES were provided: assess each KR against expected pace and call out specific KRs that need attention]

---
### SECTION 4: Mid-Quarter Reset Protocol

**Trigger:** If 3 or more KRs are at confidence ≤ 2 by Week 7, run the OKR Reset Meeting.

**Reset Meeting Agenda (45 min):**
1. Review confidence scores — which KRs are truly off track vs. temporarily blocked? (10 min)
2. For each off-track KR: Is the target wrong, the strategy wrong, or execution the issue? (15 min)
3. Decision: Revise target / Revise strategy / Add resources / Accept miss (10 min)
4. Update OKRs with revised targets marked [REVISED] and the date of revision (5 min)
5. Assign one person to own recovery plan for each revised KR (5 min)

**Reset Rules:**
- You can revise KR targets mid-quarter, but you must document why
- You cannot add new objectives mid-quarter (that's scope creep)
- A revised KR is not a failure — an unacknowledged dying KR is

[If WEEK_NUMBER ≥ 7 and UPDATES provided: assess whether reset criteria are met. Output: "RESET RECOMMENDED" or "No reset needed — continue monitoring [specific KR(s)]"]

---
### SECTION 5: Quarter-End Scoring Preview

*(Run in Week 11–12 to project final scores before the formal scoring meeting)*

For each KR, project the likely end-of-quarter score based on current trajectory:

| KR | Target | Current (Week [WEEK_NUMBER]) | Trajectory | Projected Score |
|----|--------|---------------------------|------------|----------------|
[One row per KR — if UPDATES provided, calculate; if not, show formula]

*Score calculation:* OKR Score = (Actual / Target) × confidence_weight
*Confidence weight:* Apply 1.0 for straight-line KRs, 0.8 for KRs with known back-half concentration

---
RULES:
- Confidence is forward-looking ("will we hit this?"), not backward-looking ("did we do work?")
- Check-in should take < 15 minutes per person — if longer, the template is too complex
- Energy check is non-negotiable — it's the burnout early warning system
- Status emoji rules: 🟢 = confidence 4–5, 🟡 = confidence 3, 🔴 = confidence 1–2
- Never punish a 🔴 check-in — the goal is surfacing problems early, not creating fear of reporting
```

## Tips
- Run this prompt at the start of the quarter with UPDATES blank to generate the full template set
- Re-run with actual UPDATES in Week 6 to get your mid-quarter pacing assessment
- The energy check is the most underrated feature — managers who ignore burnout signals lose their best people
