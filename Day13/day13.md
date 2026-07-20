# Day 13 — Job Discovery & Analysis with Claude + Indeed Connector

## 🎯 Task
Use Claude's Indeed MCP connector to automate the early stages of a job search: build a structured professional profile, define job search criteria, and let Claude discover, score, and analyze real job postings against that profile — closing the loop from "I need a job" to "here's what to apply to and why."

## 🛠️ Workflow
1. **Prompt 1 — Professional Profile:** Gave Claude a structured prompt covering current role, skills, domain expertise, and achievements. Claude compiled this from prior conversation context (skills, certifications, CGPA, GitHub/LinkedIn presence).
2. **Prompt 2 — Job Search Criteria:** Defined target title (Data Analyst), location flexibility (open to remote/hybrid/onsite), and company type (open to any) — Claude asked clarifying questions via quick-select options instead of guessing.
3. **Prompt 3 — Job Discovery & Analysis:** Connected the Indeed MCP connector and asked Claude to search live listings, score them against my profile, and return a comparison table with company, role, location, posted date, apply link, match score, fit reasoning, and CTC.

## 📊 What Claude Delivered
- A ranked table of **6 live Data Analyst openings** across Delhi NCR, Pune, Madurai, and remote — with match scores from 50–90%, direct apply links, and posted dates (filtered out a stale 5-month-old listing and a mismatched 2+ year e-commerce role that Indeed had mislabeled as "Data Analyst").
- **Skill gap analysis:** flagged Power BI/Tableau and Advanced Excel as the most in-demand skills missing clear evidence in my current profile — the biggest lever for improving match quality.
- **Market demand insights:** most fresher-level Data Analyst hiring in India currently runs through Intern/Trainee/Junior titles first, with pay clustering ₹2L–4.5L/year, and hybrid/in-person roles outnumbering remote at entry level.
- **Actionable recommendations:** build a Power BI/Tableau portfolio project, surface Advanced Excel skills explicitly on the resume, prioritize NCR-hybrid roles for logistics, and apply within the first 1–2 weeks of a posting going live.

## 💡 Key Learnings
- Connecting a live job-board MCP connector turns Claude from an advisor into an active researcher — it pulled real, current listings instead of generic advice.
- Letting Claude ask clarifying questions (via quick-select prompts) upfront produced far more targeted search criteria than a single open-ended prompt would have.
- Match scoring is only as good as the filtering behind it — Claude caught a mislabeled listing and a stale posting that a keyword-only search would have surfaced as "matches."
- Skill-gap analysis grounded in actual job postings (not generic advice) gives a much clearer, more prioritized next step than a general "learn these skills" list.

## 🔗 Screenshots
<img width="809" height="660" alt="image" src="https://github.com/user-attachments/assets/88429a77-51bf-4fa6-a03e-7ad799298acd" />

---
#60DayClaudeChallenge Day 13 · @Anthropic @ABTalksOnAI @AnilBajpai
