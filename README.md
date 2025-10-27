# Firm Model

> **The Firm is the promoter**

## 🌌 Constellation Information

- **Module Key**: `firm_model`  
- **Repository**: `firm-model`
- **Orbit**: 🧩
- **Status**: 🌿
- **Emoji**: 🏢

## 🚀 Quick Start

1. **Review seeds/**: Adapt seeded data for this module
2. **Configure schemas/**: Update schema definitions as needed  
3. **Generate signals/**: Create latest.json broadcast file

## 📡 Broadcasting

This module produces a `signals/latest.json` file conforming to the constellation's broadcast schema. The Signal (📡) aggregates these across all stars.  Use new-broadcast.sh within /scripts to run a new broadast.

## 🔗 CORE SYSTEM Links

- **Hub**: [FourTwenty Analytics](https://github.com/zbreeden/FourTwentyAnalytics)
- **The Archive**: Glossary, tags, and canonical definitions pulled down nightly and distributed out for constellation harmony.
- **The Signal**: Cross-constellation broadcasting and telemetry pulled and circulated nightly to foster promotion and development.
- **The Launch**: Detailed workflows pulled in nightly to assure an aligned culture of process improvement that starts from the Barycenter outwards to foster healthy architecture.
- **The Protector**: Examines workflows to assure drift is minimal fostering sustainability.
- **The Develper**: Feeds the constellation data for healthy modelling.

---
---

## Promotional Story — The Firm

**Founder:** Zachry Breeden  
**Mission:** To turn data into direction — where insight meets impact.

### About

FourTwenty Analytics was built on a simple idea: smart data should lead to smarter decisions.  
Rooted in descriptive and diagnostic analytics, the work began by asking better questions — not just “what happened,” but “why did it happen, and what should we do next?”

That foundation expanded into predictive and prescriptive analytics, focusing on clarity, communication, and measurable outcomes. Each project aims to bridge insight and action, shaping decisions that drive meaningful change.

### Approach

Every engagement begins with a question.  
From there: identify the right data, understand its lineage, clean and normalize it, explore patterns, visualize findings, and narrate insights that tie directly to decisions.

Technical execution supports this storytelling:
- **Python** for wrangling and analysis  
- **Power BI / Tableau** for visualization  
- **Excel / SQL** for storage and manipulation  
- **AWS** for architecture, flow, and scalability  

Ambiguity is handled through framing and analogy — turning uncertainty into storylines people can reason through.  
Data quality comes through documentation, peer review, governance, and security.  
Workflow is prioritized by impact, focusing energy on what moves the needle.  
Feedback is treated as signal, not noise — analyzed for context and pattern.

### Collaboration & Storytelling

Empathy and alignment sit at the center of stakeholder collaboration.  
Understanding goals, language, and perspective builds trust.  
Zach’s background in creative writing brings a natural voice to data storytelling — translating analysis into narratives people can see themselves in.

### Impacts & Outcomes

- Led conversion optimization projects using experimental data to identify key behavioral trends.  
- Streamlined data collection, reducing analysis costs by up to **10%** for platinum clients and strengthening long-term loyalty.  
- Monitored and maintained KPI reporting pipelines for **15–20 clients**, automating data collection and validation to improve reporting accuracy and turnaround time.  
- Reduced analytical operational costs by optimizing ETL and reporting workflows, saving up to **three hours per cycle**.  
- Scaled improvements firmwide and was later asked to **lead the implementation**.

### Closing

FourTwenty Analytics exists at the intersection of clarity and creativity — where clean data, sound methodology, and human understanding turn complexity into confident decisions.

## 🛠 Recent changes (2025-10-22)

The Firm UI was enhanced to provide immediate, interactive views for exploration and review:

- README renderer: The module now lazy-loads and sanitizes `README.md` (marked + DOMPurify) so you can preview documentation inline.
- Archive renderer: A new Archive panel fetches `signals/archive.latest.json` and renders archived broadcast cards.
- Workflow / Funnel renderer: A progress view consumes `signals/funnel_progress.json` and renders per-training cards with total steps, percent complete, progress bars and drill-down step lists. For Firm these steps represent job applications.
- Quick demo data: A fake `firm-model/signals/funnel_progress.json` was added (job-application steps derived from `data/internal/steps_df.csv`) so the UI shows content immediately. Replace or regenerate this file to reflect live data.

How to preview:

```bash
# start a simple server at the repo root so module-relative paths resolve
python3 -m http.server 8000
# then open http://localhost:8000/firm-model/index.html
```

If you want reproducible JSON from the CSVs, I can add a small script that converts `data/internal/*.csv` into `signals/funnel_progress.json` on demand.

*This star is part of the FourTwenty Analytics constellation - a modular analytics sandbox where each repository is a specialized "model" within an orbital system.*
