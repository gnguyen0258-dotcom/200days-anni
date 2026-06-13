# Our Day Bice Clone

Static clone of `https://our-day-bice.vercel.app/?id=261f2m2x0b0tihu9`.

## Run

Use a local server because the app uses ES modules:

```bash
python -m http.server 4290
```

Then open:

```text
http://127.0.0.1:4290/index.html
```

Customize:

```text
http://127.0.0.1:4290/customize.html
```

## Customize to GitHub Pages workflow

1. Open `customize.html` and edit the text, images, music, colors, pages, plates, and phrases.
2. Click `Xem trang` to preview the current draft in `index.html?preview=1` on the same browser.
3. Click `Luu nhap` only keeps a browser draft. It does not change the public GitHub Pages site.
4. Click `Xuat ZIP` when the preview is correct.
5. Extract the ZIP and upload/replace all extracted files in the GitHub repo.
6. GitHub Pages will then serve the new `assets/config.js`, `assets/config.json`, images, and music.

## Files

- `index.html`: static boot page, no Firebase/protection scripts.
- `customize.html`: browser editor for changing text, images, gallery, phrases, heart color, music, and exporting a ready-to-upload ZIP.
- `assets/config.js`: local `window.FIREBASE_DATA` used by `data.js`.
- `assets/config.json`: readable copy of the same config.
- `assets/images/`: downloaded letter and gallery images.
- `assets/music/background.mp3`: downloaded background music.
- `main.js`, `data.js`, `acts/`: original front-end modules/styles needed by the experience.

Three.js and Google Fonts are still loaded from CDN.
