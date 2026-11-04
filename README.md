# 927-927.github.io
testing RBedu website github pages feasibility

## Local preview

```bash
pip install -r requirements.txt
mkdocs serve
```

Then open <http://127.0.0.1:8000>. Pushing to `main` rebuilds the live site.

## Adding a page

1. Create a new `.md` file in the right section folder under `docs/`.
2. Add it to the `nav` section of `mkdocs.yml`.

## Chinese version

The 中文 / English button in the header switches between the English site
(`/`) and the Chinese site (`/zh/`). Every page has a Chinese copy next to it
with a `.zh` suffix, e.g. `docs/hardware/cad.md` → `docs/hardware/cad.zh.md`.
When you change an English page, update its `.zh.md` too. A page without one
shows the English text on the Chinese site.

- Use the terms in [translation-glossary.md](translation-glossary.md).
- Keep the English heading anchors on translated headings, e.g.
  `## 线规（AWG） { #wire-gauge-awg }`, so links work in both languages.
- Chinese nav titles go under `nav_translations` in `mkdocs.yml`.
- Diagrams work the same way: `can-bus-chain.zh.svg` is used on the Chinese
  site in place of `can-bus-chain.svg`.
- The CAN animations' own labels are in `STRINGS` in
  `docs/javascripts/can-sim.js`.

## Adding item photos

Item photos live in `docs/assets/images/electronics/` and
`docs/assets/images/hardware/`. To swap one, replace the
file and keep its name (square or landscape 4:3 works best). If the photo is
someone else's (e.g. from Wikimedia Commons), keep or add the credit line under
it, like the existing ones.
