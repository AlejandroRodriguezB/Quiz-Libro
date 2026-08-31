# Quiz Libro - Setup Guide

This project is a static HTML/CSS/JS quiz.
## Project structure

```text
Quiz-Libro/
├── index.html
├── styles.css
├── files/
│   ├── books-data.json
│   ├── audio/
│   └── img/
│       ├── covers/
│       └── others/
├── pkmn-font.ttf
├── ico.svg
└── README.md
```

## Quick start

From the project root, run a local static server:

```bash
python -m http.server 8000
```

Then open in the browser:

```text
http://localhost:8000
```

## Required assets

Make sure these files exist in the right folders:

### Book covers

Folder: `files/img/covers/`

The app loads cover images by ISBN, for example:

```text
files/img/covers/9788491040255.webp
```

### Background / decoration images

Folder: `files/img/others/`

These are used for the background and text borders, such as:
- dreambackloop.png
- dreamfrontloop.png
- pmdtextbox.png

### Audio

Folder: `files/audio/`

Optional files:
- quiz-music.ogg
- click-sound.mp3

### Fonts and favicon

Files in the project root:
- pkmn-font.ttf
- ico.svg

## Notes about the current app

- The app is plain HTML loaded directly in the browser.
- CSS is in `styles.css` and linked from `index.html`.
- The questions, books, and language texts are stored in JSON files under `files/lang/en/`.
- The book list is hardcoded in `index.html`.
- No build step is required for normal local use.

## Deployment

Since this is a static site, you can deploy it to any static host:

- GitHub Pages
- Netlify
- Vercel
- Any simple static hosting service

Upload the project root as-is and keep the `files/` folder intact.

## Summary

This project is ready to run as a static site with no install step. Just serve the folder and open the local URL in a browser.
