# On hold (not published)

Content taken off the website in November 2026 until some open issues are resolved.
Jekyll ignores folders whose names start with an underscore, so nothing here is on the site.

To restore:

1. `software.md` -> move back to `_pages/software.md` (adds the Software & Data page and menu item).
2. `preprint.bib` -> move the entry back into `_bibliography/papers.bib`, and remove the
   `{% comment %}` tags around the Preprints section in `_pages/publications.md`.
3. `_pages/research.md`, end of the "Sexually transmitted infections" paragraph, add back:
   Building on these models, I assembled an [open state-level syphilis and chlamydia panel]({{ '/software/' | relative_url }}) for 2000–2024 and used it to score, state by state, how well published transmission models predict years they were not fitted to.
4. `_pages/about.md`, second paragraph: change "..., and an ensemble forecasting approach that won the 2026 _Modeling the Invisible_ forecasting competition." back to
   "..., an ensemble forecasting approach that won the 2026 _Modeling the Invisible_ forecasting competition, and an open state-level surveillance panel for benchmarking STI transmission models."
5. News item (file `_news/2026-10-29-news.md`, with `display_date: Oct 2026`):
   Released the [U.S. State Syphilis and Chlamydia Panel and Model Validation Benchmark](/software/) (v1.0.0) on GitHub and Zenodo, with an accompanying preprint.
6. `_data/repositories.yml`: add `maruf-lawal/us-sti-state-panel` under `github_repos`.
