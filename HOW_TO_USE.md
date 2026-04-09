# How to Use

## Setup (already done)
- `master_resume.md` — your complete background, every job, project, and skill. Keep this up to date as you do new things.
- `resume_template.tex` — your LaTeX resume format that all tailored resumes follow.
- `CLAUDE.md` — instructions Claude Code reads automatically when you're in this folder.

## Applying for a job

```bash
cd ~/Documents/resumes
claude
```

Then say:

> "Applying to [Role] at [Company]. Here's the JD: [paste]. Make the resume and a cover letter."

Claude will:
1. Read your full background from `master_resume.md`
2. Pick only what's relevant for that specific role
3. Write and compile a tailored PDF resume → `output/YYYY-MM-DD_Company_Role.pdf`
4. Write and compile a custom cover letter → `cover-letters/YYYY-MM-DD_Company_Role.pdf`

If you don't want a cover letter, just don't mention it.

## Output
```
output/          — tailored resumes (.tex + .pdf)
cover-letters/   — cover letters (.tex + .pdf)
```

Each file is dated and named so nothing gets overwritten.

## Keeping it working well
- Add new projects and jobs to `master_resume.md` as you do them
- Don't edit the files in `output/` or `cover-letters/` — they're generated every time
