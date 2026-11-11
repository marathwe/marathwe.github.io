# Personal academic website

Built with [Quarto](https://quarto.org).

## Preview locally

```bash
quarto preview
```

## Where to edit what

| What | File |
|---|---|
| Name, sidebar links, email/GitHub/Scholar icons | `_quarto.yml` |
| Home page (bio, photo, news) | `index.qmd` |
| Research interests, projects, presentations | `research.qmd` |
| Publications, working papers, theses | `data/papers.yml` (one entry per paper) |
| Teaching | `teaching.qmd` |
| CV | replace `files/CV_Weber.pdf` (keep the same name) |
| PDFs (papers, appendix, syllabi) | put them in `files/` |
| Colours and fonts | `styles.scss` (light), `styles-dark.scss` (dark mode) |

## Publishing

The site lives at **https://marathwe.github.io** (repo `marathwe/marathwe.github.io`).
Every push to `main` rebuilds and publishes it automatically via GitHub Actions
(`.github/workflows/publish.yml`). It usually takes 1–2 minutes.

```bash
git add -A
git commit -m "Update website"
git push
```
# marathwe.github.io
