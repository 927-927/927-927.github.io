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

## Adding item photos

Item photos live in `docs/assets/images/electronics/`. To swap one, replace the
file and keep its name (square or landscape 4:3 works best). If the photo is
someone else's (e.g. from Wikimedia Commons), keep or add the credit line under
it, like the existing ones.
