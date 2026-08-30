# The Christ Frequency — Landing Page

Landing page for *The Christ Frequency* by Gideon George, offering the free
7-day starter guide and collecting email signups.

## Contents

- `index.html` — the full single-file landing page (styles and scripts inline)
- `privacy.html` — privacy policy, linked from the footer
- `tcf-cover.jpg` — cover image shown in the hero
- `tcf-cover-small.jpg` — smaller cover variant, served to phones
- `og-card.jpg` — 1200×630 social share image
- `og-card.src.html` — the page that image is rendered from
- `favicon.svg`, `apple-touch-icon.png` — browser tab and home-screen icons
- `robots.txt`, `sitemap.xml` — crawl directives and the two-page sitemap

## Local preview

Open `index.html` directly in a browser, or serve the folder:

```bash
python -m http.server 8000
```

## Social share image

`og-card.jpg` is what Facebook, X, LinkedIn and WhatsApp show when the page is
shared. It is 1200×630 because they all crop to that ratio; the square cover on
its own lost the top and bottom of the book.

To rebuild it after a headline or cover change, open `og-card.src.html` in a
browser at exactly 1200×630 and export, or render it headless — the file's
opening comment has the command. Its colours and type are copied from
`index.html`, so keep the two in step.

Anything cached by a social network needs re-scraping before the new image
shows: Facebook's Sharing Debugger and LinkedIn's Post Inspector both force it.

## Notes

Analytics and pixel snippets (GA4, Meta) are present in `index.html` as
commented-out placeholders — drop in your IDs to switch them on.

The book manuscript, print files, sales materials, and the `launch-src/`
launch kit (epub, revised manuscript, marketing copy, mockups) live alongside
this project locally and are deliberately excluded from version control via
`.gitignore` and from deploys via `.vercelignore`.
