# HSC study sheets

Static GitHub Pages app: one editable JSON file per module.

## Publish
Upload this folder to a GitHub repo, then enable **Settings → Pages → Deploy from a branch → main / root**.

## Add a module
Copy any file in `data/modules/`, change its `slug` and content, then add matching metadata to `data/modules/index.json`. Commit and push.

Preview locally with `python -m http.server 8000`; do not double-click the HTML, because browsers block JSON fetches from `file://`.

The provided JSON structure contains the fields required by the study-sheet app: core ideas, formula box, diagrams, practicals, traps, lower-priority knowledge and syllabus coverage. Populate each from the supplied syllabus before relying on it for revision.
