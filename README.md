# Task-1-GitHub-Link-Android-Club-Website

# Android Club VIT Bhopal — Club Showcase  
A clean, responsive, single-file website to showcase the Android Club at VIT Bhopal. Built with semantic HTML, modern CSS (glass + gradients), and vanilla JavaScript — no build tools or frameworks needed.

## Features

- ⚡ Single-file app (index.html) — copy, run, ship
- 🎯 Sticky navbar + smooth scrolling
- 🧭 Mobile menu (hamburger) with accessible aria attributes
- 🧪 Projects grid with category filters (All/Android/Compose/UI-UX/ML)
- 🗓️ Events timeline with status pills
- ✉️ Contact form (client-side demo) + success toast
- 🎞️ Subtle scroll animations (IntersectionObserver)
- ⬆️ Back-to-top floating button
- ♿ Accessibility aware (semantic tags, aria labels, reduced-motion support)
- 📱 Fully responsive (desktop → tablet → mobile)

---

## Tech Stack

- HTML5
- CSS3 (custom properties, responsive grid, glassmorphism)
- Vanilla JavaScript (no dependencies)

---

## Quick Start

Option A — Double click:
1. Download/clone the repo
2. Open `index.html` in your browser

Option B — Run a tiny local server (recommended for testing):
- Python 3:
  ```bash
  python3 -m http.server 8080

Visit http://localhost:8080

Node (serve):
Bash

npx serve .
Visit the printed URL
Project Structure
This repo is intentionally minimal:

text

.
├─ index.html          # All HTML, CSS, and JS in one file
├─ README.md           # This file
└─ screenshot.png      # Optional screenshot for README
Customize It
All edits happen in index.html.

Branding

Title and meta: <title> and <meta name="description">
Header brand text: .brand → “Android Club VITB”
Primary accent color: in :root — --accent: #3ddc84
Hero Section (Welcome)

Update headings and paragraph inside #welcome
CTA links point to sections via #projects, #events, #contact
About Section

Change “Our Mission”, stats, and bullet list under #about
Projects

Each project card is an <article class="project" data-cat="android,compose">
Categories available by default: android, compose, uiux, ml
To add a project, duplicate a card and update:
.thumb text (project name)
<h3> title and description
Links (GitHub, Demo)
data-cat with one or more categories (comma-separated)
Filters

Add/remove chips in .filters with data-filter="your-category"
Ensure project data-cat contains the same category tokens
Events

Each event is a .event block inside #events .timeline
Update the date, title, description, and status pill (Upcoming/Past)
Contact

Form is a demo (shows a toast + alert). Replace with your backend/form service if needed.
Update the email button: mailto:androidclub@vitbhopal.ac.in
Update social links under “Find us online”
Animations

Reveal-on-scroll uses IntersectionObserver
Respects prefers-reduced-motion. No action needed.
Deploy
GitHub Pages (fastest)
Push index.html and README.md to a GitHub repo
Go to Settings → Pages
Source: “Deploy from a branch”
Branch: main (or master), Folder: /root
Save — wait 1–2 minutes for your Pages URL
Update the “Live Demo” link at the top of this README
Netlify
Drag-and-drop the repo folder onto https://app.netlify.com/drop
Or connect your Git repo and select the root as the publish directory
Vercel
Import the Git repo at https://vercel.com/new
Framework preset: “Other”
Output directory: root
Accessibility & Performance Notes
Uses semantic HTML (header, main, section, nav, footer)
Buttons and links have clear labels, ARIA where needed
Smooth scrolling disabled if user prefers reduced motion
Minimal JS, no external runtime dependencies -> fast load
Customize color contrast in :root if needed for your theme
Submission Checklist (for the challenge)
 Code in a GitHub repo
 Live deployed link (GitHub Pages/Netlify/Vercel)
 README with setup and customization instructions
 Placeholder text/links replaced where possible
 Clean, responsive design with multiple sections:
Welcome, About, Projects, Events, Contact
FAQ
Can I split the single file into multiple files?

Yes. This starter is single-file by design, but you can extract CSS/JS when needed.
How do I change the green accent?

In :root, edit --accent: #3ddc84;.
How do filters work?

Chips have data-filter="compose" etc. Project cards declare categories in data-cat="android,compose". The tiny JS toggles visibility.
License
MIT — feel free to reuse and adapt. Consider giving credit to the Android Club VIT Bhopal showcase starter.

Credits
Android green accent color: #3ddc84
Built for the Android Club VITB frontend challenge