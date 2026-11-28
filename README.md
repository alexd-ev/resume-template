# LaTeX Resume Template
## Overview
My personal LaTeX resume template uses a bibliography file for optional referees. Generates a compiled PDF file for viewing.

## Technical Specification
To build the latex project, an online LaTeX previewer can be used such as [Overleaf](https://www.overleaf.com/project). Alternatively, if building locally is desired, then a LaTeX distrubution such as [TeX Live](https://www.tug.org/texlive/acquire.html) is required. Download the latest released `alexds-resume-template.zip` archive found here: https://github.com/alexd-ev/resume-template/releases/latest. If using an online previewer upload the zip when creating a project. Otherwise, extract the files then run the application using `latexmk` by running this command in a terminal:
```bash
latexmk -pdf alexds-resume-template.tex
```
Open the PDF file: `alexds-resume-template.pdf`

To remove the optional referees, comment out lines `alexds-resume-template.tex:165-168`, and can build instead with `pdflatex` for faster compilation:
```bash
pdflatex alexds-resume-template.tex
```
Open the PDF file: `alexds-resume-template.pdf`

## Project Structure
```
resume-template/
├── .gitignore                              - Ignore LaTeX metadata files
├── LICENSE                                 - GPL-3.0 licence
├── README.md                               - Documentation
├── resume-template-referees.bib            - BibTeX bibliography document
├── resume-template.pdf                     - Generated PDF file
└── resume-template.tex                     - LaTeX text document
```

# Author
`alexd-ev` (Alex Davidson)

Copyright Alex Davidson (c) 2026
