# Day 4 — Chain-of-Thought Prompting Challenge

## Task
Built a personalized career roadmap using a Chain-of-Thought prompt template in Claude.

## Prompt Approach
Used a structured CoT prompt that had Claude:
1. Ask 4 clarifying questions (current situation, skills, goal, timeline)
2. Reason step-by-step (position → strengths → gaps → fastest path → priorities → projects → networking → milestones)
3. Output a one-page, visually structured PDF roadmap

## My Inputs
- Current situation: Student
- Skills: Python, Web Development, Data Analysis
- Goal: Get a job
- Timeline: 3 months

## Roadmap Output
<img width="1202" height="754" alt="image" src="https://github.com/user-attachments/assets/810775f7-06c3-4039-a322-91fde117d788" />


## Biggest Insight
The bottleneck isn't new skills — it's turning existing skills into visible, provable work (GitHub projects, SQL basics, a sharp resume) fast enough to apply within 3 months.

## Learnings on CoT Prompting
- Asking clarifying questions BEFORE reasoning produces much more personalized output than a single-shot prompt.
- Explicitly listing reasoning steps (1-8) in the prompt made Claude's output more structured and less generic.
- Specifying exact output format (sections, one-pager, visual hierarchy) prevented a wall of unstructured text.
