# Prabhat Joshi — Portfolio

A single-file, dependency-free portfolio site (dark, glassmorphic, "developer console" theme). No build step required — it's plain HTML/CSS/JS, so it deploys anywhere that serves static files.

## Before you deploy — 3 quick edits

1. **GitHub & LinkedIn links** — open `index.html`, find this block near the bottom (inside the `<script>` tag) and replace with your real URLs:
   ```js
   const GITHUB_URL = "https://github.com/your-username";
   const LINKEDIN_URL = "https://linkedin.com/in/your-username";
   ```
2. **Resume file** — add your resume as `resume.pdf` in this same folder (same name, or update the `href="./resume.pdf"` in the Resume section).
3. **Contact form** — it currently opens the visitor's email app pre-filled to `joshiprabhat12@gmail.com` (no backend needed). If you'd rather have a real form backend, swap in a service like Formspree or Web3Forms and point the `<form>` action at it.

## Deploy (pick one — all free)

### Vercel (recommended)
1. Go to vercel.com → New Project → Import (or drag-and-drop this folder in the dashboard).
2. No build settings needed — it's a static site. Deploy.

### Netlify
1. Go to app.netlify.com/drop and drag this whole folder in.
2. Done — you get a live URL instantly.

### GitHub Pages
1. Push this folder to a GitHub repo.
2. Repo Settings → Pages → set source to the `main` branch, root folder.
3. Your site goes live at `https://your-username.github.io/repo-name`.

## Structure
```
portfolio/
├── index.html   # everything — markup, styles, and scripts in one file
├── resume.pdf   # add your resume here
└── README.md
```

## Customizing
- Colors, fonts, and spacing are all controlled by CSS variables at the top of the `<style>` block (`:root { --bg, --accent, --accent-2, ... }`).
- All content (projects, skills, experience) is plain HTML further down the file — search for the section you want (`<!-- PROJECTS -->`, `<!-- SKILLS -->`, etc.) and edit directly.
