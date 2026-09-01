# Quiz Libro

A browser-based personality quiz that matches your answers to a book recommendation. It follows the same idea as the classic PMD personality tests, but with a curated set of books and a custom visual style.

## About

This project is a static web app built in plain HTML, CSS and JavaScript. The quiz asks a series of personality questions, scores your answers, and then recommends a book based on the trait profile that best matches you.

## Features

- 2 modes:
  - normal mode: 10 random questions
  - full mode: all questions
- responsive layout for desktop and mobile
- custom background and UI styling
- result screen with cover, title, author and ISBN
- personality radar chart
- static data-driven structure using JSON files

## Project structure

```text
Quiz-Libro/
├── index.html
├── styles.css
├── files/
│   ├── audio/
│   └── img/
│       ├── covers/
│       └── others/
├── README.md
├── SETUP.md
├── pkmn-font.ttf
├── ico.svg
└── .gitignore
```

## Run locally

From the project root:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Assets required

### Covers

Place the book covers in:

```text
files/img/covers/
```

Files are loaded by ISBN, for example:

```text
files/img/covers/9788491040255.webp
```

### UI images

Place decorative assets in:

```text
files/img/others/
```

Common ones include:
- dreambackloop.png
- dreamfrontloop.png
- pmdtextbox.png

### Audio

Optional audio files can go in:

```text
files/audio/
```

## How it works

1. The user answers a set of questions.
2. Each answer adds points to personality traits.
3. The app normalizes the scores.
4. It picks the trait with the highest weight.
5. The result screen shows a matched book based on that personality.

## Files of interest

- [index.html](index.html) — full app logic and question data
- [styles.css](styles.css) — styling, layout and UI behavior
- [SETUP.md](SETUP.md) — setup and asset instructions

## Notes

This repo is intentionally a static app and does not require a package install or build process.

## License

This project is distributed for personal and educational use. Check the repository license if present in your fork.

## Acknowledgements

- Inspired by PMD-style personality tests
- Book list and visual direction adapted for this project
