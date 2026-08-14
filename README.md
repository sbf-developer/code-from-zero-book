# Code, From Zero

A beginner-first, syntax-centered introduction to programming and software development.

## Included

- `src/code-from-zero.tex` — the complete LaTeX source
- `output/pdf/code-from-zero.pdf` — the compiled book

## Build

Requires a LaTeX installation with `pdflatex` and `makeindex`.

```bash
mkdir -p output/pdf
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=output/pdf src/code-from-zero.tex
makeindex output/pdf/code-from-zero.idx
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=output/pdf src/code-from-zero.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=output/pdf src/code-from-zero.tex
```

The book is designed as a clean, self-paced path from zero programming knowledge through core syntax, programming concepts, tools, web development, data, systems, and further study.
