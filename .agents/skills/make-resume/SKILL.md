---
name: make-resume
description: Generates customized résumés that matches job description .txt files using data from a knowledge base and laTeX templates.
---

# Make Resume

## When to use this skill

Use this skill when the user wants to generate tailored résumés based on specific job descriptions. This skill is designed to work with a structured workspace containing:

- A `job-descriptions` folder with `.txt` files.
- A `knowledge_base` folder containing the source data for the résumé.
- A `templates` folder containing LaTeX or Markdown templates with placeholders.
- A `config.md` file in the root folder specifying the preferences of the user regarding the résumé, for example number of pages, bullet style, skills configuration, etc.

## How to use it

### 1. Language selection

- **Language**: Let the user decide whether they want the résumé in `English`, `Spanish`, both languages or another (specify).

### 2. Output format selection

- **Format**: Let the user decide whether they want the résumé in `.tex` or `.md` format. In case the selected format is `.tex` the résumé template will be `resume_template.tex` and the output will be in `.tex` format. Otherwise if the selected format is `.md` the résumé template will be `markdown-template.md` and the output will be in `.md` format.

### 3. Preparation

- **Read Configuration**: Access `config.md` to get the identity, contact information and preferences of the user regarding the résumé.
- **Load Template**: Retrieve the specified LaTeX or Markdown template from the `templates` folder.
- **Gather Data**: Read all relevant files in the `knowledge_base` folder. This is your only source of truth.

### 4. Job Analysis

- **Job description file selection**: In case there are more than one `.txt` file in the `job-descriptions` folder, let the user decide which one to use.
- **Analyze Job Description**: Read the selected `.txt` file in the `job-descriptions` folder.
- **Identify Keywords**: Extract key skills, technologies, and responsibilities emphasized in the job description.

### 5. Résumé Construction

- **Match Content**: Select data points from the `knowledge_base` that best demonstrate alignment with the job requirements.
- **Maintain Integrity**: **CRITICAL**: Use only provided data. Do not invent, hallucinate, or exaggerate experience or skills.
- **Populate Placeholders**: Replace the `[placeholder]` markers in the laTeX or markdown template with the mapped information from the knowledge base.

### 6. Finalization

- **Verify Output**: Ensure the resulting laTeX or markdown file is well-formatted and all placeholders are replaced.
- **Save Résumé**: Save the output file in the `built-resumes` folder, naming it based on the job description, language and role type.
