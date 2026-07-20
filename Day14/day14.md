# Day 14 – AI Red Flag Detector for Job Descriptions
### #60DayClaudeChallenge

## 🎯 Task
Built an AI-powered Red Flag Detector to analyze job descriptions and company
information for red flags before applying — covering unrealistic requirements,
toxic workplace signals, fake remote roles, hiring risks, and company risks.

## 🛠️ Tool Used
Claude (Effort Level: Low)

## 📋 Input
- Job Description: Junior Data Analyst role at DataNova Analytics Pvt. Ltd.
- Company Information: 80–150 employees, founded 2021, AI/BI/ML consulting

## 📊 Output Summary
- **Overall Risk Score:** 78/100
- **Verdict:** ⚠️ Apply with Caution

### Key Red Flags Identified
- "Junior" title requiring 3–5 years + expert-level skills across SQL, Python,
  ML, Deep Learning, AWS, Docker, and Kubernetes
- Misleading remote listing — hidden Bengaluru office requirement
- No salary disclosed
- Scope creep — one role covering analyst + data engineer + ML engineer + DevOps
- Toxic culture language: "fast-paced," "wear multiple hats," "extra hours
  whenever required"

### Risk Breakdown
| Category | Risk Level |
|-----------|-----------|
| Requirements | High |
| Culture | High |
| Remote | Medium-High |
| Hiring | Medium |
| Company | Low-Medium |

### 5 Interview Questions Generated
1. Clarify actual on-site frequency despite "remote" label
2. Which skills are must-have vs. nice-to-have for a "junior" title
3. Request salary band upfront
4. How overtime/workload during tight deadlines is handled
5. Career progression and connecting with a current employee in the role

## 💡 Key Learnings
- A well-structured prompt can turn a job posting into a structured, scored
  risk report in seconds — useful as a pre-application screening step.
- Contradictions between job *title* and job *requirements* (e.g., "Junior"
  + "3–5 years" + "leadership skills") are one of the strongest, most
  reliable red-flag signals.
- "Remote" claims need to be checked against fine print — hidden office
  clauses are a common trap.
- This kind of tool is genuinely reusable for my own job search going forward.

## 📸 Screenshots
<img width="559" height="677" alt="image" src="https://github.com/user-attachments/assets/af1c4403-c098-448a-8017-daef7f69c49d" />
<img width="564" height="602" alt="image" src="https://github.com/user-attachments/assets/da44dee4-e535-4637-806f-9488ae3eaa00" />

---
🔗 Part of the ABTalks 60-Day Claude Challenge
