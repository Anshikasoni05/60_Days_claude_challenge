# Day 18 — Custom Skills: Brain Dump Action Planner

## 🎯 Task
Create a reusable **Custom Skill** in Claude that turns messy notes, meeting transcripts, voice memos, and brainstorming sessions into a structured, interactive HTML dashboard — without inventing or assuming any missing information.

## 🛠️ What I Built
A Custom Skill named **`brain-dump-action-planner`** with:
- **Full Breakdown Mode** — single note → structured dashboard
- **Transcript Mode** — speaker-labeled input → adds speaker summaries, decisions by speaker, and attribution notes
- **Merge Mode** — multiple notes/sources → consolidates with duplicate detection and conflict tracking

### Required Output Sections
1. Summary
2. Key Takeaways
3. Action Items (Task / Owner / Deadline / Status table)
4. Open Questions
5. Risks / Blockers
6. Conflicts
7. Additional Notes
8. Source Information (Merge Mode only)

### Status Badges Used
🔴 High Priority · 🟠 Medium Priority · 🟢 Low Priority · ⚠️ Conflict · ❓ Open Question · ✅ Completed · ⏳ Pending

## 📋 Steps Followed
1. Opened Claude and set effort level to Low/Medium.
2. Navigated to **Settings → Skills** and created a new Custom Skill.
3. Named it `brain-dump-action-planner`.
4. Added the description (defines when the skill should trigger) and pasted the full instructions.
5. Saved the skill.
6. Tested it against three different note formats:
   - Plain meeting notes (team sync, Aug 3)
   - Speaker-labeled transcript (Q3 roadmap discussion)
   - Unstructured brainstorm / voice memo (side-project ideas)
7. Merged all three into one dashboard to test **Merge Mode** specifically.
8. Reviewed the generated dashboard for accuracy and rule compliance.

## ✅ Key Observation: The "Never Invent" Rule
The most important design constraint was that the skill must **never guess** missing details. In testing, this held up correctly:
- Tasks with no named owner (e.g. "loop in DevOps on API rate limiting") were labeled **"Not specified"** instead of assigning a guessed owner.
- Deadlines not mentioned in the source stayed blank/"Not specified" rather than being estimated.
- Genuine scheduling conflicts (e.g. marketing's Sept 1 CMS deadline vs. engineering's Sept 10 estimate) were surfaced under a dedicated **Conflicts** section instead of being silently resolved.
- Open, unanswered questions from the notes (e.g. "are we still doing customer interviews this month?") were logged as **❓ Open Questions**, not answered speculatively.

## 📊 Results
- Generated a clean, mobile-responsive interactive dashboard resembling Notion/Linear/Asana-style project tools.
- Action items table pulled tasks, owners, deadlines, and statuses accurately across all three note formats.
- Merge Mode correctly added a Source Information section and per-speaker breakdown for the transcript portion.
- Skill was **fully reusable** — once saved, it didn't require re-pasting instructions for subsequent tests; just pasting new notes triggered the same structured output.

## 💡 Key Learnings
- Custom Skills let you encode a repeatable workflow (structure + rules + output format) once, so future sessions don't need re-explaining.
- Being explicit about a "don't invent, say 'Not specified'" rule in the skill instructions is critical for reliability — without it, models tend to fill gaps with plausible-sounding guesses.
- Designing for multiple **modes** (single note / transcript / merge) inside one skill, rather than three separate skills, kept things simpler while still handling different
- <img width="752" height="766" alt="image" src="https://github.com/user-attachments/assets/063600c9-ddbf-40ac-870e-26cd56e73d43" />
