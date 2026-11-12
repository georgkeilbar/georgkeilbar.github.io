# Personal website — Georg Keilbar

A single-page academic website for GitHub Pages. No build step, no Jekyll.

## Publish

1. Create a public repository named `<your-github-username>.github.io`.
2. Upload `index.html`, `README.md` and `.nojekyll` to the root of the `main` branch.
3. In the repo go to **Settings → Pages**, set *Source* to "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute the site is live at `https://<your-github-username>.github.io`.

Command-line version:

```bash
git init && git add . && git commit -m "Personal website"
git branch -M main
git remote add origin https://github.com/<username>/<username>.github.io.git
git push -u origin main
```

## Edit

Everything lives in `index.html`. Sections are marked with `id="research"`, `id="publications"`, etc.

- **Add a paper:** copy an `<li>` block inside the relevant `<ul class="pub">`.
- **Add a PDF CV:** put `cv.pdf` in the repo and uncomment the link in the CV section.
- **Links:** the Google Scholar, LinkedIn and ResearchGate buttons currently point to name searches; replace them with your profile URLs (marked with a comment in the header).
- **Custom domain:** add a `CNAME` file containing your domain and configure DNS per GitHub's docs.
