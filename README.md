# Survival Wiki Starter (MkDocs Material)

A ready‑to‑run starter for a printable, cross‑linked survival knowledge wiki.

## Quickstart
```bash
python -m venv .venv && source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
mkdocs serve  # open http://127.0.0.1:8000
```
- Edit Markdown files in `docs/` (you can use Obsidian).
- Use `[[Wikilinks]]` to cross‑link pages; they’re resolved by the `mkdocs-roamlinks-plugin`.
- Print any page from your browser. For a **single‑PDF of the whole site**, open **“Print whole site”** in the nav, then print to PDF.
- Build static site: `mkdocs build` → output in `site/` (host on GitHub Pages, Cloudflare Pages, or Netlify).

## Structure
```
docs/
  index.md
  ingredients/alcohol.md
  recipes/tinctures.md
  plants/skirret.md
  styles/print.css   # tuned for 8.5×11in
mkdocs.yml
requirements.txt
```

## Notes
- `styles/print.css` enforces US Letter paper and hides chrome when printing.
- Add tags in the YAML front matter (`tags: [...]`) to organize content.
- Add more content types: `tools/`, `techniques/`, `recipes/`, etc.
