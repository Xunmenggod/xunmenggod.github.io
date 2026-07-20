# Yuxuan Zhao — Personal Website

A static personal academic website built for GitHub Pages. It has no build step and no runtime dependencies.

## Preview

Run a local server from this directory:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Content map

- `index.html`: all profile, research, selected-project, and life content
- `styles.css`: layout, typography, responsive behavior, and shared media frames
- `script.js`: mobile navigation, active-section highlighting, and viewport-aware video previews
- `assets/images/`: optimized research teaser images
- `documents/Yuxuan_Zhao_CV.pdf`: public CV download

## Replace the media placeholders

Project and life media frames can contain either images or videos. Place new files under `assets/media/` and replace the contents of the matching `.project-media` or `.life-media` block with one of these:

```html
<img src="assets/media/climbing.webp" alt="Yuxuan climbing an indoor bouldering route" />
```

```html
<video controls muted playsinline preload="metadata" poster="assets/media/skiing-poster.webp">
  <source src="assets/media/skiing.mp4" type="video/mp4" />
</video>
```

For a silent looping preview, add `class="media-preview"`, `muted`, `loop`, and `playsinline`; `script.js` will play it only while it is visible. Keep images under 500 KB where practical and short videos under 8–12 MB.

## Personal links still needed

Add GitHub, Google Scholar, and LinkedIn links to `.profile-links` when the URLs are available. A portrait can replace the current research image in `.profile-image` once a preferred photo is available.

## GitHub Pages

Push these files to a repository and set **Settings → Pages → Deploy from a branch**, using the repository's default branch and `/ (root)`.
