# Prompt 4: Annual Goal-Setting Workshop Kit

## When to Use
Use once per year (or at company founding, or when restarting an OKR program). Generates a complete facilitator kit for a 4–8 hour annual planning workshop.

## Input Variables
- `[COMPANY_NAME]` — company name
- `[FACILITATOR_NAME_AND_ROLE]` — e.g., "Alex Chen, CEO"
- `[ATTENDEES]` — list of participants with names and roles
- `[DURATION]` — "half-day (4 hours)" or "full-day (8 hours)"
- `[LAST_YEAR_SUMMARY]` — brief summary of last year's goals and outcomes. Use "N/A — first OKR cycle" if this is new.
- `[STRATEGIC_PRIORITIES]` — 2–3 company priorities for the coming year (e.g., "hit $5M ARR, reduce churn below 5%, launch enterprise tier")
- `[YEAR]` — planning year (e.g., 2027)

## Prompt

```
You are an OKR coach and workshop facilitator. Generate a complete annual goal-setting workshop kit for [COMPANY_NAME] planning for [YEAR].

CONTEXT:
- Facilitator: [FACILITATOR_NAME_AND_ROLE]
- Attendees: [ATTENDEES]
- Duration: [DURATION]
- Last Year Summary: [LAST_YEAR_SUMMARY]
- Strategic Priorities for [YEAR]: [STRATEGIC_PRIORITIES]

GENERATE THE FOLLOWING COMPLETE WORKSHOP KIT:

---
## [COMPANY_NAME] Annual Goal-Setting Workshop — [YEAR]
### Complete Facilitator Kit

---
### MODULE 1: Pre-Workshop Materials (send 1 week before)

**1A — Pre-Read Document (1 page — attendees read in 10 min)**

[Generate a concise pre-read covering:]
- What are OKRs and why they work (4 rules in plain English — no jargon)
- Last year in review: wins, misses, and what we learned (based on LAST_YEAR_SUMMARY)
- Strategic priorities for [YEAR] (the 3 strategic priorities as framed for general audience)
- What attendees should come prepared to discuss: their team's biggest leverage point for [YEAR]
- Logistics: location, agenda preview, what to bring

**1B — Pre-Work Assignment (attendees complete before attending)**

Send this form to each attendee 1 week before. Estimated time: 20 minutes.

[Generate 5 reflection questions covering:]
1. [What did your team achieve last year that you're most proud of?]
2. [What goal did you miss, and what would you do differently?]
3. [What is the single most important thing your team should accomplish in [YEAR]?]
4. [What is one thing the company should STOP doing to free up capacity?]
5. [What cross-functional dependency blocked your team last year, and how should we fix it?]

---
### MODULE 2: Workshop Agenda ([DURATION])

[Generate a detailed timed agenda. For half-day (4hr), scale down. For full-day (8hr), use full version:]

**Full-Day Agenda:**

| Time | Session | Duration | Format | Output |
|------|---------|----------|--------|--------|
| 9:00 | Welcome & Year in Review | 30 min | Plenary | Energy check-in, wins/misses surfaced |
| 9:30 | Strategic Priority Deep-Dive #1 | 40 min | Facilitated discussion | Priority defined with success metrics |
| 10:10 | Strategic Priority Deep-Dive #2 | 40 min | Facilitated discussion | Priority defined with success metrics |
| 10:50 | Break | 10 min | | |
| 11:00 | Strategic Priority Deep-Dive #3 | 40 min | Facilitated discussion | Priority defined with success metrics |
| 11:40 | Company OKR Draft Session | 60 min | Working groups (3–4 people) | Draft 3 company objectives + KRs |
| 12:40 | Lunch | 45 min | | |
| 1:25 | OKR Gallery Walk + Voting | 25 min | All-hands review | Top 3 company OKRs selected |
| 1:50 | Cross-Functional Alignment Review | 30 min | Structured round-robin | Dependencies mapped, gaps identified |
| 2:20 | Department OKR Breakout | 50 min | Department groups | Each dept drafts their OKRs |
| 3:10 | Break | 10 min | | |
| 3:20 | Department Share-Out | 30 min | Plenary | Each dept presents top KR |
| 3:50 | OKR Quality Filter | 20 min | Pairs | All OKRs pass 10-point checklist |
| 4:10 | Commitment Ritual | 20 min | Plenary | Public commitments, accountability partners |
| 4:30 | Close + Next Steps | 15 min | Plenary | Cadence set, owners confirmed |
| 4:45 | End | | | |

**[If half-day: compress to 4 hours — remove one strategic priority deep-dive, shorten breakouts to 30 min each, skip gallery walk, use simplified commitment ritual]**

---
### MODULE 3: Facilitator Scripts

**3A — Opening (verbatim, 3 minutes)**
[Write an energizing opening script that:]
- Acknowledges what the team accomplished last year (without being a laundry list)
- Creates psychological safety: "We will talk about misses today. The goal is learning, not blame."
- Sets expectations: "We will make 3 bets. Not 10. If everything is a priority, nothing is."
- Energizes the room: "The decisions we make today will define what [COMPANY_NAME] is by [YEAR+1]."

**3B — Year in Review Transition (verbatim, 2 minutes)**
[Write a transition script for moving from opening to the Year in Review exercise]

**3C — Strategic Priority Framing (template — use for each priority)**
[Write a 3-sentence framing for each strategic priority provided:
- "Here's the opportunity we see..."
- "Here's the risk if we don't act..."
- "Here's what success looks like..."]

**3D — Cross-Functional Alignment Round-Robin Script (verbatim)**
[Write the exact script for the round-robin exercise:]
"I'm going to ask each team lead to read their most important KR out loud. After you read it, the rest of the room answers: Does anyone here need to do something different for that KR to be achievable? If yes, raise your hand. We'll capture the dependency on the board."
[Continue with facilitation instructions for handling the responses]

**3E — Commitment Ritual Script (verbatim)**
[Write a closing ritual where each leader:]
1. States their team's #1 objective for Q1 aloud to the group (30 sec per person)
2. Names one accountability partner who will hold them to it
3. States one thing they're willing to give up to make room for this objective
[Include facilitator script for wrapping this up and closing the session]

---
### MODULE 4: Breakout Exercise Materials

**4A — Strategic Priority Deep-Dive (40-min breakout)**
[Generate 3 discussion questions for each strategic priority, covering:]
- What does "success" concretely look like by December 31?
- What must be TRUE at the company level for this to happen?
- What are we explicitly NOT doing in pursuit of this priority?
[Provide a structured note-taking template for breakout groups to capture their outputs]

**4B — OKR Draft Session (60-min working groups)**
[Generate working group instructions:]
- Group composition: mix of functions, 3–4 people per group
- Task: Draft 1 company objective + 3 KRs
- Template to fill in: [provide the OKR draft template]
- Constraint: Every KR must have a specific number. "Improve" and "increase significantly" are not KRs.
- Time check: 20 min draft, 20 min sharpen, 20 min prepare to present

**4C — OKR Quality Filter Checklist (pairs exercise, 20 min)**
[Generate a 10-question checklist for pairs to pressure-test each OKR:]
1. [ ] Is the objective inspiring — would it energize the team if read aloud?
2. [ ] Does the objective avoid numbers? (Numbers belong in KRs, not objectives)
3. [ ] Are all KRs measurable with existing data? (Flag any that need new instrumentation)
4. [ ] Is each KR an outcome, not an output? (Test: does it describe *impact*, not *activity*?)
5. [ ] Is each KR achievable at 70% confidence — not guaranteed, not impossible?
6. [ ] Does every KR have exactly one DRI?
7. [ ] Does every KR have a clear baseline (where we are today)?
8. [ ] Are there fewer than 5 KRs per objective?
9. [ ] Does this objective cascade from at least one company objective?
10. [ ] Is there a corresponding KR in another department that depends on this one?

**4D — Department Breakout Instructions**
[Generate clear instructions for the 50-min department breakout:]
- What to do in the first 20 min (review company OKRs, identify which ones your team contributes to)
- What to produce in the next 20 min (draft 1–2 department objectives + 3 KRs each)
- What to present in the final 10 min (1-slide: department objective + top KR + cross-functional dependency)

---
### MODULE 5: Post-Workshop Deliverables

**5A — Post-Workshop Email Template (send within 24 hours)**
[Generate a follow-up email from the facilitator/CEO to all attendees and their teams:]
- Subject line: "[COMPANY_NAME] [YEAR] OKRs — What we decided"
- Body: What was decided (3 company objectives + owners), what each team owns (1 sentence per team), when check-ins start, how to flag concerns or revisions, link to full OKR document [placeholder]

**5B — Annual OKR Calendar**
[Generate a full-year cadence with specific dates for [YEAR]:]
[Table: Month | Activity | Owner | Output]
- Q1: OKR kickoff + Week 6 check-in + Week 12 scoring + retrospective
- Q2: Kickoff + check-ins + scoring
- Q3: Kickoff + check-ins + scoring
- Q4: Kickoff + annual planning prep + check-ins + full-year scoring
- Annual: Workshop (December for next year planning)
[Include recurring meeting names, suggested duration, and required attendees for each]

**5C — Manager Action Items (48-hour checklist)**
[Generate a checklist for each team manager to complete within 48 hours of the workshop:]
1. [ ] Share company OKRs with team (with context, not just the slide)
2. [ ] Schedule team OKR cascade session (Prompt 2 of this skill)
3. [ ] Draft team-level OKRs, share with your manager for alignment
4. [ ] Set up weekly check-in cadence (use Prompt 3 of this skill)
5. [ ] Identify 1–2 ICs who need extra context on the company strategy
6. [ ] Confirm accountability partner from the commitment ritual

---
WORKSHOP FACILITATION RULES:
- Psychological safety is non-negotiable: frame every miss as a learning, never a failure
- No phones during breakouts — capture attention is the product of the workshop
- Every exercise has a concrete output artifact — no "general discussion" without a deliverable
- The commitment ritual is the emotional close of the workshop — don't rush it
- If discussion derails to tactics (which features, which marketing channels): "Park it in the lot"
- Maximum 3 company OKRs exit the room — force prioritization even if painful
- Every attendee must leave knowing their personal #1 priority for Q1
```

## Tips
- The pre-work assignment is the highest-leverage piece — attendees who complete it arrive ready to decide, not just discuss
- The OKR quality filter checklist (4C) alone reduces post-workshop revisions by 60%
- The commitment ritual is awkward if rushed — build in the full 20 minutes
- Save this output as a Google Doc and share with all attendees as the official record of the workshop
