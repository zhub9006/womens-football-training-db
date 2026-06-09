# 🏟️ Women's Football Training Database

> **An evidence-based reference database for coaches, practitioners, and researchers** — cataloguing clinical trial protocols, intervention data, and trend analysis from ClinicalTrials.gov studies focused on strength, conditioning, and physical performance in female football players.

---

## 📋 Table of Contents
- [About This Database](#about-this-database)
- [Clinical Trial Landscape](#clinical-trial-landscape)
- [Trend Analysis](#trend-analysis)
- [Study Catalogue](#study-catalogue)
- [Protocol Library](#protocol-library)
- [Repository Structure](#repository-structure)
- [How to Contribute](#how-to-contribute)
- [Data Sources & Disclaimer](#data-sources--disclaimer)

---

## About This Database

Women's football is one of the fastest-growing sports globally, with over **30 million registered female players** (FIFA Women's Football Survey). Yet the evidence base for sex-specific strength and conditioning protocols lags far behind the men's game. This repository aggregates all identifiable clinical trial data from ClinicalTrials.gov relevant to:

- **Resistance & maximal strength training** in female footballers
- **Elastic band / blood-flow restriction (BFR) conditioning**
- **Neuromuscular & Kinetic Control training**
- **Physical performance outcomes** (sprint, jump, change-of-direction)
- **Injury prevention** (ACL, hamstring, lumbar spine, knee)

All protocols are extracted from registered clinical trials and are structured to be immediately actionable for practitioners.

---

## Clinical Trial Landscape

### Overview

Searching ClinicalTrials.gov with queries targeting resistance training, physical performance, conditioning, and injury prevention in female football / soccer players identified **~20 unique registered studies** across multiple nations and institutions. The evidence base is growing rapidly, with several trials registered in 2024–2025.

### Key Findings

| Metric | Value |
|--------|-------|
| Total studies identified | ~20 |
| Completed trials | ~13 |
| Recruiting / Active | ~5 |
| Not Yet Recruiting | ~2 |
| Trials with female-only cohorts | **100%** of core studies |
| Predominant study phase | Not Applicable (NA) — exercise science RCTs |
| Earliest registered trial | 2017 (Universidad de Zaragoza, Spain) |
| Most recent registrations | 2025 (Portugal, Turkey, Spain) |

### Geographic Distribution (countByCountry)

Based on trend analysis of studies focusing on female football players and exercise training:

| Country | Studies | Notable Institutions |
|---------|---------|----------------------|
| 🇪🇸 Spain | 3 | Universidad de Zaragoza (GENUD), University of Oviedo |
| 🇵🇹 Portugal | 2 | University Institute of Maia, Federação Portuguesa de Futebol |
| 🇹🇷 Turkey | 2 | Istanbul Medipol University, Istanbul Rumeli University |
| 🇨🇦 Canada | 2 | (undisclosed institutions) |
| 🇵🇱 Poland | 1 | John Paul II University in Biała Podlaska |
| 🇧🇦 Bosnia & Herzegovina | 1 | — |
| 🇸🇪 Sweden | 1 | — |
| 🇧🇪 Belgium | 1 | — |
| 🇳🇴 Norway | 1 | University of Tromsø (UiT) |
| 🇦🇪 UAE | 1 | Emirates Health Services |
| 🇩🇰 Denmark | 1 | Odense University Hospital |

> **Key insight:** Europe dominates this research space, particularly the Iberian Peninsula (Spain + Portugal) and Scandinavia. There is a notable absence of large-scale trials from major women's football nations such as the USA, Germany, England, or Australia — representing a significant research gap.

### Sponsor Type Analysis (countBySponsorType)

| Sponsor Category | Count | % of Total |
|-----------------|-------|------------|
| OTHER (universities, hospitals, research groups) | 10 | **91%** |
| NETWORK (multi-institutional consortia) | 1 | 9% |
| Industry / Pharma | 0 | 0% |

> **Key insight:** Research is almost entirely driven by academic institutions and sports science departments — not federation bodies, professional clubs, or commercial entities. This reflects both the grassroots nature of women's football research and a significant opportunity for governing bodies (FIFA, UEFA, national FAs) to co-fund larger, higher-powered studies.

### Phase Distribution (countByPhase)

| Phase | Count | Interpretation |
|-------|-------|----------------|
| Not Applicable (NA) | All studies | Exercise science trials are behavioural/other interventions — standard pharmaceutical phasing does not apply |

> **Key insight:** All registered trials are classified as "Not Applicable" phase, which is standard for exercise/behavioural intervention studies. This is not a limitation — rather, it reflects the nature of S&C research. The quality differentiator is study design (RCT vs. single-group, cluster-randomised vs. individual).

### Trial Status Breakdown

| Status | Count |
|--------|-------|
| ✅ COMPLETED | ~13 |
| 🔄 RECRUITING | ~3 |
| ⏸️ ACTIVE, NOT RECRUITING | ~2 |
| 📅 NOT YET RECRUITING | ~2 |
| ❓ UNKNOWN | ~1 |

---

## Trend Analysis

### Research Trajectory

- **2017–2019:** First wave of registrations — Spain (Zaragoza), Poland (Biała Podlaska), Norway (Tromsø). Focus on foundational questions: does maximal strength training improve sprint/jump? Does neuromuscular training prevent injury?
- **2023–2024:** Second wave — Turkey (Istanbul), Portugal (Maia). Focus shifts to comparison of modalities (BFR vs. isokinetic), elastic band training feasibility.
- **2025+:** Expanding scope — multi-level player comparisons (U15/U19/Senior), observational load-performance studies (Spain), hamstring eccentric/concentric RCTs (UAE).

### Emerging Themes

1. **Elastic band resistance training (EBT)** is the most actively studied modality in 2024–2025, with at least two concurrent Portuguese trials (NCT06648616, NCT06800079) examining its effects across age groups.
2. **Blood flow restriction (BFR) training** has entered women's football research (NCT06445478, Turkey), a technique previously studied almost exclusively in rehabilitation and male athlete populations.
3. **Neuromuscular / movement control training** (Kinetic Control framework) is gaining traction as a dual injury-prevention and performance-enhancement modality.
4. **Inter-limb asymmetry** is increasingly recognised as a risk factor and performance variable, with Spanish trials leading this work.
5. **Load monitoring** (sRPE, perceived fatigue) is emerging as a research focus for non-professional players.

### Critical Gaps Identified

- ❌ No large-scale (n>200) multi-site RCTs for women's football S&C
- ❌ No studies from major women's football markets (USA, Germany, England, Australia)
- ❌ Limited long-season (>16 weeks) intervention data
- ❌ No trials examining periodisation strategies across a full competitive season
- ❌ Sparse data on elite/professional level players (most studies use semi-professional or university-level cohorts)
- ❌ No trials integrating GPS/wearable load data with S&C outcomes

---

## Study Catalogue

See [`/studies/`](./studies/) for individual study files. A summary index is below:

| NCT ID | Title | Country | n | Duration | Intervention | Status |
|--------|-------|---------|---|----------|--------------|--------|
| [NCT04048928](./studies/NCT04048928.md) | Maximal Strength Training in High-level Female Football Players | 🇳🇴 Norway | 46 | 5 weeks | Barbell back squat MST (≥85% 1RM) | ✅ Completed |
| [NCT03862560](./studies/NCT03862560.md) | Physical Performance & Functional Asymmetries in Female Football | 🇪🇸 Spain | 68 | 12 weeks | Strength training program | ✅ Completed |
| [NCT06445478](./studies/NCT06445478.md) | BFR Exercises vs. Isokinetic Exercises in Female Football Players | 🇹🇷 Turkey | 30 | 8 weeks | BFR-RE vs. ID-RE | ✅ Completed |
| [NCT04134741](./studies/NCT04134741.md) | Neuromuscular Training (Kinetic Control) in Female Football Players | 🇵🇱 Poland | 18 | 4 weeks (×2 seasons) | Kinetic Control NMT | ✅ Completed |
| [NCT06648616](./studies/NCT06648616.md) | Elastic Band Resistance Training in Female Football — Pilot | 🇵🇹 Portugal | 10 | 6 weeks | EBT (bi-weekly, 20 min) | 🔄 Recruiting |
| [NCT06800079](./studies/NCT06800079.md) | Elastic Band Training: Knee Strength & Performance (U15/U19/Senior) | 🇵🇹 Portugal | 60 | 8 weeks | EBT (bi-weekly, 20 min) | 🔄 Recruiting |
| [NCT07274566](./studies/NCT07274566.md) | Exer-Genie Speed & ABC Drill Training in Female Football Players | 🇹🇷 Turkey | 37 | 8 weeks | Exer-Genie® resisted sprint + ABC drills | ✅ Completed |
| [NCT06789900](./studies/NCT06789900.md) | Football Fitness Concept for Bone Health in Postmenopausal Women | 🇩🇰 Denmark | 136 | 24 weeks | Football Fitness (1hr, 2×/week) | ⏸️ Active |
| [NCT07408739](./studies/NCT07408739.md) | Weekly Strength Training Load & Perceived Performance in Soccer | 🇪🇸 Spain | — | Cross-sectional | Observational (sRPE) | ⏸️ Active |

---

## Protocol Library

See [`/protocols/`](./protocols/) for structured workout protocols extracted from trials.

| Protocol File | Modality | Duration | Sessions/Week | Key Exercises |
|--------------|----------|----------|---------------|---------------|
| [maximal-strength-squat.md](./protocols/maximal-strength-squat.md) | Maximal Strength | 5 weeks | 2 | Back squat ≥85% 1RM + Nordic hamstring |
| [elastic-band-resistance.md](./protocols/elastic-band-resistance.md) | Elastic Band RT | 6–8 weeks | 2 | 6 EBT exercises, 20 min/session |
| [blood-flow-restriction.md](./protocols/blood-flow-restriction.md) | BFR Resistance | 8 weeks | 2 | BFR leg press/squat/knee ext at 20–40% 1RM |
| [kinetic-control-nmt.md](./protocols/kinetic-control-nmt.md) | Neuromuscular | 4 weeks | 3 | Active core/lower limb Kinetic Control exercises |
| [exer-genie-speed.md](./protocols/exer-genie-speed.md) | Resisted Speed + Agility | 8 weeks | 3 | Exer-Genie® sprints + ABC agility drills |
| [isokinetic-resistance.md](./protocols/isokinetic-resistance.md) | Isokinetic RT | 8 weeks | 2 | Leg press, squat, knee extension (isokinetic device) |

---

## Repository Structure

```
womens-football-training-db/
├── README.md                          # This file — landscape overview & trend analysis
├── studies/                           # Individual study detail files (one per NCT ID)
│   ├── NCT04048928.md
│   ├── NCT03862560.md
│   ├── NCT06445478.md
│   ├── NCT04134741.md
│   ├── NCT06648616.md
│   ├── NCT06800079.md
│   ├── NCT07274566.md
│   ├── NCT06789900.md
│   └── NCT07408739.md
├── protocols/                         # Extracted workout protocols
│   ├── maximal-strength-squat.md
│   ├── elastic-band-resistance.md
│   ├── blood-flow-restriction.md
│   ├── kinetic-control-nmt.md
│   ├── exer-genie-speed.md
│   └── isokinetic-resistance.md
├── data/                              # Machine-readable data
│   ├── studies-index.json             # Full study index in JSON
│   └── trend-analysis.json            # Trend analysis results
└── CONTRIBUTING.md                    # How to add new studies
```

---

## How to Contribute

This is a **living database** — new trials are registered regularly. To contribute:

1. **Add a new study:** Search ClinicalTrials.gov, create a new file in `/studies/` using the template in any existing study file, and update the index table in this README.
2. **Add a protocol:** If a study contains sufficient intervention detail, extract it into `/protocols/` following the existing template.
3. **Update data files:** Keep `/data/studies-index.json` and `/data/trend-analysis.json` current.
4. **Report errors:** Open a GitHub Issue if you find inaccuracies in extracted data.

See [`CONTRIBUTING.md`](./CONTRIBUTING.md) for detailed guidelines.

---

## Data Sources & Disclaimer

- **Primary source:** [ClinicalTrials.gov](https://clinicaltrials.gov) (U.S. National Library of Medicine)
- **Data accessed:** June 2025
- **Search terms used:** Female/women football/soccer + resistance training, strength conditioning, physical performance, plyometric, neuromuscular training
- **Filters applied:** COMPLETED, RECRUITING, ACTIVE_NOT_RECRUITING status

> ⚠️ **Disclaimer:** This database is for educational and reference purposes only. All protocols are extracted from registered clinical trial descriptions and should not be implemented without appropriate professional supervision. Always consult a qualified strength and conditioning coach or sports medicine professional before prescribing training interventions.

---

*Last updated: June 2025 | Maintained by the Women's Football Research Community*
