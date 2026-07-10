# Day 6 – Resume ATS Optimization with Claude

## Task
Used Claude as an ATS optimization expert to review and rewrite my resume for better ATS parsing and recruiter readability, then documented the before/after.

## Original Resume
- Had a two-column layout with a profile photo
- Experience section was buried inside "Technical Skills"
- Typos present ("EXpereince", "visulalisation")
- No LinkedIn or GitHub links included
- <img width="712" height="903" alt="image" src="https://github.com/user-attachments/assets/769a3c7f-ba51-4d9f-9439-05b4f270ee40" />


## Optimized Resume
- Removed photo and table/column layout (ATS parsers can't reliably read text next to images or inside table cells)
- Created a proper single-column layout with standard section headings: Professional Summary, Education, Experience, Projects, Skills, Certifications
- Fixed typos and moved Experience out of the Skills section into its own section
- Rewrote the Professional Summary with role-relevant keywords (Python, SQL, Machine Learning, Data Analytics)
- Added LinkedIn and GitHub links as plain, ATS-readable text
- Grouped Skills into labeled categories (Languages, Web, Database, Data & ML, Concepts, Version Control, Soft Skills)
- Result fits cleanly on one A4 page
-<img width="847" height="828" alt="image" src="https://github.com/user-attachments/assets/928bd6e9-28af-476a-9a52-262b9fff26ad" />


## ATS Score
| Version | Score |
|---|---|
| Original | 42/100 |
| After first optimization pass | 89/100 |
| After adding LinkedIn + GitHub | 94/100 |

## Key Learnings
1. Tables, columns, and photos in a resume actively hurt ATS parsing — plain single-column text is safest.
2. Section headings need to match standard ATS-recognized labels (e.g. "Experience", not content buried under "Skills").
3. Keyword alignment in the summary and skills sections matters as much as formatting.
4. Adding verifiable links (LinkedIn, GitHub) with real, quantifiable detail (e.g. "6 public repositories") builds more credibility than generic mentions.
5. Small wording fixes (typos, consistent bullet punctuation) can meaningfully affect keyword-matching accuracy.

## Screenshots
original-resume
<img width="677" height="884" alt="image" src="https://github.com/user-attachments/assets/e9e21a69-54ff-4115-9f4b-0f11161e144f" />

- optimized-resume
- <img width="841" height="828" alt="image" src="https://github.com/user-attachments/assets/02075875-7848-4c70-863b-a533b9343858" />

  ats-score
  <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1b4a5159-470e-4b71-a50e-ba701045f772" />
