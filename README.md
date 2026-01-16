# Internship Report LaTeX Template

This repository contains a LaTeX template for an internship report.

## Prerequisites

You need a LaTeX distribution (like TeX Live, MiKTeX, or MacTeX) installed on your system.

## Project Structure

- `main.tex`: The main LaTeX file that defines the document structure and formatting.
- `titlepage.tex`: Contains the layout for the front cover.
- `chapters/`: Directory for individual report sections (Introduction, Background, etc.).
- `images/`: Directory for scans and figures.
- `.gitignore`: Configured to ignore LaTeX build artifacts.

## How to Compile

### Locally
Run `pdflatex` on the main file:

```bash
pdflatex main.tex
```

Note: You may need to run the command twice to correctly generate the Table of Contents and Figure lists.

### Overleaf

There are three ways to use this with Overleaf:

**Option 1: Direct Upload (Easiest)**
1. Create a "Blank Project" in Overleaf.
2. Upload all files and folders.

**Option 2: Import from GitHub**
1. Push this repository to a GitHub account.
2. In Overleaf, select **New Project** > **Import from GitHub**.
3. Select your repository. This maintains a link for future syncs.

**Option 3: Direct Git Push (Premium)**
1. Create a "Blank Project" in Overleaf.
2. Go to **Menu** > **Git** and copy the provided Git URL.
3. Add it as a remote to your local repository:
   ```bash
   git remote add overleaf <overleaf_git_url>
   ```
4. Push your changes:
   ```bash
   git push overleaf master
   ```

## Output

The generated report will be saved as `main.pdf`.
