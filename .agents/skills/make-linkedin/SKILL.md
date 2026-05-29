---
name: make-linkedin
description: Transforms modular resume data into a highly optimized, compelling LinkedIn profile layout (Headline, About, Experience, and Education).
---

# Make LinkedIn

## When to use this skill

Use this skill when you need to transform a user's modular resume data into a highly optimized, compelling LinkedIn profile layout. This skill is designed to maximize the user's professional impact, target role alignment, and search engine optimization (SEO) within the LinkedIn platform.

## How to use it

### 1. Interactive Discovery (User Inputs)

Before generating any content, you must get the preferences of the user in the `config.md` file under the `## make-linkedIn Skill Customizations` section. These are the basic parameters required, if not present in the `config.md` file, ask the user these questions and update the `config.md` file with the user's responses:

1. **Target Expertise & Focus**: "What specific professional
expertise, core strengths, or career direction do you want to highlight for potential recruiters?"
2. **Keywords**: "Are there specific keywords, hard skills, or industry terms you want to weave into your profile to improve your search visibility on LinkedIn?"
3. **Output Language(s)**: "What language should the profile be generated in?"

### 2. Generation Strategy

Once the context is gathered, locate and analyze the user's modular resume data in the workspace, then apply the following optimization rules:

- **Headline**: Craft a high-conversion headline (max 220 characters). It must combine their core title, target expertise, and 2-3 high-impact keywords. Avoid generic text.
- **About (Summary)**: Write a compelling, first-person narrative (`I am...`). It should immediately hook recruiters, highlight their unique value proposition, seamlessly integrate the requested keywords, and end with a brief "Core Expertise" or "Tech Stack" list for scannability.
- **Experience & Education**: Adapt standard resume bullet points into a format optimized for digital reading—clean, impact-driven, and emphasizing outcomes rather than just responsibilities.

### 3. Output Formatting & File System Constraints

You must strictly adhere to the following output conditions:

- **Clean Markdown Only**: Do not include complex Markdown styling, HTML elements, or decorative UI blocks. The user needs to copy and paste this text directly into LinkedIn's plain-text form fields. Use only basic markdown headers (`#`, `##`) and standard bullet points (`*`) so the text is easily scannable in a standard markdown editor.
- **Multi-Language Handling**: If the user requests multiple languages, generate complete, separate sections for each language within the same file, clearly separated by an H1 header (e.g., `# English Profile`, `# Spanish Profile`).
- **File Destination**: Save the final output to the `built_profiles/` directory.
- **Naming Convention**: The file name must strictly follow this pattern: `linkedin-profile-[Current date and time in YYYY-MM-DD_HH-MM-SS format].md`.
  - *Example*: A file could be named exactly as: `built_profiles/linkedin-profile-2026-05-29_13-35-23.md`

### 4. Markdown Structure Template

Ensure the generated file strictly mirrors this structural layout for clean visualization and easy copy-pasting:

```markdown
# [Language] Profile
---

## Headline
[Insert optimized, high-impact headline here]

## About
[Insert compelling, keyword-rich summary narrative here]

## Experience
### [Job Title] at [Company Name]
[Dates or Location if applicable]
* [Impact-driven achievement bullet point]
* [Impact-driven achievement bullet point]

## Education
### [Degree/Certification]
[Institution Name]
```
