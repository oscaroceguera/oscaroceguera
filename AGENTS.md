# AGENTS.md

## Project Overview

This is Oscar Oceguera's GitHub profile repository (`oscaroceguera/oscaroceguera`). Its `README.md` is shown on github.com/oscaroceguera, so the README is the product.

- No code, dependencies, build, or test suite. The only content is Markdown with some inline HTML.
- Sources of truth for profile facts:
  - GitHub: github.com/oscaroceguera
  - LinkedIn: linkedin.com/in/oscaroceguerab

## Repository Layout

- `README.md`: the profile page.
- `.claude/skills/update-readme/SKILL.md`: workflow for refreshing the README from GitHub and LinkedIn. Follow it when asked to update the profile.
- `.agents/skills/`: agent skills installed from other repos, tracked by `skills-lock.json`. Don't hand-edit these.

## Editing README.md

- Keep the existing section order, emoji headings, `---` separators, and centered `<div align="center">` blocks.
- Badges use shields.io with `style=for-the-badge` in the main sections and `style=flat-square` in "Quick Facts". Reuse that format for new badges.
- Stats widgets (`github-readme-stats`, `github-readme-streak-stats`, `komarev` profile views) are live images. Don't replace them with static numbers.
- The README is in English. The Spanish testimonial stays as-is, with its English translation.
- Use only facts from the sources above or given directly by Oscar. Never invent roles, dates, numbers, certifications, or testimonials.
- When a number changes (followers, certifications, years of experience, repo count), update every place it appears. Counts are repeated in the header, highlights, and Quick Facts badges.
- The email badge points to `mailto:your.email@example.com`, a placeholder. Don't fill it with a guessed address. Ask Oscar first.

## Checking Changes

There's nothing to build or test. Before finishing:

- Check for unclosed HTML tags (`<div>`, `<table>`, `<details>`) and broken Markdown tables.
- Check that badge URLs are URL-encoded (spaces as `%20`, `+` as `%2B`).
- Preview with `gh markdown-preview` if the extension is installed, or view the pushed branch on GitHub.

## Commits and PRs

- Main branch is `main`. Work on a feature branch and open a PR.
- Use Conventional Commits, e.g. `docs(readme): update certifications for 2026`.
- Don't commit or push unless asked.
