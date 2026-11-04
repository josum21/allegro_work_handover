# Experimental technical notes

English LaTeX draft for PCB test installation, toolkit usage, bench procedures and analysis definitions. Red **To complete** paragraphs mark information that needs bench knowledge or validation; example script values are not claimed to be universally valid instrument presets.

## Build

From this directory, with a TeX distribution providing `latexmk` and pdfLaTeX:

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=output/pdf main.tex
```

The result is `output/pdf/main.pdf`. `main.tex` loads two top-level chapters: `chapters/pcb_testing.tex` and `chapters/tbd.tex`. The PCB chapter includes the existing numbered source files as sections, including its configuration reference and record template. Add photographs and diagrams under `figures/` and replace the framed placeholders with `\includegraphics`.

## Contents

Chapter 1, **PCB Testing**, contains the following sections. Chapter 2, **TBD**, is reserved for the next topic.

- Setup, signal path and numbering conventions
- Installation and communication checks
- Toolkit entry points and data organisation
- Practical acquisition and offline workflow
- Analysis equations, output interpretation and limitations
- Configuration reference, campaign record template and source notes

Drafted from the local FCC installation note and PCB toolkit on 2026-11-03. No hardware acquisition or MATLAB analysis was run. Source toolkit files were left unchanged.
