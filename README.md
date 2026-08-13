# Sibiyon S — Portfolio

A single-page, self-contained personal portfolio website for **Sibiyon S**, Computer Science & Engineering graduate (SASTRA Deemed University), focused on Software Development and AI/ML.

**Live Site:** [https://sibiyon-s-portfolio.onrender.com](https://sibiyon-s-portfolio.onrender.com)

---

## Overview

This portfolio presents an overview of Sibiyon S's education, technical skills, projects, and certifications through a modern glassmorphism design with light/dark theme support.

## Features

- **Light & Dark theme toggle** — switch instantly via the sun/moon button in the navbar
- **Glassmorphism UI** — frosted glass panels with soft blur and layered background accents
- **Fully responsive** — works across desktop, tablet, and mobile, with a dedicated mobile menu
- **Smooth in-page navigation** — JS-driven scrolling between sections (About, Skills, Work, Experience, Education, Contact)
- **Downloadable resume** — resume PDF is embedded directly in the page for one-click download
- **Scroll-reveal animations** — sections fade/slide into view as you scroll
- **Zero dependencies** — no build step, no external JS framework; pure HTML, CSS, and vanilla JavaScript

## Sections

| Section | Description |
|---|---|
| Hero | Name, role, short intro, quick stats |
| About | Bio and quick facts (degree, focus area, minor, languages) |
| Skills | Categorized technical skills (Programming, Databases, AI/ML, Data Processing, Explainable AI, Web & Deployment) |
| Work | Featured projects — Explainable AI for Deepfake Voice Detection, Dysarthric Speech Recognition |
| Experience | Timeline of major project work and education |
| Education | Academic background |
| Certifications | Courses, workshops, and quiz participation |
| Contact | Email, phone, LinkedIn, and GitHub |

## Tech Stack

- HTML5
- CSS3 (custom properties / CSS variables for theming, no framework)
- Vanilla JavaScript (theme toggle, scroll navigation, scroll-reveal via `IntersectionObserver`)
- Google Fonts — [Sora](https://fonts.google.com/specimen/Sora) & [Inter](https://fonts.google.com/specimen/Inter)

## Project Structure

```
├── index.html      # Single-file site (HTML + inline CSS + inline JS)
└── README.md        # This file
```

The resume PDF is embedded inside `index.html` as a base64 data URI, so the site works as a single file with no external assets to manage.

## Running Locally

No build tools or dependencies required.

```bash
# Clone or download the repository, then simply open the file:
open index.html        # macOS
start index.html        # Windows
xdg-open index.html      # Linux
```

Or serve it with any static file server, e.g.:

```bash
npx serve .
```

## Deployment

The live site is deployed on [Render](https://render.com) as a static site:

**https://sibiyon-s-portfolio.onrender.com**

To redeploy your own copy on Render:
1. Push this repository to GitHub
2. Create a new **Static Site** on Render and connect the repo
3. Leave the build command empty and set the publish directory to the project root
4. Deploy

## Customization

- **Contact links** (LinkedIn, GitHub, email, phone) — update the `href` values inside the `#contact` section of `index.html`
- **Project links** — update the `View on GitHub →` links inside the `#work` section
- **Resume** — replace the embedded base64 PDF with your own by re-encoding a new resume and swapping the `data:application/pdf;base64,...` string on the resume buttons
- **Theme colors** — adjust the CSS custom properties under `:root`, `html[data-theme="light"]`, and `html[data-theme="dark"]`

## Author

**Sibiyon S**
Computer Science & Engineering Graduate — SASTRA Deemed University
[LinkedIn](https://www.linkedin.com/in/sibiyon-s-09871a322/) · [GitHub](https://github.com/SibiyonS)

## License

This project is personal portfolio content. Feel free to reference the structure/design for your own portfolio, but please do not reuse the personal content (name, resume, project details) as your own.
