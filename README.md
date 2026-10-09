# Chloe Chan — Personal site

A static personal site for Chloe Chan, MSc Marketing candidate at HKU.
Editorial-minimal design, single page, fully self-contained.

## Live

Hosted on GitHub Pages:
`https://<your-username>.github.io/<repo-name>/`

## Files

```
.
├── index.html            # The whole site (HTML + inlined CSS + JS)
├── README.md             # This file
└── assets/
    └── profile.png       # Headshot, 720×720, ~340 KB
```

That is the whole project. No build step, no dependencies.

## Tech

- HTML5 with semantic structure (`section`, `article`, `nav`, `header`, `footer`)
- CSS custom properties for theming
- `IntersectionObserver` for subtle fade-in on scroll
- Web fonts: Source Serif 4 (serif) + Inter (sans) via Google Fonts
- Responsive down to ~360 px width

## Local preview

Open `index.html` directly in any modern browser, or run a quick static server:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy — drag and drop to GitHub Pages

1. Create a new repository on github.com.
   - For a user-page URL, name it `<username>.github.io`.
   - Otherwise any name works; URL becomes `<username>.github.io/<repo>`.
2. On the repo page, click **Add file ▾ → Upload files**.
3. Drag the three files into the upload box. GitHub will preserve the `assets/` folder structure.
4. Commit with a message like `Initial site`.
5. Go to **Settings → Pages**:
   - **Source:** Deploy from a branch
   - **Branch:** `main` · **Folder:** `/ (root)`
   - Save
6. Site is live within 1–3 minutes.

## Updating content

- Edit `index.html` locally with any text editor.
- Re-upload via the same drag-and-drop flow (or commit through GitHub's web editor).
- GitHub Pages rebuilds automatically, usually within 30 seconds.

## Notes

- All copy is based on Chloe Chan's CV (as of October 2026). Update
  the experiences section as new roles are added.
- Photo: replace `assets/profile.png` with a new headshot (recommend
  square, ≥720 px, ≤500 KB) — keep the filename to avoid changing the path.
- To switch palettes, edit the `:root { --bg, --fg, --accent, ... }` block at
  the top of `index.html`.
