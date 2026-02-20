# Vishnu Selvaraj — Photos

Single-page photo portfolio.

## Add / remove / reorder photos

1. Put image files in `photos/` (recommended: `.jpg`).
2. Edit `photos.json`:
   - Add a photo: add a new entry like:
     ```json
     { "src": "photos/my-new-photo.jpg" }
     ```
   - Remove a photo: delete its entry.
   - Reorder: move entries up/down.

Notes:
- Paths are case-sensitive on GitHub Pages.
- Keep filenames simple (lowercase, no spaces) to avoid URL issues.

## Slideshow behavior

- Auto-advances every **4 seconds**.
- Pauses when:
  - The menu is open, or
  - The browser tab is hidden.
- Manual navigation (scroll / swipe / keyboard / dots) resets the timer.

## Local preview

From the repo root:

```bash
python3 -m http.server 8000
```

Then open: http://localhost:8000/

## Publish (GitHub Pages)

```bash
git add index.html photos.json photos/
git commit -m "Update photos"
git push
```
