# maruf-lawal.github.io

Personal academic website of Maruf A. Lawal, live at https://maruf-lawal.github.io.
Built with Jekyll and the [al-folio](https://github.com/alshedivat/al-folio) theme.

**How it publishes:** every change to `main` runs the "Deploy site" GitHub Action, which builds the site and pushes the result to the `gh-pages` branch. GitHub Pages serves `gh-pages` (Settings → Pages → Source: *Deploy from a branch*, branch `gh-pages`, folder `/ (root)`). A build takes about 3–5 minutes; check the **Actions** tab if a change does not appear.

## How to update the site

Edit a file on GitHub (pencil icon), then commit. The table says which file holds what.

| To change...                              | Edit this file                                  |
|-------------------------------------------|-------------------------------------------------|
| Papers (journal, preprint, under review)  | `_bibliography/papers.bib`                      |
| Badge colour/link for a journal           | `_data/venues.yml`                              |
| Home page text                            | `_pages/about.md`                               |
| News on the home page                     | add a file to `_news/` (see below)              |
| Research page                             | `_pages/research.md`                            |
| Software & data page                      | `_pages/software.md`                            |
| Talks and workshops                       | `_pages/talks.md` (Markdown tables)             |
| Teaching philosophy and courses           | `_pages/teaching.md`                            |
| CV page content                           | `_data/cv.yml`                                  |
| Downloadable CV                           | replace `assets/pdf/Maruf_Lawal_CV.pdf` (same name) |
| Email, ORCID, Scholar, GitHub, LinkedIn   | `_data/socials.yml`                             |
| Name, site description, theme options     | `_config.yml`                                   |
| Theme colour                              | `_sass/_themes.scss` (`--global-theme-color`)   |

### Adding a paper

Copy an entry in `_bibliography/papers.bib` and edit it.

- Entry type decides the section: `article` = journal article, `misc` = preprint (put the server in `howpublished`), `unpublished` = under review.
- `abbr = {...}` is the coloured badge; add the same name to `_data/venues.yml` to set its colour.
- `selected = {true}` also lists the paper on the home page.
- `doi`, `pdf`, `code`, `html` add buttons. `bibtex_show = {true}` adds a "Bib" button.
- Your name is underlined automatically when written `Lawal, M. A.`.
- Only list work once it is submitted.

### Adding a news item

Create `_news/YYYY-MM-DD-news.md` (the date is when it happened):

```
---
layout: post
date: 2026-12-15
inline: true
related_posts: false
---

Graduated with a Ph.D. in Mathematics from the University of Tennessee, Knoxville.
```

If you only know the month, add `display_date: Dec 2026` under `inline: true`. The home page shows the six most recent items.

### Profile photo

Add a square photo as `assets/img/prof_pic.jpg`, then in `_pages/about.md` set `image: prof_pic.jpg` under `profile:`.

### When the PhD is conferred (December 2026)

1. `_pages/about.md`: change the `subtitle:` line and the first sentence of the bio.
2. `_data/cv.yml`: change `label:` and the Ph.D. "Expected December 2026" line.
3. Add a news item; upload the new CV PDF.
4. If your email changes: `_data/socials.yml` and `_data/cv.yml`.

## Local customizations of the theme

Most layouts come from the `al_folio_core` gem. Three files override it locally:

- `_sass/_themes.scss`: theme colour set to deep teal.
- `_includes/news.liquid`: supports `display_date` on news items.
- `_includes/hook/bib.liquid`: shows the preprint server for `misc` entries.

## Previewing locally (optional)

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000. The theme's own documentation is in `docs/`.
