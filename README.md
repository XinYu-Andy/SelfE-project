# Self-E static page (modified)

This bundle contains:

- `index.html` — the main page
- `strip_data.js` — **the only file you need to edit** to populate the "Any-step sample strip" gallery

## What changed vs your original

1. Removed the GIF "Training progress" overlay (HTML/CSS/JS).
2. Moved the gallery (strip) image paths + prompts into `strip_data.js`.

## How to use

1. Put `index.html` and `strip_data.js` in the same folder.
2. Place your images under the paths you specify in `strip_data.js` (relative to `index.html`), e.g.:
   - `strip/2/01.png`
   - `strip/4/01.png`
   - `strip/8/01.png`
   - `strip/50/01.png`
3. Open `index.html` in a browser (or serve the folder via a static server).

## Editing the gallery

Open `strip_data.js` and replace each `src` and `prompt`.

Example:

```js
window.SELFE_STRIP_DATA = {
  2: [
    { src: 'strip/2/my_image.png', prompt: 'a photo of ...' },
  ],
  4: [],
  8: [],
  50: [],
};
```
