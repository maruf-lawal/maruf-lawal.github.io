# maruf-lawal.github.io

Personal academic website of Maruf Lawal, live at https://maruf-lawal.github.io.
Built with Jekyll on the AcademicPages theme and published automatically by GitHub Pages whenever `main` changes.

## How to update the site

Almost everything is kept in short YAML lists in the `_data/` folder. To add an item, open the file on GitHub, click the pencil icon, copy an existing block, edit it, and commit. The site rebuilds in a minute or two.

| To change...                         | Edit this file                 |
|--------------------------------------|--------------------------------|
| Papers (published, preprints, under review) | `_data/publications.yml` |
| Datasets, code, benchmarks           | `_data/software.yml`           |
| Talks                                | `_data/talks.yml`              |
| Workshops / boot camps               | `_data/workshops.yml`          |
| Courses taught                       | `_data/teaching.yml`           |
| Homepage news (first 6 shown)        | `_data/news.yml`               |
| Header menu                          | `_data/navigation.yml`         |
| Homepage text                        | `_pages/about.md`              |
| Research page                        | `_pages/research.md`           |
| Teaching philosophy                  | `_pages/teaching.html`         |
| CV page summary                      | `_pages/cv.md`                 |
| Sidebar (title line, email, links)   | `author:` section of `_config.yml` |
| Profile photo                        | replace `images/profile.png` (square image) |
| CV PDF                               | replace `files/Maruf_CV.pdf` (keep the same name) |

### Notes

- **YAML formatting:** keep the two-space indentation and put text in double quotes. If a title contains a double quote, use single quotes around it instead.
- **Your name is bolded automatically** in publication author lists when written as `M. A. Lawal`.
- **Paper status:** use `status: published`, `preprint`, or `under-review`; the Publications page sorts them into sections. Only list work once it is submitted.
- **Links in news items** use Markdown: `[text](https://...)`; italics use `*text*`.

### When the PhD is conferred (December 2026)

1. `_config.yml`: change the `bio:` line (e.g. "Ph.D. in Mathematics, University of Tennessee...") and, if it changes, `employer:` and `email:`.
2. `_pages/about.md` and `_pages/cv.md`: change "Ph.D. candidate ... expected December 2026".
3. Add a news item in `_data/news.yml`.
4. Upload the new CV as `files/Maruf_CV.pdf`.

## Previewing locally (optional)

```
bundle install
bundle exec jekyll serve
```
Then open http://localhost:4000.
