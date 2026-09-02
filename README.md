# Résumé — Amit Singh

Single self-contained page. No build step, no dependencies.

## Publish on GitHub Pages

1. Commit `index.html` (and `Amit-Singh-Java-Backend-Engineer.pdf` once exported) to the root of `amit-sengar/resume` on `main`.
2. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main`, folder: `/ (root)` → Save.
3. Live in ~1 minute at `https://amit-sengar.github.io/resume/`.

Custom domain: add a `CNAME` file containing the domain, then point a `CNAME` DNS record at `amit-sengar.github.io`.

## Regenerating

Edit the source résumé, then re-export the standalone page — do not hand-edit `index.html`, it is compiled output.
