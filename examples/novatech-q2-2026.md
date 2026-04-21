# Example: NovaTech Solutions — Q2 2026 OKR System

**Company:** NovaTech Solutions  
**Stage:** Series A SaaS  
**Headcount:** 35 employees  
**ARR:** $2.1M  
**Mission:** Help mid-market operations teams eliminate manual data entry through AI-powered workflow automation  
**Q2 Top Priority:** Customer retention + expansion revenue (churn hit 8% in Q1 — board flagged)  
**Departments:** Engineering, Sales, Customer Success, Marketing

---

## OUTPUT: Prompt 1 — Company + Department OKR Framework

### NovaTech Solutions — Q2 2026 OKR Framework

---
### Company-Level OKRs

**Objective 1:** Turn our best customers into the proof that NovaTech scales

| Key Result | Metric | Baseline | Target | Owner |
|-----------|--------|---------|--------|-------|
| KR1.1: Net Revenue Retention | % NRR | 94% | 108% | VP Sales |
| KR1.2: Logo Churn Rate | % monthly churn | 8% | <4% | VP Customer Success |
| KR1.3: Expansion revenue from existing accounts | $ | $12K/month | $28K/month | VP Sales |

*Strategic rationale:* Q1 churn rate of 8% is unsustainable at $2.1M ARR — one more quarter at this rate and we're growing a leaky bucket.  
*Stretch factor:* 70% confidence — achievable with CS hiring and new onboarding flow, but requires execution across 3 teams.

---

**Objective 2:** Make our product so obviously valuable that trials convert themselves

| Key Result | Metric | Baseline | Target | Owner |
|-----------|--------|---------|--------|-------|
| KR2.1: Trial-to-paid conversion rate | % | 18% | 28% | VP Product |
| KR2.2: Time-to-first-value (setup to first automation run) | Hours | 72hr | <24hr | VP Engineering |
| KR2.3: Product-qualified leads (PQLs) from free tier | # per month | 22 | 45 | VP Marketing |

*Strategic rationale:* CAC is rising while conversion is flat — we need the product to do more of the selling.  
*Stretch factor:* 65% confidence — 24hr time-to-value requires a new onboarding wizard (Engineering dependency).

---

**Objective 3:** Build the revenue engine that will carry us to Series B

| Key Result | Metric | Baseline | Target | Owner |
|-----------|--------|---------|--------|-------|
| KR3.1: New MRR from outbound | $/month | $14K | $26K | VP Sales |
| KR3.2: Pipeline coverage ratio | 3x plan | 2.1x | 3.5x | VP Sales |
| KR3.3: ICP win rate (enterprise tier, 50–500 employee targets) | % | 22% | 31% | VP Sales + Marketing |

*Strategic rationale:* Series B readiness requires demonstrating a repeatable outbound motion, not just inbound luck.  
*Stretch factor:* 60% confidence — depends on new SDR ramp (hired March 15, needs 45-day ramp).

---

### Department OKRs

**Engineering**  
*Cascades from:* Company Objective 2 — "Make our product so obviously valuable that trials convert themselves"

**Objective:** Ship the onboarding and automation reliability improvements that make NovaTech stick

| Key Result | Metric | Baseline | Target | DRI |
|-----------|--------|---------|--------|-----|
| KR1: Time-to-first-automation (onboarding wizard) | Hours | 72hr | <24hr | Sarah Kim (Eng Lead) |
| KR2: Workflow reliability (automation success rate) | % | 91.3% | 99.1% | Darius Osei (Backend) |
| KR3: API response time p95 | ms | 340ms | <120ms | Marcus Webb (Infra) |

*Cross-functional dependency:* Product must deliver finalized onboarding UX spec by April 30 for Engineering to build  
*Anti-goal:* No new features this quarter — only reliability, performance, and onboarding (feature freeze enforced)

---

**Customer Success**  
*Cascades from:* Company Objective 1 — "Turn our best customers into the proof that NovaTech scales"

**Objective:** Cut churn in half and build a CS motion that scales beyond white-glove

| Key Result | Metric | Baseline | Target | DRI |
|-----------|--------|---------|--------|-----|
| KR1: Monthly logo churn rate | % | 8% | <4% | Jordan Lee (CS Lead) |
| KR2: Customer health score coverage | % of accounts scored | 40% | 95% | Priya Nair (CS Ops) |
| KR3: Expansion revenue influenced by CS | $/month | $4K | $12K | Jordan Lee |

*Cross-functional dependency:* Engineering must deliver health score data API endpoint by May 15  
*Anti-goal:* No new enterprise onboarding commitments until existing onboarding backlog (6 accounts) is cleared

---

**Sales**  
*Cascades from:* Company Objectives 1 + 3 — retention + new ARR

**Objective:** Prove that NovaTech can grow revenue predictably from both existing and new accounts

| Key Result | Metric | Baseline | Target | DRI |
|-----------|--------|---------|--------|-----|
| KR1: Expansion ARR (existing accounts) | $/month | $12K | $28K | AE Team (Riley Chen) |
| KR2: New MRR from outbound | $/month | $14K | $26K | SDR Team (Alex Park) |
| KR3: Enterprise pipeline (50–500 employee ICP) | $ pipeline | $180K | $315K | VP Sales |

*Cross-functional dependency:* Marketing must deliver 2 new case studies (CloudPath + ReportLab) by May 1 for enterprise proof points  
*Anti-goal:* No SMB deals under $500 MRR — AE time is too expensive for sub-threshold accounts

---

**Marketing**  
*Cascades from:* Company Objectives 2 + 3 — conversion + pipeline

**Objective:** Generate qualified pipeline and proof points that close enterprise deals faster

| Key Result | Metric | Baseline | Target | DRI |
|-----------|--------|---------|--------|-----|
| KR1: Product-qualified leads (PQL) from free tier | # per month | 22 | 45 | Morgan Hayes (Demand Gen) |
| KR2: Published case studies (enterprise use cases) | # | 0 | 2 | Yuki Tanaka (Content) |
| KR3: ICP trial starts from paid channels | # per month | 31 | 52 | Morgan Hayes |

*Cross-functional dependency:* CS must identify 2 champion customers willing to be case study subjects by April 20  
*Anti-goal:* No brand awareness campaigns this quarter — all budget is conversion + ICP-targeted

---

### OKR Health Check

**Coverage:** ✅ All 3 company KRs have at least one department KR supporting them  
- NRR 108% → CS KR3 (expansion via CS) + Sales KR1 (expansion ARR)  
- Logo churn <4% → CS KR1 (direct ownership)  
- Trial conversion 28% → Engineering KR1 (time-to-value), Marketing KR1 (PQL volume)

**Stretch Check:**  
- Company O1 (churn + retention): 70% confidence ✅  
- Company O2 (trial conversion): 65% confidence ⚠️ — Engineering dependency is tight  
- Company O3 (new ARR): 60% confidence ⚠️ — SDR ramp risk is real

**Measurability:** ⚠️ CS KR2 (health score coverage) requires Engineering API — instrument before April 30 or revise KR

**Overload check:** All departments at 3 KRs ✅

---

### Alignment Matrix

| Company Objective | Engineering | Customer Success | Sales | Marketing |
|-------------------|-------------|-----------------|-------|-----------|
| O1: Retention + NRR | ⚠️ (API needed) | ✅ | ✅ | ✅ (case studies) |
| O2: Trial conversion | ✅ | ⚠️ (onboarding backlog) | - | ✅ |
| O3: Revenue engine | - | ✅ (expansion) | ✅ | ✅ |

---

## OUTPUT: Prompt 2 — Individual + Team OKR Cascade

**Team:** Engineering  
**Manager:** Sarah Kim, VP Engineering  
**ICs:** Darius Osei (Backend), Marcus Webb (Infrastructure), Lisa Park (Frontend)

---
### Manager OKRs — Sarah Kim, VP Engineering

**Objective 1:** Ship a product that earns trust at every layer of the stack

| KR | Metric | Target | Source |
|----|--------|--------|--------|
| KR1.1: Engineering P0/P1 incidents | Count per month | ≤1 | PagerDuty |
| KR1.2: Sprint commitment accuracy | % stories completed vs. planned | ≥85% | Linear |
| KR1.3: Onboarding wizard shipped and in production | Binary | Yes by May 15 | Deploy log |

**Objective 2:** Build a team that ships fast and stays

| KR | Metric | Target | Source |
|----|--------|--------|--------|
| KR2.1: Engineering eNPS | Score | ≥40 | Quarterly survey |
| KR2.2: PR cycle time (open → merge) | Hours | <18hr | GitHub |

*Manager Anti-Goal:* Stop attending every product sync — delegate to Darius (frees 5hr/week for 1:1s and unblocking)

---
### Individual OKRs

**Darius Osei — Backend Engineer**  
*Primary contribution to:* Engineering KR2 (automation reliability 99.1%)

**Objective:** Make NovaTech's automation engine bulletproof at 10x current scale

| KR | Type | Target | How Measured | Confidence |
|----|------|--------|-------------|------------|
| KR1: Automation success rate | Core | 99.1% | Internal metrics dashboard | 4/5 |
| KR2: P95 error response time | Core | <200ms | Datadog APM | 4/5 |
| KR3: Load test at 10x production traffic passing | Stretch ⚡ | Pass by June 15 | Load test report | 3/5 |

*Dependencies:* Needs Marcus to complete infrastructure autoscaling (KR depends on it) by May 20  
*One-line focus:* "Darius wins if: automation runs don't fail during customer demos or peak usage."

---
**Marcus Webb — Infrastructure Engineer**  
*Primary contribution to:* Engineering KR3 (API p95 <120ms)

**Objective:** Build the infrastructure foundation that makes NovaTech fast enough to be invisible

| KR | Type | Target | How Measured | Confidence |
|----|------|--------|-------------|------------|
| KR1: API p95 latency | Core | <120ms | Datadog | 4/5 |
| KR2: Infrastructure cost per customer | Core | <$18/month | AWS Cost Explorer | 3/5 |
| KR3: Autoscaling fully automated (zero manual capacity incidents) | Stretch ⚡ | 0 incidents by June 30 | PagerDuty | 3/5 |

*Dependencies:* Needs Darius to provide database query profiling report (heavy queries to optimize) by April 30  
*One-line focus:* "Marcus wins if: no customer ever notices the infrastructure."

---
**Lisa Park — Frontend Engineer**  
*Primary contribution to:* Engineering KR1 (time-to-first-value <24hr — onboarding wizard)

**Objective:** Build the onboarding experience that converts skeptical trials into paying customers

| KR | Type | Target | How Measured | Confidence |
|----|------|--------|-------------|------------|
| KR1: Onboarding wizard shipped to production | Core | May 15 | Deploy log | 4/5 |
| KR2: Trial completion rate (% reaching first automation) | Core | 65% | Mixpanel funnel | 3/5 |
| KR3: Onboarding A/B test: 3 variants live | Stretch ⚡ | 3 variants by June 1 | Mixpanel | 3/5 |

*Dependencies:* Needs Product to finalize UX spec by April 30; needs Marketing copy for onboarding email sequence by May 5  
*One-line focus:* "Lisa wins if: a brand-new trial user runs their first automation in under 24 hours."

---
## OUTPUT: Prompt 3 — Weekly Check-in (Week 6 Example)

**Week 6/13 — May 13, 2026**  
Expected % of quarter elapsed: 46%

### Individual Check-in — Lisa Park

**Objective:** Build the onboarding experience that converts skeptical trials into paying customers

| KR | Target | Current | % to Goal | Confidence | Status |
|----|--------|---------|-----------|------------|--------|
| KR1: Onboarding wizard shipped | May 15 | In QA | 85% | 4 | 🟢 |
| KR2: Trial completion rate | 65% | 48% | ~44% | 3 | 🟡 |
| KR3: A/B test 3 variants live | June 1 | 1 variant | 33% | 3 | 🟡 |

**Wins this week:**
- Onboarding step 4 (API key setup) reduced from 3 screens to 1 — A/B test shows 18% higher completion  
- QA found and fixed critical Firefox bug before release

**Blockers:**
- Email sequence copy from Marketing still not received (needed by May 5 — 8 days late). Escalation: need Sarah to follow up with Yuki

**Next week focus:** Ship wizard to production May 15. Begin variant 2 design.

---
### Manager Rollup — Week 6

| IC | Avg Confidence | 🔴 KRs | Blocked On | Trend |
|----|---------------|--------|------------|-------|
| Darius | 3.7 | 0 | Marcus (autoscaling) — on track | ↑ |
| Marcus | 3.3 | 0 | Darius (query profiling) — received | → |
| Lisa | 3.3 | 0 | Marketing copy (8 days late) | → |

**Team Confidence Score (Week 6):** 3.4/5 — Steady  
**Trend vs Week 5:** Flat  
**Escalations:** Marketing/Lisa email copy dependency — needs Sarah action by May 14

**Pacing Alert:**  
- Lisa KR2 (trial completion): Expected 46%, actual ~44% — Within 5% of pace ✅  
- Marcus KR2 (cost/customer): Expected 46% reduction, actual 22% — ⚠️ BEHIND PACE

---
## OUTPUT: Prompt 4 — Annual Workshop Highlights (Q4 Planning for 2027)

### Pre-Work Question Highlights (for NovaTech leadership team)

1. *Most proud of in 2026:* "Reducing churn from 8% to 3.2% in 2 quarters" — Jordan Lee, CS Lead
2. *Missed goal:* "Enterprise pipeline didn't hit 3.5x — ICP definition took too long to finalize. Next year: lock ICP in January, not March."
3. *Biggest leverage point for 2027:* "Expand into Salesforce integration — 40% of ICP prospects asked for it in demos"
4. *What to stop:* "Supporting legacy API v1 — takes 15% of backend time, only 3 customers still using it"
5. *Cross-functional dependency fix:* "Product + Engineering need a shared roadmap lock by Week 2 of each quarter, not ad-hoc"

### Opening Script (excerpt)

*"2026 was the year NovaTech learned what we're actually building. We started the year with an 8% churn rate and a conversion funnel that leaked. We ended it with 3.2% churn, $4.1M ARR, and a product that customers actually finish setting up.*

*Today we make 3 bets for 2027. Not 10. 3. If someone proposes a 4th objective today, I'm going to thank them and park it in the lot.*

*Everything on this whiteboard is fair game — including ideas I've been championing. The best plan wins."*

### Company OKRs 2027 (Workshop Output)

**Objective 1:** Become the default automation tool for operations teams at Series B+ companies  
**Objective 2:** Build a product that grows itself through customer success  
**Objective 3:** Operate with the financial discipline that earns Series B at $10M ARR

### Commitment Ritual (closing)

Each leader read their Q1 objective aloud:
- *Jordan Lee (CS):* "CS owns NRR. We hit 108% or we didn't do our job."  
- *Sarah Kim (Eng):* "The product will not fail during a customer demo in Q1. That's my personal commitment."  
- *Alex Rivera (Sales):* "New MRR from outbound hits $42K by March 31 or I owe the team lunch."  

Accountability partners assigned. Workshop closed 4:47 PM.

---
*Generated by Skill #67: OKR & Goal Setting Framework Generator*  
*All 4 prompts run end-to-end — NovaTech Solutions, Q2 2026*
