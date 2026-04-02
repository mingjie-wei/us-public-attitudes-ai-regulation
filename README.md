# U.S. Public Attitudes Toward AI and Federal Regulation

This repository contains the final project for IDS 702 - Modeling and Representation of Data at Duke University.

It presents descriptive summaries and survey-weighted multivariate analysis (logistic regression, estimated marginal means, and related figures) in **R** and **Quarto**. 

The analysis uses Pew Research Center **American Trends Panel (ATP) Wave 152** (August 2024, *Americans’ Views of Artificial Intelligence*) and focuses on U.S. adults’ views of AI’s long-term impact and federal AI regulation.

## Report

The full write-up, figures, and tables are in **[`report.pdf`](report.pdf)** (rendered from the Quarto source). Read that document for background, methods, and detailed results.

## Key findings

- **Ideology and demographics** are linked to AI optimism: for example, men, liberals, higher-income respondents, and racial minorities tend to be more optimistic than women, conservatives, and lower-income White respondents (with age and education accounted for); adults aged 50–64 are comparatively the most pessimistic.
- **Trust in the federal government** conditions fears about over-regulation: among those who trust government competence, conservatives are much more likely than liberals to worry regulation will “go too far”; among those with little confidence, ideological gaps are smaller and over-regulation concern is lower overall.
- **Race** remains associated with fear of over-regulation after controls, consistent with how experience of state power may shape views of AI governance.

## Data

**Survey microdata are not included in this repository** (Pew ATP files cannot be redistributed here). To run `scripts/script.qmd` yourself, obtain **Wave 152** under [Pew Research Center](https://www.pewresearch.org/)’s terms, then place the zip on your machine at:

`data/W152_Aug24.zip`

(relative to the repo root; create the `data/` folder locally if needed). Inside the zip, the script expects the CSV at `W152_Aug24/ATP W152.csv`, matching the usual ATP delivery layout. For any publication or presentation that uses these data, follow Pew’s recommended citation and attribution for the American Trends Panel and Wave 152 materials (see Pew’s documentation for the dataset you use).

## Repository layout

| Path | Role |
|------|------|
| `scripts/script.qmd` | Quarto source: data prep, models, figures, and narrative |
| `data/` | **Not tracked** - local folder where you place `W152_Aug24.zip` if you re-run the analysis (see **Data**) |
| `report.pdf` | Compiled policy report (when present) |
