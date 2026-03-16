# Ravine Studios Site

Static single-page site (`index.html`) with inline CSS and JS.

## Generic Modal System

The site includes a reusable modal overlay system with a registration-based architecture. To add a new modal:

1. Add HTML with `modal-backdrop` / `modal-panel` classes (see the template comment in `index.html`)
2. Register it: `registerModal('my-param', document.getElementById('my-modal'))`
3. Open via JS: `openModal('my-param')`
4. Deep-link: `?my-param` — the query param **key** triggers the modal on page load
5. Escape key and backdrop click close whichever modal is active

The query param is the key itself (e.g. `?gdc`, `?announce`), not a value. This lets the same mechanism be extended for other query-param-driven behaviors.
