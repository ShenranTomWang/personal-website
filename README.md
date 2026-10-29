# Shenran Wang — personal website

A responsive academic portfolio built with HTML, CSS, and a small JavaScript enhancement. No build step or npm dependencies.

## Preview locally

With Node.js and Python 3 installed:

```sh
npm run dev
```

Open http://127.0.0.1:5173. Alternatively, run `python3 -m http.server 5173 --directory dist --bind 127.0.0.1`.

## Connect to GitHub

Create an empty repository under **ShenranTomWang**, then run the following from this folder, replacing YOUR-REPOSITORY with its name:

```sh
git remote add origin https://github.com/ShenranTomWang/YOUR-REPOSITORY.git
git push -u origin main
```

In the repository's **Settings → Pages → Build and deployment**, select **GitHub Actions**. Run the included **Deploy to GitHub Pages** workflow from the Actions tab if the initial push happened before Pages was enabled. Later pushes to `main` deploy automatically.

For a root website, name the repository `ShenranTomWang.github.io`; it will be available at https://ShenranTomWang.github.io/. Other names use a repository subpath; all local asset URLs are relative and support either option.

## Edit content

- `dist/index.html`: biography, publications, education, experience, links.
- `dist/styles.css`: layout, colors, typography, and mobile breakpoints.
- `dist/assets/portrait.jpg`: supplied portrait, cropped visually with CSS.
- `dist/assets/resume.pdf`: supplied downloadable research resume.
- `dist/script.js`: automatic copyright year.

Content and publication status reflect the supplied resume as of October 2026. Update the ongoing projects and review status as they change. The site uses Google Fonts with system fallbacks; the page remains usable when fonts are unavailable.

The original portrait and resume are included in the repository. Publishing the repository or website makes those assets accessible to visitors. Remove the resume link and file if you prefer to share only the website summary.

## Validation

```sh
npm run check
```

The GitHub Pages workflow publishes `dist/` directly. No server, API keys, database, or hosting configuration is needed locally.
