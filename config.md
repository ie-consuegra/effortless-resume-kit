# Configuration

## Global Configuration (Applied to all skills)

### Identity / Contact information

Write the values (in the links section write the URLs without the https:// protocol, just write the domain name with the path) or leave blank.

**Full Name**: Fred Flintstone
**Degree Suffix**: B.Sc.
**Location**: Bedrock, 345 Cave Lane
**Phone**: +1-BR-549
**Email**: <fred.f@slatequarry.com>

**LinkedIn**: linkedin.com/in/fredflintstone-yabbadabbadoo
**GitHub**:
**Website**: fredflintstone.com
**Portfolio**:
**Behance**:

---

## `make-resume` Skill Customizations

### Résumé Summary Template

Write a professional summary of the user, based on the data in the `knowledge_base` folder and the job description in the `job-descriptions` folder. The summary should be tailored to the job description.
The template is a suggestion, the agent can modify it if needed, the final summary should be as follows (it contains further instructions enclosed in square brackets [] that must be followed while generating the summary):

[Domain] professional with [N]+ years combining [primary method] and [secondary method] for [application domain].
[1-2 sentences on key accomplishments tailored to the job description]. [Metrics: publications, citations, awards if applicable].

### Document Preferences

- **Resume pages:** 2
- **Resume bullet variant:** 2L (all variable bullets are 2-line)
- **Skills config (resume):** 4-3-2-2-2 (13 lines, 5 groups)
- **Immigration line:** No | "Authorized to work in the United States"

---

### Provenance Flags

Track the publication status of your work. Skills check this table before every output.

| Item | Status | Correct Framing |
| ---- | ------ | --------------- |
| _Example: My Nature paper_ | _under review_ | _"under review at Nature" — never say "published in Nature"_ |
| _Example: Internal tool_ | _unpublished_ | _"infrastructure I developed" — never imply peer-reviewed_ |

Add your own rows. Delete the examples.

---

### KB Corrections Log

Verified errors to never re-introduce. Add entries as you catch mistakes.

| Correction | Details |
| ---------- | ------- |
| _Example: Tool X name_ | _It's "ToolX-v2" not "ToolX". Always use the correct name._ |

---

### Role Types

Define the role types you're targeting. Each gets a bundle during setup.

| Role Name | Target Employers | Tier | Bundle File |
| --------- | ---------------- | ---- | ----------- |
| _Example: National Lab_ | _DOE labs, national facilities_ | _1_ | _bundle_national_lab.md_ |
| _Example: Industry R&D_ | _Tech companies, R&D divisions_ | _2_ | _bundle_industry_rd.md_ |

**Tier guide:** 1 = strongest evidence, full portfolio | 2 = strong with targeted emphasis | 3 = viable with careful framing

---

### Role-Type Decision Tree

Customize this to map Job descriptions keywords to your role types.

| If Job descriptions mentions... | Primary profile | Secondary (hybrid) |
| ----------------- | -------------- | ----------------- |
| _[your domain keywords]_ | _[role type]_ | _[secondary or --]_ |

---

### FIXED Sections

List template sections that should NEVER be modified during generation.
These are copied verbatim from your template every time.

- Education
- Leadership & Volunteering
- Publications (if applicable)
- Honors & Awards (if applicable)
- Header block (name, contact, links)

---

### Output Rules

- **Email in all outputs:** [same as Personal Info email]
- **Resume package:** [N] pages + 1-page cover letter

---

## `make-linkedIn` Skill Customizations

**Target Expertise & Focus**:

- Target Roles: Heavy Equipment Operator, Quarry Operations Supervisor, Industrial Site Foreman.

- Professional Branding: A dedicated, hands-on specialist with over 20 years of uninterrupted experience in raw material extraction and mega-fauna steering.

- Key Value Proposition: "Maximizing bedrock excavation throughput while maintaining zero-incident safety records with unpredictable biological machinery."

**Keywords**: Bronto-Crane Operator, Quarry Supervisor, Heavy Equipment
**Output language(s)**: English

### Tone & Style Preferences

**Tone**: Conversational, first person narrative ("I am", "I do", "I did").
**Emoji use**: Use professional emojis sparingly in the 'About' section (e.g., 🚀, 💼) to break up text sections. | Do not use emojis in the output.

---
