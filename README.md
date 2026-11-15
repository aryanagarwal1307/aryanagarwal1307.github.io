# Aryan Agarwal

A minimal personal website at <https://aryanagarwal1307.github.io/>. Plain HTML and CSS, with no JavaScript, external fonts, dependencies, or build step.

## Repository structure

- `index.html` — page content and document metadata.
- `assets/css/styles.css` — typography, colors, spacing, and responsive layout.
- `assets/favicon.svg` — browser tab icon.
- `.nojekyll` — tells GitHub Pages to serve the static files directly.

Future sections such as About, Research, Publications, CV, and Contact can be added inside the existing `<main>` element, with their styles in the same stylesheet. No future sections are included yet.

## Edit in VS Code

1. Open this repository folder in VS Code and stay on the `main` branch.
2. Edit `index.html` for content or `assets/css/styles.css` for appearance, then save.
3. Open `index.html` in your browser to preview. Optionally, run `python3 -m http.server 8000` from VS Code's terminal and visit <http://localhost:8000/>. Press Ctrl+C to stop the server.
4. Review the changes in VS Code's Source Control panel, stage the intended files, enter a commit message, commit, and choose **Push** (or **Sync Changes**).

The equivalent terminal commands are:

```sh
git add index.html assets/css/styles.css
git commit -m "Update personal website"
git push origin main
```

Include other edited files in `git add` when needed. GitHub authentication is required to push.

## Deployment

The repository must be named `aryanagarwal1307.github.io` to use the root URL above. In GitHub, go to **Settings → Pages → Build and deployment** and use:

- **Source:** Deploy from a branch
- **Branch:** `main`
- **Folder:** `/(root)`

After this one-time setup, every push to `main` automatically publishes the files at the website URL. No custom workflow is needed. Check the repository's **Actions** tab for the `pages build and deployment` result, and **Settings → Pages** for the live URL. Publishing may take a few minutes.
