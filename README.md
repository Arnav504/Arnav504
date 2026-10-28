# Arnav Sahai

**Data analyst** for clients who need a decision from ambiguous data.

Columbia SIPA, MPA, Data Science for Policy · New York, NY

I do the technical work and the client work on the same problem. I clean conflicting sources, fit the method to the question, and write the result so a non-technical reader can see what was measured, what was assumed, and what decision the analysis supports. The five repositories below are the public record: a community-board housing study, an equity-market event study, trade briefs tied to official statistics, and two analyst tools for noisy public and crisis data.

Open to data analyst roles.

[Portfolio](https://arnav-sahai-portfolio.vercel.app/) · [LinkedIn](https://www.linkedin.com/in/arnav-sahai-370702116/) · [arnav.sahai@columbia.edu](mailto:arnav.sahai@columbia.edu)

---

## Five repositories

Each one names the question, the sources, and a page or script a reviewer can open.

### [Manhattan CB9 housing analysis](https://github.com/Arnav504/CB9_housing)

**Client question.** When housing in Western Harlem is offered at a share of Area Median Income, which households can afford it, and where are supportive services already concentrated?

Built for Manhattan Community Board 9 during a Community Planning Fellowship with the Fund for the City of New York. The repository retrieves and reconciles 2023 Census estimates, HPD and NYCHA records, PLUTO, the NYC Facilities Database, and 311 complaints, and sets those comparisons beside the board report. The service-saturation formula is specified and left unscored, because the facilities file has site locations and a capacity field of zero, not supportive-housing unit counts.

Python · Quarto · public-data pipelines  
[Methods site](https://arnav504.github.io/CB9_housing/)

### [Data breach disclosures and equity markets](https://github.com/Arnav504/Data_breach_stock)

**Question.** How do U.S. stock prices react when a firm publicly discloses a data breach?

Two reproducible pipelines on a cited breach dataset and daily prices: a market-model event study, and a Callaway–Sant’Anna difference-in-differences comparison of firm and S&P 500 cumulative returns. On the documented run of 20 April 2026, mean CAR(0, +10) is about −0.12% across 224 non-confounded events, and the average abnormal return is sharply negative on the disclosure day. The dynamic ATT is about −0.22 (95% CI [−0.42, −0.02]). The write-up keeps those as separate estimates.

R · tidyquant · event studies · `did`

### [ASAN Macro](https://github.com/Arnav504/Trade_AI_Project)

**Question.** How do you brief a trade corridor so every figure in the prose is the same row as the chart?

A tool-grounded agent writes short economic briefs from UN Comtrade merchandise, World Bank trade totals, and IMF current-account series. The bars are SQL aggregates of the rows behind the text. When Comtrade returns no official rows, the page reports that and does not fill the corridor with sample data. Three briefs are already computed: BRICS minerals, US–China electronics, and Vietnam/Mexico supply into the United States.

Python · SQLite · tool-calling  
[Live briefs](https://asan-macro.vercel.app)

### [Cyber Narrative Radar](https://github.com/Arnav504/cyber-narrative-radar)

**Question.** Which shifts in public cyber discussion deserve an analyst’s attention, and which posts justify the flag?

The pipeline ingests public feeds (RSS, Reddit, CISA, NVD) and a labeled synthetic demo set, maps posts to organizations and narrative types, and raises alerts with a score plus the evidence underneath. Clustering is TF-IDF and K-means. Summaries are rule-based, so a reviewer can retrace an alert from the posts that produced it.

Python · FastAPI · React · SQLAlchemy  
[Dashboard](https://cyber-narrative-radar-web.onrender.com)

### [Escalation Risk Lab](https://github.com/Arnav504/crisis-analyzer-ai)

**Question.** Relative to a human-only baseline, how does an AI-assisted reading change crisis-escalation risk, and which assumptions move the score?

A dashboard over a synthetic corpus of cyber, geopolitical, and energy incidents. A reader compares baseline and AI-assisted scores and changes detection speed, model confidence, false-positive risk, human oversight, attribution uncertainty, and economic dependency. Methods and data limits are part of the interface. Scoring is a unit-tested module that runs in the browser on local data.

TypeScript · React · TanStack  
[Demo](https://crisis-analyzer-ai.lovable.app)

---

## Client and research work

The same standard as the repositories: name the decision, reconcile the sources, and leave a trail someone else can audit.

- **Community Planning Fellow**, Fund for the City of New York — Manhattan Community Board 9 (Sep 2025–Apr 2026). Housing affordability and equity in West Harlem. ACS, GIS, and a service-saturation analysis, delivered as a board presentation, a resource guide, and a decision framework for CB9 leadership.
- **Research Consultant**, Sinclair Capital (Sep 2025–Dec 2025). Client-facing statistical and financial model for an open business question. Assumptions, inputs, and outputs documented for review. Recommendation presented in writing and in person to a non-technical audience.
- **Development Impact Measurement Intern**, International Finance Corporation, World Bank Group (Oct 2025–Dec 2025). Quantitative work across 15+ projects: cleaned and validated datasets, relational databases, and repeatable SQL, Python, and R workflows with methods and metadata for later review.
- **Data Analyst Intern**, The Smart Cube (Mar 2019–May 2019). Procurement and supply-market research, including supplier benchmarks, cost drivers, and Tableau and Power BI reporting. Redesigned ETL and QA workflows and improved data accuracy by 70%.
- **Application Development Associate**, Accenture (Oct 2019–May 2021). Production data integration for a global pharmaceutical client. Java and Spring MVC processes across 1,500 interfaces, monitored with Splunk, with defect triage for downstream consumers.

## Toolkit

**Analysis.** Python, R, SQL, Pandas, the tidyverse, survey and administrative microdata, event studies, difference-in-differences

**Client reporting.** Tableau, Power BI, Quarto, and memos a non-technical reader can challenge

**Delivery.** TypeScript, React, FastAPI, Git, and pipelines that rerun from the repository

Longer case studies, papers, and certificates are on the [portfolio](https://arnav-sahai-portfolio.vercel.app/).
