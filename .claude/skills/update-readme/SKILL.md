---
name: update-readme
description: Update README with my personal info about my professional career, using my GitHub account (github.com/oscaroceguera) and LinkedIn profile (linkedin.com/in/oscaroceguerab) as sources. Use whenever I ask to update, refresh, or sync my profile README.
---

# Update README

Refresh `README.md` (my GitHub profile README) with current info about my professional career.

## Sources

1. **GitHub** — `github.com/oscaroceguera`. Prefer the `gh` CLI:
   - `gh api users/oscaroceguera` — bio, company, location, blog, followers
   - `gh api "users/oscaroceguera/repos?sort=pushed&per_page=30"` — recent/notable repos, languages, stars
   - `gh api users/oscaroceguera/events/public` — recent activity
   - `gh api "search/commits?q=author:oscaroceguera&sort=author-date&order=desc"` if more activity detail is needed
2. **LinkedIn** — `linkedin.com/in/oscaroceguerab`. LinkedIn usually blocks unauthenticated fetches, so:
   - Try WebFetch first.
   - If blocked, use the Chrome browser tools (logged-in session) to read the profile: headline, current role, experience, skills, certifications, education.
   - If neither works, tell me and ask me to paste the relevant sections. Never invent career details.

## Steps

1. Read the current `README.md` fully to understand its structure, tone, and sections.
2. Gather data from both sources.
3. Compare: identify what is new or outdated (role, company, years of experience, tech stack, featured projects, achievements, stats).
4. Edit `README.md` in place:
   - Keep the existing structure, style, badges, and language unless something is clearly obsolete.
   - Update only what changed; don't rewrite sections that are still accurate.
   - Only include facts found in the sources or provided by me.
5. Show me a short summary of what changed and which facts came from which source. Flag anything I should verify.
6. Do not commit or push unless I ask.
