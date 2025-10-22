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
