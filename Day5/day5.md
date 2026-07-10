# Day 5 — Context Engineering

**Challenge:** ABTalks 60-Day AI Challenge
**Topic:** Context Engineering — comparing AI outputs with and without context

---

## Task

Compare two versions of the same prompt — one with no context, one with detailed personal context — to observe how context changes the quality and relevance of an AI's output.

---

## Prompt A (No Context)

```
Create a 30-day learning roadmap.
```

### Output A

**30-Day Learning Roadmap**

**Week 1: Foundations**
- Day 1–2: Assess your current skill level and choose a primary focus area (e.g., programming, design, data)
- Day 3–5: Complete beginner tutorials in your chosen area
- Day 6–7: Practice exercises to reinforce basics

*Milestone: Understand core fundamentals*

**Week 2: Building Skills**
- Day 8–10: Work through intermediate tutorials
- Day 11–12: Start a small practice project
- Day 13–14: Review and refine what you've learned

*Milestone: Apply skills in a small project*

**Week 3: Practical Application**
- Day 15–17: Build a more complex project
- Day 18–19: Learn a complementary tool or technology
- Day 20–21: Get feedback on your project

*Milestone: Complete an intermediate-level project*

**Week 4: Portfolio & Job Readiness**
- Day 22–24: Polish your project(s)
- Day 25–26: Update your resume and LinkedIn
- Day 27–28: Practice interview questions
- Day 29–30: Final review and next-steps planning

**Final Outcome:** A completed project and a stronger resume/profile to start applying for relevant roles.

---

## Prompt B (With Context)

```
Create a 30-day learning roadmap.

Context:
- Current Situation: Student
- Current Skills: Python, Java Basics, HTML,CSS,C,Excel,ML
- Goal: to improve my skills within 3 months so that i get high paying job
- Available Time: 3 hrs per day
- Experience Level: Beginner
- Preferred Learning Style: Reading and project

Include:
- Weekly milestones
- Daily tasks
- Resources
- Projects
- Final outcome
```

### Output B (summary — full version saved separately)

- **Week 1:** Python refresh (functions, OOP) + Git/GitHub + SQL basics → **Project:** Python CLI Expense Tracker
- **Week 2:** pandas/numpy + data cleaning + visualization → **Project:** EDA Notebook on a Kaggle dataset
- **Week 3:** HTML/CSS/JS refresh + deployment → **Project:** Live personal portfolio website
- **Week 4:** Applied ML + Streamlit deployment + resume/LinkedIn overhaul → **Project:** Deployed ML web app

**Final Outcome:** 3 portfolio projects (all on GitHub), a live portfolio site, working knowledge of Git/SQL/pandas/deployment, an updated resume and LinkedIn, and a visible learning trail documenting progress.

*(Full daily breakdown with resources saved as `30-Day-Learning-Roadmap.md` in this repo / attached separately.)*

---

## Comparison

| Aspect | Prompt A (no context) | Prompt B (with context) |
|---|---|---|
| Starting point | Assumes nothing — generic "assess your level" | Starts from actual existing skills (Python, HTML/CSS, ML basics) |
| Specificity | Vague tasks ("complete tutorials") | Named resources, exact daily tasks, named tools (Git, SQL, Streamlit) |
| Time fit | No mention of daily time budget | Built around a 3 hrs/day budget |
| Learning style | Ignored | Matches stated reading + project preference |
| Projects | Generic "a project" | 3 concrete, named projects (CLI tool, EDA notebook, deployed ML app) |
| Career target | Generic "relevant roles" | Targets data analyst / junior data scientist roles, closes named skill gaps (SQL, Git, deployment, LinkedIn) |

---

## Key Learnings

1. **Context turns a generic template into an actionable plan.** Without context, the AI has to guess at a starting point and fills in the gaps with placeholders — the output is safe but not usable as-is.
2. **Specific constraints (time, skill level, learning style) produce specific outputs.** Stating "3 hrs/day" and "beginner, reading + project style" removed guesswork and produced a day-by-day plan that's realistic to actually follow.
3. **Naming existing skills prevents wasted effort.** Prompt B skipped re-teaching Python/HTML basics already known and instead targeted real gaps (SQL, Git, deployment) — this is the core value of context engineering: relevance over generic completeness.
4. **A clear goal (job in 3 months) shapes prioritization.** With that context, the roadmap prioritized portfolio-building and job-readiness (resume, LinkedIn, deployment) over abstract skill mastery.
5. **Takeaway for future prompts:** the more specific and structured the context given to an AI, the less generic and more directly usable the output — this is the practical difference between "asking a question" and "engineering a prompt."

---

**Challenge Day:** 5/60
**Date:** 11-07-2026
