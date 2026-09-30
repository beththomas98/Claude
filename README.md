# Recruitment prompts for Claude

## `/ai-sourcing`

Paste (or attach) a job description and Claude will:

1. Break the JD down into titles, must-haves, nice-to-haves, location and exclusions.
2. Write **Tight / Balanced / Broad** Boolean search strings.
3. Search **RMS (our CRM)**, **CV-Library**, **Reed** and **Indeed** for candidates.
4. Return a de-duplicated, ranked shortlist.

**Defaults:** 15-mile radius, CVs active in the last month. Override in the
same message, e.g. `/ai-sourcing radius 25 miles, last 3 months` followed by the JD.

**Accessing the job boards:** Claude uses a connector for a source if one is
connected, otherwise your browser (via Claude in Chrome) where you're already
logged in. If it can't reach a source it will say so and give you the
ready-to-paste string and filters instead — it won't make up results.

The prompt lives in `.claude/skills/ai-sourcing/SKILL.md` — edit it to change
defaults or house style.
