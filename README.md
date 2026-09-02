# Résumé — Amit Singh

All content lives in [`resume.yaml`](resume.yaml). `build.py` turns it into the web page and the PDFs.

## Editing

1. Edit `resume.yaml` (plain text; `&`, `<` etc. are escaped for you).
2. Rebuild:

   ```sh
   pip install pyyaml        # once
   python3 build.py          # HTML + PDFs
   python3 build.py --no-pdf # HTML only
   ```

PDFs are printed with headless Chrome (Chromium, Brave or Edge also work); set `CHROME=/path/to/binary` to choose one.

## Outputs

| File | Contents | Committed |
| --- | --- | --- |
| `index.html` | Public web page (GitHub Pages) | yes |
| `Amit-Singh-Senior-Software-Engineer-Resume.pdf` | Public PDF, linked from the page's *Download PDF* button | yes |
| `out/Amit-Singh-Senior-Software-Engineer-Resume.pdf` | Private PDF including contact items marked `private: true` (phone) — the one to send to recruiters | no (git-ignored) |

Styling is in `assets/resume.css`; fonts (Archivo, SIL OFL) are in `assets/fonts/`. Don't hand-edit `index.html` — it is regenerated on every build.

## Publish on GitHub Pages

1. Commit and push to `amit-sengar/resume` on `main`.
2. Repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main`, folder: `/ (root)` → Save.
3. Live in ~1 minute at `https://amit-sengar.github.io/resume/`.

Custom domain: add a `CNAME` file containing the domain, then point a `CNAME` DNS record at `amit-sengar.github.io`.
