# Prompt 1: Company + Department OKR Framework (FREE)

## When to Use
Use this prompt at the start of each quarter to generate your company-level and department-level OKR tree. Run before Prompt 2 (individual cascade).

## Input Variables
Fill in these variables before running:

- `[COMPANY_NAME]` — your company name
- `[COMPANY_STAGE]` — early-stage / growth / enterprise
- `[HEADCOUNT]` — approximate number of employees
- `[TOP_PRIORITY]` — your single biggest bet this quarter (growth, profitability, product quality, retention, market expansion)
- `[DEPARTMENTS]` — comma-separated list (e.g., Engineering, Sales, Marketing, Customer Success)
- `[QUARTER]` — e.g., Q2 2026
- `[REVENUE_TARGET]` — quarterly revenue target or ARR goal (or "N/A — non-revenue quarter")
- `[COMPANY_MISSION]` — one sentence describing what your company does and why

## Prompt

```
You are an OKR coach and strategy consultant with expertise in the Google/Intel OKR methodology. Generate a complete company-level + department-level OKR framework for [COMPANY_NAME].

CONTEXT:
- Company: [COMPANY_NAME]
- Stage: [COMPANY_STAGE] | Headcount: [HEADCOUNT]
- Mission: [COMPANY_MISSION]
- Top Priority for [QUARTER]: [TOP_PRIORITY]
- Departments: [DEPARTMENTS]
- Revenue/ARR Target: [REVENUE_TARGET]

GENERATE THE FOLLOWING:

---
## [COMPANY_NAME] — [QUARTER] OKR Framework

### SECTION 1: Company-Level OKRs (3 objectives maximum)

For each company objective:
**Objective [N]:** [Inspiring, qualitative direction — 1 sentence, present tense, action-oriented, no numbers]

| Key Result | Metric | Baseline | Target | Owner |
|-----------|--------|---------|--------|-------|
| KR[N].1: | | | | |
| KR[N].2: | | | | |
| KR[N].3: | | | | |

*Strategic rationale:* [1 sentence — why this objective matters for the company's mission or survival this quarter]
*Stretch factor:* [Assess whether this is 70% confidence (good) or 50% (too hard) or 90% (too easy)]

---
### SECTION 2: Department OKRs

For each department listed, generate:

**[Department Name]**
*Cascades from:* Company Objective [N] — "[Objective text]"

**Objective:** [Department-level objective — aligned to company O, owned by this team]

| Key Result | Metric | Baseline | Target | DRI |
|-----------|--------|---------|--------|-----|
| KR1: | | | | |
| KR2: | | | | |
| KR3: | | | | |

*Cross-functional dependency:* [Which other department must deliver something for these KRs to be achievable, and what specifically]
*Anti-goal:* [One thing this team is explicitly NOT doing this quarter to stay focused]

---
### SECTION 3: OKR Health Check

Run the following quality checks on the OKRs above:

**Coverage Check:**
Does every company KR have at least one department KR supporting it?
[List: Company KR → Supporting Department KR(s) | Flag any company KRs with no department support]

**Stretch Check:**
Rate each company KR: Too Easy (>90% confidence) / About Right (60–80%) / Too Hard (<50%)
[Table: KR | Confidence Estimate | Assessment]

**Measurability Check:**
Can every KR be measured with data available today?
[Flag any KR that requires a new tracking system or data source not yet in place]

**Overload Check:**
Total KRs per department: [list counts]
Flag any department with >5 KRs total — they need to cut.

---
### SECTION 4: Alignment Matrix

[Table: Company Objectives as rows, Departments as columns. Mark ✅ where a department has a KR supporting that objective. Mark ⚠️ where a department is implicitly needed but has no formal KR.]

---
### SECTION 5: Recommended OKR Kickoff Talking Points

3 key messages for the CEO/leader to communicate when sharing these OKRs company-wide:
1. [Why we chose these 3 objectives over other priorities]
2. [What tradeoffs we made — what we're deprioritizing]
3. [How we'll know if we're on track mid-quarter]

---
RULES TO FOLLOW:
- Maximum 3 company objectives. If you generate more, consolidate.
- KRs must be outcomes, not outputs. "Launch feature X" is an output. "Increase activation rate from 32% to 45%" is an outcome.
- Every KR needs: a specific number, a clear metric name, a baseline, and a target.
- Each KR should have one DRI (directly responsible individual by role, not "the team")
- No more than 2 department KRs should depend on a different department
- Anti-goals are mandatory — they help teams say no to scope creep
```

## Tips
- Run this before your quarterly kickoff meeting — share the output as a pre-read
- The alignment matrix is the most valuable output: it shows cross-functional gaps before they become mid-quarter surprises
- If a department has no OKR cascading from company objectives, that team has no strategic direction — fix this before the quarter starts
