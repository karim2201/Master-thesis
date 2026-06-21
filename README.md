# Master Thesis LaTeX Project

**Title:** Digital Twin for eHealth: State of the Art and Conceptual Architecture

This project contains the complete LaTeX source of the Master thesis. The state-of-the-art chapter is organized into two complementary reviews:

1. **Digital Twins in eHealth and healthcare**, covering patient, organ, hospital-process, public-health, architectural, AI, interoperability, governance, and validation research.
2. **Cardiovascular Digital Twins**, covering precision cardiology, electrophysiology, arrhythmia-risk modeling, ablation planning, virtual drug testing, electromechanics, hemodynamics, heart failure, AI surrogates, and population-scale cardiac twinning.

Each state of the art includes a dedicated landscape comparative table and a critical synthesis of maturity, evidence, limitations, and research gaps.

## Main file

- `main.tex`

## Compilation

Recommended on Overleaf or locally:

```bash
latexmk -pdf main.tex
```

Manual compilation:

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

## Main folders

- `preliminaries/`: title page, acknowledgements, abstracts, and acronyms
- `chapters/`: thesis chapters
- `figures/`: TikZ figures
- `bibliography/`: BibTeX references

## State-of-the-art chapter

`chapters/chapter6_comparative_study.tex` contains:

- the eHealth/healthcare Digital Twin state of the art;
- its dedicated comparative table;
- the cardiovascular Digital Twin state of the art;
- its dedicated comparative table;
- cross-domain synthesis and research gaps.

## Notes

- This version is configured for XeLaTeX in order to preserve Arabic, French, and English rendering.
- Landscape tables use `pdflscape`, `longtable`, and `ragged2e`.
- The title page styling, Arabic header text, and multilingual front matter are preserved from the current formatted project.
