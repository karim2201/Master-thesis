# Master Thesis LaTeX Project

**Title:** Digital Twin for eHealth: State of the Art and Conceptual Architecture

This project is a starting LaTeX structure for a Master thesis about Digital Twin for eHealth in a general healthcare context. It intentionally avoids focusing on any specific PFE project or a single clinical specialty.

## Main file
- `main.tex`

## Compile
Recommended on Overleaf or locally:

```bash
latexmk -pdf main.tex
```

If compiling manually:

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

## Folder structure
- `preliminaries/`: title page, acknowledgements, abstracts, acronyms
- `chapters/`: thesis chapters
- `figures/`: generated TikZ figures
- `bibliography/`: BibTeX references

## Notes
- The project uses XeLaTeX with Polyglossia for English, French, and Arabic.
- Arabic text is supported in `preliminaries/abstract_ar_placeholder.tex`.
- The generated figures are TikZ diagrams included directly in the chapters.
- Replace all `[ ... ]` placeholders with your real university, student, supervisor, and jury information.
