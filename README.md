# Dr. Sakirman — Academic Website

Static academic website designed for GitHub Pages at `https://sakir-man.github.io/`.

## Structure

- `index.html` — homepage
- `research/` — research roadmap
- `publications/` — filterable publication list
- `teaching/` — teaching portfolio
- `service/` — academic and community service
- `cv/` — curriculum vitae
- `assets/css/style.css` — global visual design
- `assets/js/` — navigation, animations, publication filtering
- `assets/data/publications.json` — publication database
- `assets/img/profile.svg` — temporary profile image

## How to publish

1. Back up the current `sakir-man.github.io` repository.
2. Remove the old Jekyll theme files from the repository root.
3. Upload the contents of this package to the repository root.
4. Keep `.nojekyll` in the root.
5. Commit and push to the branch used by GitHub Pages (normally `main`).
6. In **Settings → Pages**, ensure the source is **Deploy from a branch**, `main`, `/ (root)`.
7. Open `https://sakir-man.github.io/` after deployment.

## Replace the profile image

The website works immediately with `assets/img/profile.svg`.
To use your real portrait:

1. Put the portrait at `assets/img/profile.jpg`.
2. Replace all occurrences of `profile.svg` in the HTML files with `profile.jpg`.

Recommended image: square or portrait, at least 1000 × 1000 px.

## Update publications

Edit `assets/data/publications.json`.
Each record contains:

```json
{
  "year":"2026",
  "type":"journal",
  "title":"Article title",
  "venue":"Journal title",
  "authors":"Author names",
  "url":"https://doi.org/..."
}
```

The Publications page automatically supports search and filtering.

## Important review items

Before final deployment, confirm:

- current academic leadership title in the Doctoral Program;
- whether to display `Dr. Sakirman, M.S.I.` or `Dr. Sakirman, S.H.I., M.S.I.` consistently;
- a current portrait;
- additional publications and DOI links;
- downloadable PDF CV, if desired.
