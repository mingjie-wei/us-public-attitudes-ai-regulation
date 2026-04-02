# U.S. Public Attitudes Toward AI and Federal Regulation

This repository contains the final project for IDS 702 - Modeling and Representation of Data at Duke University. It presents descriptive summaries and survey-weighted multivariate analysis (logistic regression, estimated marginal means, and related figures) in **R** and **Quarto** on U.S. adults’ views of AI’s long-term impact and federal AI regulation, using Pew Research Center **American Trends Panel (ATP) Wave 152** (August 2024, *Americans’ Views of Artificial Intelligence*).

## Report

The full write-up, figures, and tables are in **[`report.pdf`](report.pdf)** (rendered from the Quarto source). Read that document for background, methods, and detailed results.

## Key findings

- **Ideology and demographics** are linked to AI optimism: for example, men, liberals, higher-income respondents, and racial minorities tend to be more optimistic than women, conservatives, and lower-income White respondents (with age and education accounted for); adults aged 50–64 are comparatively the most pessimistic.
- **Trust in the federal government** conditions fears about over-regulation: among those who trust government competence, conservatives are much more likely than liberals to worry regulation will “go too far”; among those with little confidence, ideological gaps are smaller and over-regulation concern is lower overall.
- **Race** remains associated with fear of over-regulation after controls, consistent with how experience of state power may shape views of AI governance.

## Data

The code expects a Pew ATP **Wave 152** extract in a zip archive at:

`data/W152_Aug24.zip`

Inside the zip, the script reads the CSV at path `W152_Aug24/ATP W152.csv` (as in the default ATP delivery layout). **Pew data are subject to Pew’s terms of use**; if you do not have access, obtain the file from [Pew Research Center](https://www.pewresearch.org/) under their data-sharing rules. Do not redistribute restricted microdata in a public repository. For any publication or presentation that uses these data, follow Pew’s recommended citation and attribution for the American Trends Panel and Wave 152 materials (see Pew’s documentation for the dataset you use).

## Repository layout

| Path | Role |
|------|------|
| `scripts/script.qmd` | Quarto source: data prep, models, figures, and narrative |
| `data/` | Pew zip (not necessarily committed; see **Data**) |
| `report.pdf` | Compiled policy report (when present) |
