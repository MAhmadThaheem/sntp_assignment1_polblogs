# Original User Request

## 2026-09-15T17:46:24Z

# Teamwork Project Prompt — Draft

> Status: Launched
> Goal: Craft prompt → get user approval → delegate to teamwork_preview
> Requested team: [none — teamwork routes from the description]

Write an IEEE format academic report detailing the Social Network Theory and Practice assignment on Political Blogs Network Analysis (based on the provided Jupyter notebook). The report must include the methodology, graphs, and tables, and be compiled into a PDF.

Working directory: E:\sntp_report
Integrity mode: demo

## Requirements

### R1. Content Extraction
Read the e:\sntp_a1\SNTP_Assignment01_Master.ipynb notebook and its generated outputs/ directory to extract the analysis, tables, and figures. Write a 5 to 7 page academic report answering the assignment's problem statement.

### R2. IEEE Formatting
Search the web to find and download the official IEEE LaTeX template (IEEEtran.cls). Write the report in LaTeX utilizing the standard IEEE two-column format.

### R3. Compilation and Output
Compile the LaTeX document into a final PDF using pdflatex or a similar compiler available on the host system. The final PDF, along with the source .tex file and any copied figures, must be saved in the working directory E:\sntp_report (outside the original git folder).

## Acceptance Criteria

### Compilation Check
- [ ] A valid IEEEtran.cls is present in the working directory.
- [ ] A .tex file exists that utilizes \documentclass{IEEEtran}.
- [ ] The final compiled .pdf file exists in E:\sntp_report.

### Content Verification
- [ ] The .tex file explicitly includes figures (\includegraphics) mapped from the original outputs/figures directory.
- [ ] The .tex file includes tables representing the data from outputs/tables.
