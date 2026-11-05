# AGENTS.md

Rules for any AI agent working on this repository, the personal website of Pinge (Charles) Chen. It is published through GitHub Pages at `CharlesC13.github.io`.

Everything in this repo may become public. Treat every file as something a recruiter could read.

---

## 1. Never publish

These must never appear in any committed file, page, metadata, or commit message:

- **Phone number.** It stays off the site, even though it is on the CV.
- **Personal email addresses** other than the one the owner approved for the site (`pc3191@columbia.edu`).
- **Home or mailing address**, birth date, ID numbers, visa or immigration details.
- **Anything inside `private/`**, including the resume PDF. The folder is git-ignored and must stay that way. Do not link to it, copy from it into public files without approval, or move files out of it.
- **Employer or client confidential information**: internal numbers, client names, deal values, or details beyond what the CV already states. Do not embellish CV metrics or invent new ones.
- **Secrets**: API keys, tokens, passwords, `.env` files, or analytics IDs.
- **Grades or transcripts** beyond the GPAs already listed on the CV.
- **Photos of the owner or anyone else**, unless the owner provides them for the site.
- **Third-party trackers, analytics, ads, or fingerprinting scripts.**

## 2. Ask the owner first

Stop and ask before doing any of the following:

- `git commit`, `git push`, creating or renaming the GitHub repo, or changing GitHub Pages settings. **Nothing is pushed without explicit approval each time.**
- Adding content that is not on the CV, such as new claims, a bio, or a project description, or changing the wording of a CV fact in a way that changes its meaning.
- Changing the section order. It must match the CV: Education → Professional Experiences → Project Experiences → Skills & Interests.
- Adding or changing contact details or social links.
- Deleting, renaming, or overwriting existing files.
- Adding external dependencies: CDNs, fonts, frameworks, build tools, or embeds.
- Anything that costs money, such as custom domains or paid services.
- Any time a rule here seems to conflict with a request. Ask, don't guess.

## 3. Style

### Voice and writing
- Professional but casual: friendly, clear, confident, never boastful.
- Keep CV facts accurate. Rephrase only for readability and keep every number and claim as written.
- American English. Short sentences. Active verbs.
- Dates are formatted `Mon YYYY – Mon YYYY` (for example, `Jun 2026 – Aug 2026`), or `– Present`.

### Visual design
- **Palette: Columbia blue.** All colors are CSS custom properties on `:root`:
  - Columbia blue `#B9D9EB` (accent, highlights)
  - Columbia blue tint `#E8F3FA` (tile backgrounds)
  - Deep blue `#1D4F91` (links, active states)
  - Navy `#0B2D52` (headings)
  - Light and dark themes both come from these tokens. Dark mode follows the system setting.
- **Navigation: streamlined.** One sticky top bar with a link to each CV section, the current section highlighted, and jump tiles near the top of the page. Nothing deeper than one click.
- Layout uses tiles and cards with generous white space and soft corners.
- Use a system font stack. No web fonts unless the owner approves them.
- Responsive from 320px phone width up, with no horizontal page scroll.

### Code
- Plain HTML, CSS, and a little vanilla JS. No frameworks or build step.
- Keep the site self-contained (`index.html` with inline CSS/JS) unless the owner asks for a split.
- Accessibility: semantic landmarks, one `<h1>`, logical heading order, visible focus states, WCAG AA contrast, `prefers-reduced-motion` respected.
- External links open in a new tab with `rel="noopener noreferrer"`.

## 4. Source of truth

- The CV is in `private/Pinge Chen Resume.pdf`. The site content must match it.
- LinkedIn: https://www.linkedin.com/in/pchen13
- GitHub: https://github.com/CharlesC13
