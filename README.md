# BSc. CSIT 8th Semester Internship Report LaTeX Template (CSC462)

A comprehensive, **Tribhuvan University (TU)** compliant LaTeX template for the **BSc. CSIT 8th Semester Internship (CSC462)** report. Designed for students under the **Institute of Science and Technology (IOST)** to streamline the report writing process.

## Key Features

- **Standard Compliant**: Pre-configured fonts (Times New Roman), margins, line spacing (1.5), and headings according to TU IOST guidelines.
- **Complete Structure**: Includes all necessary sections from Front Matter to Appendices.
- **APA 7 Referencing**: Built-in support for APA citation style using BibTeX.
- **Graphics Support**: Examples for including figures, tables, and screenshots.

## Report Structure

This template follows the standard structure required by the CSC462 course:

### Front Matter
- **Cover Page** & **Title Page**
- **Certificates**: Supervisor, Mentor, and Evaluation
- **Acknowledgements** & **Abstract**
- **Lists**: Tables, Figures, and Abbreviations

### Main Chapters
- **Chapter 1: Introduction**
  - Project/Work Introduction, Problem Statement, Objectives, Scope, Report Organization
- **Chapter 2: Organization Details & Literature Review**
  - Introduction to Organization, Hierarchy, Working Domains, Dept Description, Literature Review
- **Chapter 3: Internship Activities**
  - Roles, Weekly Log, Projects Involved, Technical Tasks
- **Chapter 4: Conclusion & Learning Outcomes**

### Back Matter
- **References** (APA Style)
- **Bibliography**
- **Appendices** (Screenshots, Code, Logs)

## File Structure

internship-report/
├── main.tex                  # Entry point for the LaTeX document
├── titlepage.tex             # Cover page layout
├── approval.tex              # Approval letter layout
├── supervisor.tex            # Supervisor recommendation layout
├── references.bib            # Bibliography database
├── CONTENT.md                # Detailed course guidelines & specs
├── images/                   # Directory for project images
└── chapters/                 # Individual chapter files
    ├── 00_abstract.tex
    ├── 01_introduction.tex
    └── ...
```

## Compilation Guide

### Requirements
- **Windows**: MiKTeX or TeX Live
- **macOS**: MacTeX
- **Linux**: TeX Live

### Build Commands (Local)

Run the following commands to generate the PDF and resolve references:

```bash
pdflatex main.tex
makeindex main.nlo -s nomencl.ist -o main.nls
pdflatex main.tex
pdflatex main.tex
```

The output file `main.pdf` will be generated in the root directory.

### using Overleaf

1.  **New Project**: Create a "Blank Project".
2.  **Upload**: Upload all files preserving the directory structure.
3.  **Compile**: Set `main.tex` as the main document and click "Recompile".

## Course Details (CSC462)

- **Course Title**: Internship
- **Credit Hours**: 6
- **Total Marks**: 200 (160 Internal + 40 External)
- **Duration**: Minimum 180 hours (10 weeks)

> For detailed formatting rules (Fonts, Margins, etc.), refer to `CONTENT.md`.
