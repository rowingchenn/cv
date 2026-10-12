# Weichen Zhang · Academic CV

An English academic CV centered on agentic intelligence, evaluation, and open
research infrastructure. The template uses a single column, restrained typography,
selectable text, and clickable paper and code links.

## Edit

[`cv.tex`](cv.tex) is the single source of truth. It is a standalone document:
no custom class, external fonts, bibliography, or companion files are required.
The content follows the formatting macros at the top of the file.

- `\entry{institution}{dates}{role}{advisor or location}` formats an appointment.
- `\paper{title}{authors}{venue and links}` formats a publication.
- `\me` highlights Weichen's name in author lists.

## Compile

Use a pdfLaTeX-compatible compiler. For an existing local TeX installation:

```sh
mkdir -p build
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=build cv.tex
pdflatex -interaction=nonstopmode -halt-on-error -output-directory=build cv.tex
```

The output is `build/cv.pdf`. The source is also self-contained for LaTeX editors.
GitHub Actions compiles the CV when the source changes and saves a PDF and log
as the `weichen-zhang-cv` artifact. It can also be run manually from the Actions tab.
The workflow does not publish a website or release.

## Content conventions

Keep research interests short and distinguish personal contributions from project
capabilities. Spell out submission status; do not imply acceptance. Use the
published author order and avoid ambiguous equal-contribution markers. The ALE
author list is abbreviated after the first three authors because it is extensive.

The original CV and paper attachments are reference material, not build inputs.
Working notes and unresolved facts belong in the ignored `private/` directory.
