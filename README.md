# Master Thesis LaTeX Project

**Title:** Digital Twin for eHealth: State of the Art and Conceptual Architecture

This project is a LaTeX structure for a Master thesis about Digital Twin for eHealth in a general healthcare context. The main study remains focused on Digital Twins for eHealth, while the final chapter introduces CardioTwin as a practical cardiovascular continuation for the PFE.

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
  - Chapter 1: General Introduction
  - Chapter 2: Digital Twin Fundamentals
  - Chapter 3: eHealth and Digital Health Foundations
  - Chapter 4: Digital Twins in Healthcare and eHealth
  - Chapter 5: Literature Review Methodology
  - Chapter 6: Comparative Study of Digital Twin Approaches in eHealth
  - Chapter 7: General Conclusion and Proposed Method for the PFE
- `figures/`: generated TikZ figures
- `bibliography/`: BibTeX references

## Notes
- The project uses XeLaTeX with Polyglossia for English, French, and Arabic.
- Arabic text is supported in `preliminaries/abstract_ar_placeholder.tex`.
- The generated figures are TikZ diagrams included directly in the chapters.
- Replace all `[ ... ]` placeholders with your real university, student, supervisor, and jury information.
