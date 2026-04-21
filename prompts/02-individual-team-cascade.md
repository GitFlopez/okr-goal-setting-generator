# Prompt 2: Individual + Team OKR Cascade

## When to Use
Use after Prompt 1. Takes department OKRs and cascades them down to the manager and individual contributor level. Run once per team per quarter.

## Input Variables
- `[TEAM_NAME]` — team name (e.g., "Growth Engineering", "Enterprise Sales")
- `[MANAGER_NAME_AND_ROLE]` — e.g., "Sarah Kim, VP Engineering"
- `[TEAM_MEMBERS]` — list of ICs with names and roles
- `[DEPARTMENT_OKRS]` — paste the relevant department section from Prompt 1 output
- `[QUARTER]` — e.g., Q2 2026
- `[TEAM_SIZE]` — number of people on the team

## Prompt

```
You are an OKR coach. Cascade department-level OKRs down to individual contributors for [TEAM_NAME] in [QUARTER].

DEPARTMENT OKRs (cascade from these):
[DEPARTMENT_OKRS]

TEAM CONTEXT:
- Manager: [MANAGER_NAME_AND_ROLE]
- Team size: [TEAM_SIZE]
- ICs: [TEAM_MEMBERS — name + role per line]
- Quarter: [QUARTER]

GENERATE THE FOLLOWING:

---
## [TEAM_NAME] OKR Cascade — [QUARTER]

### SECTION 1: Manager OKRs ([MANAGER_NAME_AND_ROLE])

[2 objectives max — managers own team health + delivery, not just output]

**Objective 1:** [Team delivery objective — focused on outcomes the team produces]
| KR | Metric | Target | Measurement Source |
|----|--------|--------|-------------------|
| KR1.1 | | | |
| KR1.2 | | | |
| KR1.3 | | | |

**Objective 2:** [Team health / development objective]
| KR | Metric | Target | Measurement Source |
|----|--------|--------|-------------------|
| KR2.1 | | | |
| KR2.2 | | | |

*Manager Anti-Goal:* [One thing the manager will stop doing to make room for these objectives]

---
### SECTION 2: Individual OKRs

For each IC listed, generate:

---
**[IC Name] — [Role]**
*Primary contribution to:* Department KR[N]: "[KR text from above]"

**Objective:** [Individual's primary contribution this quarter — 1 sentence, inspiring]

| KR | Type | Target | How Measured | Confidence |
|----|------|--------|-------------|------------|
| KR1: | Core | | | /5 |
| KR2: | Core | | | /5 |
| KR3: | Stretch ⚡ | | | /5 |

*Dependencies:* [List any other person or team this IC needs a deliverable from to hit their KRs]
*One-line focus:* "This quarter, [IC Name] wins if: [single most important outcome in plain English]"

---
[Repeat for each IC]

---
### SECTION 3: Team Dependency Map

| IC | KR | Depends On | What They Need | By When |
|----|-----|-----------|----------------|---------|
[One row per cross-team or cross-IC dependency]

*Dependency Risk Assessment:* [Flag any dependency where the delivering party has no corresponding KR — this is a blind spot]

---
### SECTION 4: OKR Scoring Rubric

Share this with the team at the start of the quarter:

| Score | Meaning | What to Do |
|-------|---------|-----------|
| 0.0–0.3 | Failed to make meaningful progress | Root cause required; was goal too hard or was execution the issue? |
| 0.4–0.6 | Progress made but target missed | Acceptable if external factors; concerning if repeated 2+ quarters |
| 0.7–0.9 | Delivered — this is the TARGET zone | Celebrate and build on it |
| 1.0 | Fully achieved | Re-evaluate: was this too easy? Should stretch further next quarter |

*Note:* Scoring 0.7 consistently > scoring 1.0 consistently. OKRs should be ambitious.

---
### SECTION 5: Red Flag Triggers

Specific signals that should trigger a team OKR conversation before the next scheduled check-in:

1. [Signal with threshold — e.g., "Any IC's average confidence drops below 3 for 2 consecutive weeks"]
2. [Signal with threshold]
3. [Signal with threshold]
4. [Signal — cross-team]
5. [Signal — external/market]

---
### SECTION 6: Team OKR Summary Card

[One-page summary for the team kickoff meeting:]

**[TEAM_NAME] — [QUARTER] Commitments**
| Person | Objective | Top KR | Confidence |
|--------|-----------|--------|------------|
| [Manager] | | | |
| [IC 1] | | | |
[one row per person]

**Team North Star this quarter:** [Single sentence — if we do nothing else, we must achieve X]

---
RULES:
- Every IC gets exactly 1 stretch KR (marked ⚡) — this is explicitly labeled, not penalized in scoring
- Individual KRs must use "I will" or be directly ownable (no "the team will")
- Maximum 5 KRs per person (3 is ideal)
- Every dependency must have a named owner and a date
- The scoring rubric must be shared before the quarter starts — no surprises at scoring time
```

## Tips
- The "one-line focus" for each IC is the most valuable output for 1:1s — it's the conversation starter for the whole quarter
- If two ICs have the same stretch KR, it's a coordination problem — deduplicate
- Run Prompt 3 immediately after to set up the weekly check-in cadence
