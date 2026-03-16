# Ravine Studios Site

Static single-page site (`index.html`) with inline CSS and JS.

## Generic Modal System

The site includes a reusable modal overlay system. To add a new modal:

1. Add HTML with `data-modal="<id>"` and the `modal-backdrop` / `modal-panel` classes (see the template comment in `index.html`)
2. Open it from JS with `openModal('<id>')`
3. Deep-link to it via the query param `?modal=<id>` — it auto-opens on page load
4. Escape key and backdrop click close whichever modal is active
