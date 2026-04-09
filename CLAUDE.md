# Resume Tailoring

## Files
- `master_resume.md` — my complete background (all projects, jobs, skills, everything)
- `resume_template.tex` — my base LaTeX resume to use as the formatting reference
- `output/` — tailored resumes go here
- `cover-letters/` — cover letters go here

## What to do when I give you a job description

I'll tell you the company name, role, and paste the job description. Then:

1. Read `master_resume.md` for my full background
2. Read the most recent `.tex` file in `output/` as a style/formatting reference
   (skip this step if `output/` is empty)
3. Write a tailored resume to `output/YYYY-MM-DD_Company_Role.tex`
   - Pick only what's relevant to the role — omit rather than pad
   - Mirror the language and keywords from the job description
   - Keep it one page unless it's a senior/staff role
   - Preserve the LaTeX structure from `resume_template.tex`
4. Compile it: `pdflatex -interaction=nonstopmode -output-directory=output output/YYYY-MM-DD_Company_Role.tex`
   - Run it twice if there are any reference/layout issues
   - Tell me if pdflatex isn't installed
5. If I asked for a cover letter:
   - Write it as a LaTeX document to `cover-letters/YYYY-MM-DD_Company_Role.tex`
     - Clean, professional formatting — full letter layout with my name/contact at the top
     - Enthusiastic and specific to this company and role
     - Explain why I want THIS job at THIS company (infer from the JD)
     - Why I'm a strong fit — connect my actual experience to their needs
     - No generic filler like "I am writing to express my interest"
   - Compile it: `pdflatex -interaction=nonstopmode -output-directory=cover-letters cover-letters/YYYY-MM-DD_Company_Role.tex`

## Preferences
- Prioritize projects with real users or real impact over coursework
- Include GitHub/live links for projects where relevant
- Lead with the most impressive/relevant stuff for that specific role
- If a skill or project isn't relevant to this job, cut it
