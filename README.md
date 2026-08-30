# The Christ Frequency — Landing Page

Landing page for *The Christ Frequency* by Gideon George, offering the free
7-day starter guide and collecting email signups.

## Contents

- `index.html` — the full single-file landing page (styles and scripts inline)
- `privacy.html` — privacy policy, linked from the footer
- `tcf-cover.jpg` — cover image used on the page and for social share previews
- `tcf-cover-small.jpg` — smaller cover variant

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```bash
python -m http.server 8000
```

## Notes

Analytics and pixel snippets (GA4, Meta) are present in `index.html` as
commented-out placeholders — drop in your IDs to switch them on.

The book manuscript, print files, sales materials, and the `launch-src/`
launch kit (epub, revised manuscript, marketing copy, mockups) live alongside
this project locally and are deliberately excluded from version control via
`.gitignore` and from deploys via `.vercelignore`.
