<p align="center">
  <img src="assets/memos.png" width="80" height="80" alt="leolune.fun icon">
</p>

<h1 align="center">leolune.fun</h1>

<p align="center">A little collection of things I've made.</p>

<p align="center">
  <a href="https://leolune.fun/">Open the collection</a> ·
  <a href="https://leolune.com/">Portfolio</a> ·
  <a href="#run-locally">Run locally</a>
</p>

## Small things, made to be opened

- **Find something useful.** Browse web apps, tools, and games, or search for a project by name.
- **Take a closer look.** Open a project for its story, features, screenshots, and useful details.
- **Explore the images.** Scroll through available galleries and open an image for a larger, caption-free view. Use the arrows, thumbnails, keyboard, or a swipe to move between images.
- **Try it here.** Load a live preview when available. Close it when you're finished, or open the app in its own tab.
- **Follow the source.** Each project links to its GitHub repository.
- **Browse comfortably.** The collection adapts to phone and desktop screens and respects reduced-motion preferences.

## Get started

1. [Open leolune.fun](https://leolune.fun/).
2. Choose **Apps**, **Tools**, or **Games**, or use search to narrow the collection.
3. Select a project to explore its details and available images.
4. Choose its **Open** button to launch it, or **Load preview** to take a look within the collection.

## About the collection

This repository is the collection website. The individual apps and games live in their own repositories and have their own storage, permissions, and deployment arrangements.

Live previews load those websites in an embedded frame. Some apps cannot be embedded, and features such as microphone access or downloads may need a separate tab. Closing a preview unloads it.

Project links use URL fragments, so you can share a specific entry directly—for example, [FallingBlocks](https://leolune.fun/#fallingblocks).

## Run locally

Use Python 3 to serve the static files.

```sh
git clone https://github.com/leolunelove/leolune-fun.git
cd leolune-fun
python3 -m http.server 8000
```

Open [localhost:8000](http://localhost:8000/). There is no dependency installation or build step. Edit the source files and reload the page to see changes.

## Repository guide

| Path | Purpose |
| --- | --- |
| [index.html](index.html) | Page structure, navigation, search, and project dialog |
| [projects.js](projects.js) | Project descriptions, links, features, and gallery entries |
| [app.js](app.js) | Filtering, project navigation, image viewer, and live previews |
| [style.css](style.css) | Layout, colours, responsive styles, and motion |
| [assets/](assets/) | Project icons and gallery images |
| [sculpture.webp](sculpture.webp) | Site artwork |
| [CNAME](CNAME) | Custom domain for GitHub Pages |
| [.nojekyll](.nojekyll) | Serve the static files without Jekyll processing |

GitHub Pages hosts [leolune.fun](https://leolune.fun/). Keep the site files at the repository root and preserve `CNAME` when updating the site. When changing scripts or styles, update their version query strings in `index.html` so returning visitors receive the new files.

## Built with

HTML, CSS, and vanilla JavaScript, with native browser dialogs and WebP gallery images. The website runs directly in the browser and is hosted on GitHub Pages.
