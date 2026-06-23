# Portfolio Website

Portfolio is built as a static site and hosted on GitHub Pages.

🔗 **Live site:** [tyjihn.github.io](https://tyjihn.github.io)

## Overview

A responsive single-page portfolio with a dedicated project page, covering:

- **Home** — introduction and header section
- **About** — background, education, and skills (tabbed)
- **Projects** — featured work, including *Reflexion*
- **Contact** — social links and a contact form

## Featured Project

**[Reflexion](reflexion.html)** — a 2D top-down puzzle game built in C++ with OpenGL and SDL2, featuring clone-based movement, three levels of increasing difficulty, shader-based visual effects, and audio via SDL_mixer.

Originally developed as a native desktop build, the game is made playable in the browser by compiling the C++/OpenGL/SDL2 source to WebAssembly with [Emscripten](https://emscripten.org/), which maps the desktop OpenGL calls to WebGL and runs the game on an HTML5 base. The web build was first compiled and tested locally before being deployed to GitHub Pages.

- [Play the game](https://tyjihn.github.io/reflexion)
- [View source code](https://github.com/Tyjihn/reflexion)

## Tech Stack

- **HTML5** — page structure and content
- **CSS3** — styling and responsive layout (`style.css`)
- **JavaScript** — mobile nav menu, tabbed About section, and contact form submission
- **Google Apps Script** — contact form backend (submissions to Google Sheets)

## Project Structure

```
├── index.html        # Main page (Home, About, Projects, Contact)
├── reflexion.html    # Reflexion project detail page
├── style.css         # Site styles
└── assets/
    ├── reflexion_levels.gif
    └── reflexion_demo.mp4
```

## Running Locally

No build step required. Clone the repo and open `index.html` in a browser, or serve it locally:

```bash
git clone https://github.com/Tyjihn/tyjihn.github.io.git
cd tyjihn.github.io
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deployment

Hosted on **GitHub Pages**. Pushing to the `main` branch publishes the site automatically.

## Contact

- **LinkedIn:** [LinkedIn Profile](https://www.linkedin.com/in/lucy-zheng-93b03a294)
- **GitHub:** [@Tyjihn](https://github.com/Tyjihn)
