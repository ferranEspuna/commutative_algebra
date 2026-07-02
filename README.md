# commutative_cositas

## Automated PDF build

This repository builds its LaTeX PDFs with a cross-platform Python wrapper around `latexmk`.
Generated PDFs are ignored by git and are published by GitHub Actions on every push.

Build all PDFs locally:

```bash
python scripts/build.py
```

Clean and create a release zip:

```bash
python scripts/build.py --clean --package
```

Outputs:
- `out/exercises_1.pdf`
- `out/exercises_2.pdf`
- `out/theory.pdf`

The release zip is written to `dist/commutative_algebra-release.zip` and contains the PDFs plus a buildable source tree.
