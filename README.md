<p align="center"><img src="icon.png" width="120" alt="Universal Posters icon"></p>

# Universal Posters

Design one poster and adapt it to every aspect ratio. Universal Posters is a browser-based design app that keeps a single composition consistent across square, portrait, landscape, banner, strip and custom layouts, the way responsive web design adapts one page to many screens.

It runs entirely in the browser. There is no server, no build step and no account: everything is in `index.html`.

## Features

- **Responsive layouts:** shared positions across all aspect ratios, with per-layout overrides (marked with a yellow dot).
- **Automate:** finds your assets inside reference posters with sub-pixel accuracy (detail matching plus a pixel-level refinement pass) and builds every layout from them. Layout priority: a reference with the layout's exact shape first, then any other reference, then centring on the focal point.
- **Photoshop-style editing:** layers with opacity, visibility and locking; move, scale (proportional or free, from a corner or the centre) and rotate; sticky alignment guides; rule-of-thirds grid; zoom and hand tool; undo and redo.
- **Drawing layers:** paint with a brush (size, colour, eraser) on a layer whose box hugs the drawing, so it scales and rotates like any asset.
- **Cut out and Remove Background:** draw loosely around part of an image to keep just that part, or remove the background automatically. Runs entirely in the browser.
- **Text layers:** common fonts, size, bold and italic, colour and stroke. Shown automatically in thin layouts (banners and strips) where a logo has too little room.
- **Saving and exporting:** projects save as a single editable `.html` file that also works as a responsive preview. Export a PNG, all layouts as PNGs, all layouts as a ZIP, or a full project package.

## Publish on GitHub Pages

1. Create a new repository on GitHub, for example `Universal-Posters`.
2. Upload every file in this folder to the root of the repository, including the hidden `.nojekyll` file. On the repository page, choose **Add file › Upload files** and drag the files in.
3. Open **Settings › Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, then **Save**.
4. After a minute or two, the app is live at `https://<your-username>.github.io/<repository-name>/`.

On a phone, open that address and use **Add to Home Screen** to install it with its icon.

## Running it locally

Open `index.html` in a browser. Everything works offline except the optional text-layer fonts from Google Fonts, which need an internet connection the first time.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The complete app |
| `icon.png`, `icon-192.png` | App icons (512 px and 192 px) |
| `icon-maskable-512.png` | Full-bleed icon for Android home screens |
| `apple-touch-icon.png` | iPhone and iPad home-screen icon |
| `favicon-32.png` | Small browser-tab icon |
| `icon-original.jpg` | The original icon artwork |
| `manifest.webmanifest` | Lets phones install the app with its name and icon |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Browser notes

- Chrome and Edge on a computer open the system **Save** dialog, so you choose the file name and folder. Other browsers ask for the file name, then save to the downloads folder (or ask where, if that option is on in the browser's settings).
- Projects are also autosaved in the browser, so a reload can resume the last session.
