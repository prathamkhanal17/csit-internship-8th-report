# Internship Report Template

## Overview

This project contains a LaTeX template for Bsc.CSIT CSC462 Internship Report.

## Document Structure

### Front Matter

- **Cover Page**: Title, intern name, organization details, duration
- **Certificate Pages**: Scanned certificates and approval letters
- **Acknowledgements**: Expression of gratitude to supporters
- **Abstract**: Summary of internship activities and achievements
- **Table of Contents**: Navigation guide for the report
- **List of Figures**: All figures included in the report
- **List of Tables**: All tables included in the report
- **List of Abbreviations**: Definitions of technical acronyms

### Main Chapters

- **Chapter 1: Introduction**
  - 1.1 Introduction to the project/work
  - 1.2 Problem Statement
  - 1.3 Objectives
  - 1.4 Scope and Limitation
  - 1.5 Report Organization

- **Chapter 2: Organization Details and Literature Review**
  - 2.1 Introduction to Organization
  - 2.2 Organizational Hierarchy
  - 2.3 Working Domains
  - 2.4 Description of Intern Department/Unit
  - 2.5 Literature Review / Related Study

- **Chapter 3: Internship Activities**
  - 3.1 Roles and Responsibilities
  - 3.2 Weekly Log
  - 3.3 Description of Projects Involved
  - 3.4 Detailed Technical Tasks/Activities

- **Chapter 4: Conclusion and Learning Outcomes**
  - 4.1 Conclusion
  - 4.2 Learning Outcome

### Back Matter

- **References**: APA-style citations of referenced works
- **Bibliography**: Additional studied resources
- **Appendices**: Network diagrams, screenshots, work logs, source code

## Compilation Guide

### Local Compilation

Ensure LaTeX distribution is installed:

- **Windows**: MiKTeX or TeX Live
- **macOS**: MacTeX
- **Linux**: TeX Live

Compile the document using pdflatex:

```bash
pdflatex main.tex
makeindex main.nlo -s nomencl.ist -o main.nls
pdflatex main.tex
pdflatex main.tex
```

Run pdflatex multiple times to ensure proper generation of table of contents and nomenclature.

### Overleaf Compilation

**Option 1: Direct Upload**

1. Create a "Blank Project" in Overleaf
2. Upload all files and folders maintaining directory structure
3. Ensure `main.tex` is the main document

**Option 2: Import from GitHub**

1. Push this repository to GitHub
2. In Overleaf, select "New Project" > "Import from GitHub"
3. Select your repository for automatic sync

**Option 3: Direct Git Push (Premium)**

1. Create a "Blank Project" in Overleaf
2. Go to "Menu" > "Git" and copy the Git URL
3. Add remote and push:
```bash
git remote add overleaf <overleaf-git-url>
git push overleaf main
```

## Report Requirements

Based on CSC462 course guidelines:

### Formatting Standards

- **Font**: Times New Roman
- **Font Sizes**:
  - Chapter Headings: 16pt (Bold)
  - Section Headings: 14pt (Bold)
  - Sub-section Headings: 12pt (Bold)
  - Paragraph Text: 12pt
- **Spacing**: 1.5 line spacing, justified alignment
- **Margins**: Top, Bottom, Right = 1 inch; Left = 1.25 inches
- **Page Numbering**: Roman numerals (i, ii, iii...) for front matter; Arabic numerals (1, 2, 3...) starting from Chapter 1
- **Referencing**: APA Standard

### Course Information

- **Course Title**: Internship
- **Course No**: CSC462
- **Credit Hours**: 6
- **Total Marks**: 200 (160 Internal/Mentor + 40 External)
- **Duration**: Minimum of 180 hours or 10 weeks


## File Structure

```
internship-report/
├── main.tex                  # Main LaTeX document
├── titlepage.tex             # Cover page layout
├── CONTENT.md                # Course guidelines
├── README.md                 # Project documentation
├── wiki.md                   # This file
├── images/                   # Image files directory
│   ├── certificate_scan.png
│   └── approval_scan.png
└── chapters/                 # Chapter files
    ├── 00_abstract.tex
    ├── 00_acknowledgement.tex
    ├── 01_introduction.tex
    ├── 02_background.tex
    ├── 03_internship_activities.tex
    ├── 04_conclusion.tex
    ├── 05_references.tex
    ├── 06_bibliography.tex
    └── 07_appendices.tex
```

## Quick Start

1. Ensure LaTeX distribution is installed
2. Navigate to project directory
3. Run compilation commands
4. View generated PDF as `main.pdf` in the same project directory

## Technical Details

### LaTeX Packages Used

- `geometry`: Page margin configuration
- `mathptmx`: Times New Roman font
- `setspace`: Line spacing control
- `titlesec`: Heading formatting
- `graphicx`: Image handling
- `caption`: Caption formatting
- `float`: Image positioning
- `nomencl`: Abbreviations list
- `url`: URL handling

### Custom Configurations

- Chapter headings centered at 16pt
- Section headings at 14pt
- Subsection headings at 12pt
- 1.5 line spacing throughout
- Bold captions for figures and tables

## Output

The compiled report is saved as `main.pdf` in the project directory. The PDF includes all front matter, main chapters, references, bibliography, and appendices with proper formatting, page numbering, and cross-references.
