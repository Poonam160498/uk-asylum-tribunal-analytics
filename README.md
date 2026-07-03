# UK Asylum Appeal Outcomes — Tribunal Analytics

**How consistent are UK asylum appeal decisions across hearing venues?**
An independent, exploratory analysis of Ministry of Justice First-tier Tribunal statistics (2018/19 – 2025/26).

> 🔎 **Headline finding:** disposal-weighted allow rates vary from roughly **27% to 55% across hearing venues** — a spread of ~27 percentage points. That spread has **narrowed to ~12 points by 2025/26**, coinciding with the rollout of a new case-management system.

<!-- Add a dashboard screenshot here: ![<img width="936" height="435" alt="Screenshot 2026-07-03 at 14 59 59" src="https://github.com/user-attachments/assets/50979f5d-83f3-4c9d-a07f-527ec2d7efd0" />
) -->

## Why this project

Asylum appeals are among the highest-stakes decisions in the UK justice system, yet there is little public, analytics-driven scrutiny of how consistent outcomes are between hearing venues. The official data to ask that question exists and is open — this project puts it to work.

I bring an unusual combination to it: a law background (LLM) for the legal context — tribunal procedure, what venue differences can and can't mean — and current MSc Business Analytics training (University of Exeter) for the data work.

## What's in this analysis

- **Data pipeline** — cleaning and reconciling MoJ venue-level tribunal statistics (duplicate venue labels, financial-year alignment)
- **Weighted allow rates** — rates weighted by appeals determined per venue, so small venues don't distort the picture
- **Venue comparison** — spread, coefficient of variation (0.14), and which venues sit at the extremes
- **Time trends** — how venue variation has changed from 2018/19 to 2025/26
- **Interactive dashboard** — <!-- file:///Users/poonamnauroji/Downloads/appeal_dashboard-2.html -->

## Important caveats (read before quoting)

Raw variation is **not** proof of unfairness. Part of the venue spread is expected case-mix: for example, Harmondsworth hears detained appeals, which differ systematically in character. This exploratory analysis **describes** the variation; it does not adjust for case-mix or claim causal conclusions. Treat the numbers as a starting point for questions, not a verdict.

## Data

- **Source:** Ministry of Justice, Tribunal Statistics Quarterly (First-tier Tribunal, Immigration & Asylum Chamber — asylum/protection case type)
- **Licence:** [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/)
- **Coverage:** financial years 2018/19 – 2025/26
- Contains public sector information licensed under the Open Government Licence v3.0.

## Tech

Python (pandas) for cleaning and analysis · <!-- Tableau / Power BI --> for the dashboard · Jupyter notebooks for the workflow

## Repo structure

```
├── data/          # raw + cleaned MoJ extracts (CSV)
├── notebooks/     # analysis notebooks, in order
├── images/        # dashboard screenshots & charts
└── README.md
```

## Roadmap

- [ ] Nationality-level breakdowns
- [ ] Case-mix–adjusted comparison (in progress)
- [ ] Automated quarterly data refresh

## About me

Poonam Nauroji — MSc Business Analytics, University of Exeter · LLM · Based in Exeter, UK
[LinkedIn](https://www.linkedin.com/in/poonam-nauroji) · Also built [RankReady](https://meraneetprep.netlify.app), a free NEET prep dashboard.
