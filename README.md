# Master Thesis LaTeX Project

**Title:** Digital Twin for eHealth: State of the Art and Conceptual Architecture

This project is a LaTeX structure for a Master thesis about Digital Twin for eHealth in a general healthcare context. The thesis uses a structured state-of-the-art literature review, includes cardiovascular Digital Twins as a representative clinical deep-dive, and introduces CardioTwin as a practical cardiovascular continuation for the PFE.

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
- `bibliography/`: expanded BibTeX references supporting Digital Twin foundations, healthcare applications, cardiovascular Digital Twins, interoperability, ethics, governance, and validation

## Methodology and appendix status
- The review is framed as a structured state-of-the-art literature review, not as an exhaustive protocol-based evidence synthesis.
- The comparative table remains a landscape multi-page `longtable`.
- The appendix was removed from compilation because it did not contain completed academic material.

## Notes
- The project uses XeLaTeX with Polyglossia for English, French, and Arabic.
- Arabic text is supported in `preliminaries/abstract_ar.tex`.
- The generated figures are TikZ diagrams included directly in the chapters.
