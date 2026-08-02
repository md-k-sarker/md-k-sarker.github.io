# md-k-sarker.github.io

Personal academic website, built with [Jekyll](https://jekyllrb.com/) on the [al-folio](https://github.com/alshedivat/al-folio) v1.x theme. Deployed automatically to GitHub Pages via GitHub Actions on every push to `master`.

## Adding content

- **Publications** — add a BibTeX entry to [`_bibliography/papers.bib`](_bibliography/papers.bib). Use `pdf`, `html`, and `doi` fields for links; add `selected = {true}` to feature a paper on the home page.
- **Projects** — add a new Markdown file to [`_projects/`](_projects/), copying the front matter of an existing entry. `category` must be `Research` or `Software`.
- **Teaching** — add a new Markdown file to [`_teachings/`](_teachings/).
- **News** — add a new Markdown file to [`_news/`](_news/) (see existing files for the format).
- **CV** — edit [`_data/cv.yml`](_data/cv.yml). The downloadable PDF button on the CV page points to `assets/pdf/` (set in `_pages/cv.md`).

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>.

## Deployment

Pushing to `master` triggers [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml), which builds the site and publishes it via GitHub Pages (Settings → Pages → Source → "GitHub Actions").
