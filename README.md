# aldaihanabdullah3.github.io

Static website for Abdullah Aldaihan. The site is plain HTML and CSS—no build tools, frameworks, or package managers.

## Layout

```
.
├── index.html           # Landing page with bio + selected publications
├── publications.html    # Detailed publication descriptions
├── assets/
│   └── css/style.css    # Global styles
├── images/              # Portraits or supporting imagery
└── files/               # Optional downloads (CV, papers, etc.)
```

## Developing locally

Use any static HTTP server, or just open the HTML files in your browser.

```powershell
python -m http.server 4000
```

Then browse to http://localhost:4000/.

## Deploying

Push to `main` and GitHub Pages deploys automatically via `.github/workflows/deploy.yml`. The workflow copies `index.html`, `publications.html`, and the `assets/`, `images/`, and `files/` directories into the published artifact.
