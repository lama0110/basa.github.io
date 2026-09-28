# BASA project page

Static GitHub Pages website for **Backend-Agnostic Sparse Attention for Fast High-Resolution Visual Generation**.

The page is currently configured for the anonymous ICLR 2027 submission: author names are hidden and the Code / arXiv buttons are intentionally disabled.

## Preview locally

```bash
cd BASA_project_page
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy to GitHub Pages

1. Create a GitHub repository and copy the contents of this folder to the repository root.
2. Push to `main`.
3. Open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main`, and use `/ (root)`.
5. GitHub will publish the site at the Pages URL shown in Settings.

If the repository itself is named `<username>.github.io`, the site will be served directly from `https://<username>.github.io/`.

## What to update before public release

Search `index.html` for the hero buttons and replace the disabled **Code** / **arXiv** elements with real `<a>` links. Update `Anonymous Authors`, the venue status, and the BibTeX block after deanonymization. If you have a custom domain, add a `CNAME` file containing the domain name.

> **Double-blind note:** the manuscript is currently marked as an anonymous ICLR 2027 submission. Before publishing any author-identifying repository/page during review, confirm that doing so is compatible with the conference's anonymity policy.

## Structure

```text
BASA_project_page/
├── index.html
├── .nojekyll
├── README.md
└── assets/
    ├── BASA_paper.pdf
    ├── favicon.svg
    ├── css/style.css
    ├── js/main.js
    └── images/
```

All figures and qualitative examples in `assets/images/` are derived from the supplied manuscript PDF.
