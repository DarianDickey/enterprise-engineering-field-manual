# Career Roadmap — Cyber Risk + Analytics Niche

## Context

Operation Federal Ready's core mission (SQL foundations → aggregate functions → GROUP BY/HAVING → Python → Data Engineering tooling) remains the primary roadmap and continues unchanged through Week 3 and beyond. This document captures a **future project track**, layered on top of that foundation once core SQL and Python skills are solid — not a replacement for the current sequence.

The goal is a portfolio that sits at the intersection of two things I already have real experience in — Cyber Threat Intelligence (Tier 2 CTI analyst work, military background) and enterprise data analytics (current NFCU HR Analytics internship) — rather than a generic entry-level data analyst portfolio. Financial institutions in particular prioritize risk, compliance, and governance; a portfolio that speaks that language directly, backed by genuine domain background, is a differentiator.

## Ground Rules

- **All data is synthetic/mock data only.** No real NFCU data, systems, schemas, screenshots, or observations of any kind go into any public-facing project. This is a firm security and ethics boundary, not a style preference.
- **Sequencing matters.** These projects assume completed fundamentals: SQL joins (done), aggregate functions/GROUP BY/HAVING (Week 3 target), and basic Python (not yet started). Attempting the more advanced projects before those fundamentals are solid would produce weak, copy-pasted-feeling work — the opposite of the goal.
- **Depth over quantity.** One or two of these done well and explained clearly in interviews outweighs five done shallowly.

## Recommended Sequence

### Phase 1 — Prerequisite (in progress)
Complete Operation Federal Ready's existing SQL roadmap: joins (done), aggregate functions, GROUP BY, HAVING (Week 3), then begin Python fundamentals.

### Phase 2 — First Capstone: Security Operations Dashboard
**Why first:** Lowest new-tooling overhead. Primarily SQL (joins + aggregates, already in progress) plus Power BI — no new language required.

- **Concept:** Track incident response metrics on synthetic security log data — Mean Time to Detect/Respond, attack vector breakdown, phishing trend analysis.
- **Skills demonstrated:** SQL aggregation, Power BI dashboard design, translating raw log data into executive-level metrics.
- **Data:** Fully synthetic incident/log dataset, generated or mocked — never sourced from a real employer's systems.

### Phase 3 — Second Capstone: Data Governance Scorecard
**Why second:** Builds on the same SQL + Power BI skill set as Phase 2, but shifts the framing toward compliance and data quality — a category most entry-level applicants skip entirely, and one that maps directly to regulated-industry hiring needs.

- **Concept:** Visualize compliance percentages, data quality scores, and risk heat maps across a mock dataset.
- **Skills demonstrated:** Business acumen beyond coding; governance/GRC-adjacent thinking.

### Phase 4 — Insider Risk Analytics
**Requires:** Python fundamentals in place.

- **Concept:** Build rules to flag anomalous behavior in synthetic access-log data — after-hours logins, geographic anomalies, unusual file-access volume.
- **Framing requirement:** Must be explicitly and visibly framed in the README as a learning exercise built on fabricated data, with no implication it reflects any real employer's environment or observations.
- **Skills demonstrated:** Data modeling, risk threshold logic, moving beyond static dashboards into rule-based flagging.

### Phase 5 — Threat Intelligence Pipeline (capstone)
**Requires:** SQL fundamentals complete, Python comfortable, basic ETL concepts understood (Data Engineering Manual, DE-006/DE-007 already cover ETL vs. ELT conceptually).

- **Concept:** End-to-end pipeline — ingest synthetic/public-sample threat intelligence data via Python, transform and load into a SQL database using a star schema, surface key metrics in Power BI.
- **Skills demonstrated:** Full-stack data engineering (Python ETL, SQL data modeling, BI reporting) combined with CTI domain expertise — the strongest single differentiator in this roadmap.
- **Data sourcing note:** Use clearly synthetic data or properly licensed public threat-intel sample feeds only. Do not scrape or use any feed without confirming its terms of use permit this kind of public portfolio use.

## Portfolio Repository Structure

Proposed structure for `portfolio-projects`, once Phase 2+ work begins:

```
portfolio-projects/
├── README.md
├── 01-SQL/
│   └── (fraud-pattern queries, risk analysis, banking-style KPI queries)
├── 02-PowerBI/
│   └── (Security Ops, Governance Scorecard, Risk dashboards)
├── 03-Python/
│   └── (ETL pipelines, threat-intel automation)
└── 04-Cybersecurity/
    └── (threat intelligence documentation, domain write-ups)
```

This is separate from `sql-engineering/Projects`, which remains the raw, in-progress learning-exercise home (Project-001, 002, etc.). `portfolio-projects` is reserved for polished, resume-ready versions of finished work.

## Certification Alignment

This project track pairs naturally with the certification path already noted in the Data Engineering Manual future-learning entries:

- Security+ (already held)
- AZ-900 (Azure Fundamentals) — bridges data analytics and cloud engineering
- PL-300 (Power BI) — pair formal study with the actual dashboard builds above, rather than treating the cert as separate from the project work

## Status

This is a forward-looking roadmap entry, not an active assignment. No phase begins until the corresponding SQL/Python prerequisite is complete per the existing Weekly Operations Packet schedule.
