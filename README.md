# Terry Nyirenda — Portfolio Website

Modern, responsive portfolio for AI engineering work — built with plain HTML, CSS, and a small
amount of vanilla JS (no frameworks, no build step). Deploys free on GitHub Pages.

## Folder contents

```
Portfolio-Website/
├── index.html        # Single-page site
├── styles.css        # All styling (responsive + reduced-motion support)
├── script.js         # Mobile nav toggle + footer year
├── assets/
│   ├── profile.jpg   # Headshot
│   ├── resume.pdf    # Downloadable resume
│   ├── icons/        # Contact icons (SVG)
│   └── projects/     # Project screenshots (thumbnails)
└── README.md
```

## Editing

- **Content:** edit `index.html`. Projects live in `.project-card` blocks; duplicate one to add
  a project (also add a screenshot under `assets/projects/` and reference it in `.project-media`).
- **Styling:** CSS custom properties at the top of `styles.css` control theme colors and fonts.
- **Images:** keep thumbnails ~16:9 (the `.project-media` ratio) for consistent cards.

## Deploying to GitHub Pages (free)

1. Create a repo named `Terrytd0.github.io` on GitHub (public).
2. In your local repo folder run:
   ```
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/Terrytd0/Terrytd0.github.io.git
   git push -u origin main
   ```
3. In the repo on GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root)** → Save.
4. Your site is live at `https://terrytd0.github.io`.

After the first push, any future `git push` updates the live site automatically.

## Preview locally

Open `index.html` directly in a browser (double-click), or run a local server:

```
python -m http.server 8000
```

then visit `http://localhost:8000`.
