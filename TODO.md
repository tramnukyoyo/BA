# TODO.md — Phase 1 Rebuild Sprint (10 Days)

## Phase 1: Exposé Rebuild — HRS-Specific Focus

**Goal:** Rebuild exposé with HRS-specific focus, find 10 new papers, ready for professor submission

**Duration:** 10 days | **Status:** 25% complete (infrastructure done, awaiting paper search)

**Thesis Focus:** Wasserstofftankstellen (HRS) Implementierung und Herausforderungen
- **Shift from:** General hydrogen infrastructure (production, pipelines, storage)
- **Focus now:** HRS deployment, barriers (regulatory, logistical, technical), scenarios, economics

---

## Week 1: Paper Search & Selection (Days 1–7)

### Days 1–3: Execute Paper Searches

**Research Strategy File:** `literature/SEARCH_STRATEGY_HRS.md`

**Execute 10 Targeted Searches:**

1. **Query 1: Overview & Supply Chain Integration**
   - [ ] Search Google Scholar, ScienceDirect for supply chain papers
   - [ ] Expected keywords: "hydrogen refueling station" + "supply chain integration"
   - [ ] Track candidates in PAPER_CANDIDATES.md (Content Area 1)

2. **Query 2: Logistical & Technical Challenges**
   - [ ] Search for HRS operational/technical/logistical barriers
   - [ ] Keywords: "hydrogen refueling" + "technical challenges" + "logistics"
   - [ ] Track in Content Area 2

3. **Query 3: Spatial Planning & Corridor Optimization**
   - [ ] Search for HRS location optimization, corridor deployment
   - [ ] Keywords: "hydrogen refueling station" + "spatial planning" + "location optimization"
   - [ ] Track in Content Area 3

4. **Query 4: Economic Viability & Cost-Benefit Analysis**
   - [ ] Search for HRS cost analysis, NPV, ROI
   - [ ] Keywords: "hydrogen refueling" + "cost-benefit" + "economics"
   - [ ] Track in Content Area 4

5. **Query 5: Technical Reliability & Maintenance**
   - [ ] Search for HRS reliability, maintenance, equipment performance
   - [ ] Keywords: "hydrogen refueling station" + "reliability" + "maintenance"
   - [ ] Track in Content Area 5

6. **Query 6: Regulatory Frameworks & Standards**
   - [ ] Search for HRS standards, regulations, ISO, safety
   - [ ] Keywords: "hydrogen refueling" + "regulation" + "standards"
   - [ ] Track in Content Area 6

7. **Query 7: Strategic Network Design**
   - [ ] Search for HRS network design, deployment strategy
   - [ ] Keywords: "hydrogen refueling station" + "network design" + "strategy"
   - [ ] Track in Content Area 7

8. **Query 8: Global Market Insights**
   - [ ] Search for HRS market trends, regional deployment, adoption
   - [ ] Keywords: "hydrogen refueling" + "market" + "deployment trends"
   - [ ] Track in Content Area 8

9. **Query 9: Techno-Economic Literature Reviews**
   - [ ] Search for HRS review papers, state-of-the-art
   - [ ] Keywords: "hydrogen refueling" + "review" + "techno-economic"
   - [ ] Track in Content Area 9

10. **Query 10: Policy & Institutional Context (EU)**
    - [ ] Search for EU HRS policy, AFIR, TEN-T
    - [ ] Keywords: "hydrogen refueling" + "EU" + "policy" + "AFIR"
    - [ ] Track in Content Area 10

**Target:** 30–50 candidate papers total (3–5 per content area)

**Success Metric:** At least 1 promising candidate per content area by Day 3

---

### Days 4–7: Evaluate & Select

**Evaluation Tool:** Quality checklist template in SEARCH_STRATEGY_HRS.md

**For Each Candidate Paper:**
- [ ] Verify peer-reviewed journal (recognized database)
- [ ] Check publication year (2019–2025 preferred)
- [ ] Assess HRS-specificity (not general hydrogen infrastructure)
- [ ] Review methodology clarity (formulas, data sources, simulations)
- [ ] Count citations (Google Scholar)
- [ ] Check reference list depth (50–100 citations)
- [ ] Determine content fit to one of 10 areas

**Selection Criteria:**
- [ ] Accept 10 papers total (1 per content area)
- [ ] Each paper meets ALL quality checks
- [ ] No redundancy (different aspects/authors)
- [ ] Balanced geographic coverage (EU, Asia, Australia where possible)

**Deliverable:** 10 final papers documented with:
- Title, authors, year, journal, DOI
- Citation count and quality score
- Which content area they address
- Brief summary of key contribution

---

## Week 2: Integration & Final Compilation (Days 8–10)

### Day 8: Complete Bibliography File

**File:** `expose/references_h2_CORE.bib`

**For Each of 10 Papers:**
- [ ] Fill in BibTeX entry (author, title, journal, year, volume, pages, DOI)
- [ ] Include keywords (HRS, specific content area, focus dimension)
- [ ] Add abstract summary with key findings
- [ ] Verify Harvard style formatting
- [ ] Check DOI links are valid

**Success:** All 10 papers in valid BibTeX format, ready for LaTeX compilation

---

### Days 9–10: LaTeX Integration & Final Compilation

**File:** `expose/expose_bachelor.tex`

**Integration Tasks:**
- [ ] Update bibliography reference: `\addbibresource{references_h2_CORE.bib}`
- [ ] Integrate citations throughout exposé sections:
  - Ausgangslage: cite regional HRS strategies
  - Problemstellung: cite barrier papers
  - Forschungsfragen: cite papers addressing each RQ
  - Zielsetzung: cite methods/frameworks
  - Gliederung: map papers to chapters
  - Framework section: cite all 10 papers in appropriate dimensions
- [ ] Verify framework section uses bullet-point format (not old text boxes)
- [ ] Run LaTeX compilation:
  ```bash
  pdflatex expose_bachelor.tex
  biber expose_bachelor
  pdflatex expose_bachelor.tex
  pdflatex expose_bachelor.tex
  ```
- [ ] Check PDF output (all citations render, no errors)
- [ ] Verify all 10 papers appear in Literaturverzeichnis

**Final Deliverable:** `expose/expose_final_v2.pdf`

---

## Success Criteria Checklist

**Infrastructure (Done):** ✓
- [x] SEARCH_STRATEGY_HRS.md created with 10 targeted queries
- [x] PAPER_CANDIDATES.md tracking template created
- [x] FRAMEWORK_DESIGN.md with bullet-point design created
- [x] expose_bachelor.tex restructured (HRS-specific content)
- [x] references_h2_CORE.bib template created

**Paper Search (Days 1–7):**
- [ ] 30–50 candidate papers found and tracked
- [ ] At least 1 strong candidate per content area
- [ ] 10 final papers selected (1 per area)
- [ ] All papers meet quality criteria

**Final Exposé (Days 8–10):**
- [ ] references_h2_CORE.bib completed (10 papers, valid BibTeX)
- [ ] All citations integrated into expose_bachelor.tex
- [ ] PDF compiles without errors
- [ ] All 10 papers appear in bibliography
- [ ] Framework section shows all 3 dimensions + 10 papers
- [ ] No generic "hydrogen infrastructure" language (all HRS-specific)
- [ ] expose_final_v2.pdf ready for professor submission

---

## Current Sprint Status

**Status:** ⏳ IN PROGRESS (25% complete)

**What's Done:** ✓
- Infrastructure files created (search strategy, templates, LaTeX restructure)
- expose_bachelor.tex updated with HRS-specific content
- PAPER_CANDIDATES.md ready for data entry

**What's Next:** (User-driven)
- Execute 10 paper searches (Days 1–3)
- Evaluate and select 10 papers (Days 4–7)
- Complete bibliography and compile final PDF (Days 8–10)

**Next Review:** After completing Day 3 searches (check: 30–50 candidates tracked?)

---

## Project References

- **Strategy:** See `literature/SEARCH_STRATEGY_HRS.md` (detailed search approach)
- **Tracking:** See `literature/PAPER_CANDIDATES.md` (candidate database)
- **Design:** See `expose/FRAMEWORK_DESIGN.md` (framework structure)
- **Timeline:** See `.planning/ROADMAP.md` (full 10-day rebuild timeline)
- **State:** See `.planning/STATE.md` (rebuild rationale & progress)

---

**Project Rules:** See `CLAUDE.md`
**Last Updated:** 2026-02-13 (Phase 1 Rebuild Initialization)
**Status:** Awaiting user execution of paper searches (Days 1–3)
