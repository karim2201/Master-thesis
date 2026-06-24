# Master Thesis LaTeX Project

**Title:** Digital Twin Technology in eHealth: Foundations, State of the Art, Cardiovascular Applications, and Architectural design for Cardiovascular Digital Twin

This project contains the complete LaTeX source of the Master’s thesis. It preserves the formatted title page, multilingual front matter, Arabic text support, XeLaTeX configuration, bibliography system, TikZ figures, and landscape comparative tables.

## Current Structure

- **Part I — General Introduction**
  - Chapter 1: General Introduction
- **Part II — Background**
  - Chapter 2: Digital Twin Fundamentals, Definitions, Dimensions, and Maturity
  - Chapter 3: eHealth and Digital Health Foundations
  - Chapter 4: Digital Twin in Healthcare and eHealth
- **Part III — State of the Art**
  - Chapter 5: Literature Review Methodology
  - Chapter 6: State-of-the-Art Review
- **Part IV — Selected Method**
  - Chapter 7: Selected Architecture for a Digital Twin-Based eHealth System
- **Part V — General Conclusion and Future Work**
  - Chapter 8: General Conclusion and Selected Method for the PFE

## Dual State of the Art

Chapter 6 is organized into two complementary studies:

1. **Digital Twins in eHealth and healthcare**, covering patient-specific twins, organ and device twins, hospital-process twins, public-health twins, Artificial Intelligence, hybrid AI--simulation models, interoperability, privacy, ethics, governance, validation, and technology maturity.
2. **Cardiovascular Digital Twins**, covering precision cardiology, electrophysiology, arrhythmia modeling, ablation planning, electromechanical and hemodynamic models, heart-failure twins, patient-specific calibration, AI-accelerated simulation, hybrid modeling, population-scale cardiac twins, validation, uncertainty, and identifiability.

Each state of the art includes a dedicated landscape `longtable`, critical synthesis, and explicit implications for the CardioTwin PFE.

## Added Synthesis Figures

The project includes academic TikZ synthesis figures for:

- the structured review workflow;
- the evolution of Digital Twin definitions;
- the classical three-dimensional Digital Twin approach;
- the extended five-dimensional Digital Twin approach;
- the three principal streams of Digital Twin definitions;
- the mapping of Digital Twin characteristics to the five-dimensional model;
- the Digital Twin lifecycle;
- the role of AI across the healthcare Digital Twin lifecycle;
- the taxonomy of eHealth Digital Twin applications;
- the taxonomy of cardiovascular Digital Twins;
- the evidence and maturity continuum;
- the translation from Master’s thesis findings to the CardioTwin PFE.

## Compilation

The project uses XeLaTeX because it relies on `fontspec`, `polyglossia`, and Arabic/French/English text.

Recommended command:

```bash
latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex
```

Manual compilation:

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

## Main Folders

- `preliminaries/`: title page, acknowledgement, English/French/Arabic abstracts, and acronyms
- `chapters/`: thesis chapters and completed appendix
- `figures/`: TikZ figures and the ESI logo
- `bibliography/`: BibTeX references

## Notes

- Landscape comparative tables use `pdflscape`, `longtable`, and `ragged2e`.
- The final chapter introduces CardioTwin as a practical cardiovascular continuation of the general eHealth Digital Twin study.
- The appendix contains completed supplementary review dimensions, not drafting notes.
