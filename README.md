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
GitHub Pages serves the `gh-pages` branch, which holds the rendered site.

To update the live site after editing:

```bash
quarto publish gh-pages --no-prompt   # renders and uploads the site (1-2 min to go live)
git add -A && git commit -m "Update website" && git push   # saves the source files
```

`.github/workflows/publish.yml` (automatic publishing on push) is currently disabled on
GitHub because Actions is blocked by a billing lock on the account. Once that is resolved,
it can be re-enabled with `gh workflow enable publish.yml` (and Pages switched to
"GitHub Actions" as its source).
