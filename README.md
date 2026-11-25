# Qays Judge: weather × machine learning portfolio

Everything lives in `index.html`: styles, scripts, map data and a small bundled copy of d3-geo. The only external request is Google Fonts (IBM Plex), and the page falls back to system fonts without it.

## Publish on GitHub Pages

1. Create a public repository and upload `index.html` (and the `logos` folder, below) to the root.
2. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
3. The site appears at `https://<username>.github.io/<repo>/` within a minute or two.

## Logos

The About timeline looks for three image files and shows initials until they exist:

```
logos/cambridge.png
logos/dv-trading.png
logos/balyasny.png
```

Square images work best (they sit in a 44px circle on a white background).

## Editing

- **Copy:** each project's Aim, Methodology, Results and interactive-model explanation are plain HTML inside `#monsoon`, `#floods` and `#subseasonal`.
- **Scroll-reveal timing:** each `.reveal-text` element has `data-start` and `data-end`, which set where the word-by-word reveal begins and ends within its pinned section.
- **Globe region profiles:** the `PROFILES` object.
- **Interactive models:** simulated to illustrate each method, not replays of real model output.
