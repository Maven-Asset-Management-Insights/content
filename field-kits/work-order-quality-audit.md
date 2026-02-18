---
layout: page
title: Work Order Quality Audit Kit
permalink: /field-kits/work-order-quality-audit/
---

High-quality work order data is the foundation for reliability strategy, planning effectiveness, and asset performance analytics. If work orders are missing failure details, inconsistent across crews, or closed without meaningful notes, leaders lose trust in KPIs — and improvement stalls.

This kit provides a practical, repeatable way to measure and improve Work Order (WO) quality in IBM Maximo.

---

## What “Good” Looks Like

A “high-quality” work order should include:

- Clear problem statement (symptom)
- Valid asset/location (not “UNKNOWN” unless justified)
- Work type aligned to the job (PM/CM/EM, etc.)
- Failure class + problem/cause/remedy (where enabled)
- Meaningful completion notes (what was done + what was found)
- Correct status flow (WAPPR → APPR → INPRG → COMP/CLOSE)
- Accurate labor/material postings (no bulk “catch-all” postings)

---

## 30-Minute Audit (Fast Start)

Run this audit monthly (or weekly for critical sites).

### Sample: Checks to perform

1. Randomly sample **25 completed work orders** from the last 30 days  
2. Score each WO using the rubric below  
3. Identify the top 3 data gaps  
4. Publish a short “Quality Reminder” to planners/techs  
5. Re-audit next month and compare trend

---

## Work Order Quality Scoring Rubric (0–10)

Score each WO with 1 point for each item present:

1. Asset populated and correct  
2. Location populated and correct  
3. Work type correct  
4. Problem description is specific (not generic)  
5. Completion notes describe what was done  
6. Failure class recorded (if enabled)  
7. Problem/Cause/Remedy recorded (if enabled)  
8. Labor hours captured (not blank)  
9. Materials captured (or “none used” noted)  
10. Status progression is appropriate (no skipping)

### Interpretation

- **9–10:** Excellent (analytics-ready)  
- **7–8:** Good (minor improvement needed)  
- **5–6:** Concerning (data limits learning)  
- **0–4:** High risk (KPIs and RCA will be unreliable)

---

## Suggested Monthly Targets

- ≥ 80% of sampled WOs score **7+**
- ≥ 50% score **9–10**
- < 10% score **below 5**

---

## Field Coaching Prompts (for supervisors/planners)

Use these quick prompts when reviewing completed WOs:

- “If a different technician read this next month, would they understand what happened?”
- “Can we tell if this was wear-out, misuse, condition, or process?”
- “If this repeats, do we have enough detail to prevent it?”

---

## Optional: Make it Systematic (Reliability-Grade)

Once the audit becomes routine, consider:

- Adding required fields by work type (CM vs PM)
- Using Conditional UI rules (if you have MAS Manage capabilities)
- Training techs using 5 “before/after” WO examples
- Publishing a WO quality dashboard monthly

---

## Outcome

This kit helps Maven clients:

- Improve KPI trust (MTBF/MTTR, backlog, PM compliance)
- Strengthen failure analytics and reliability strategy
- Reduce repeat work through better learning loops
- Build consistent technician/planner habits
