# Step-by-Step Guide: Adding Reference Materials

This guide walks you through adding colleague materials to the context-and-references folder.

---

## Quick Start (5 Minutes)

### Step 1: Create a Folder for This Material

```bash
mkdir context-and-references/exposés/Anna_Mueller
```

Replace:
- `exposés` with: exposés, bachelor-theses, thesis-proposals, or master-theses
- `Anna_Mueller` with colleague's name (use underscores, not spaces)

### Step 2: Add the PDF and Metadata

Inside `Anna_Mueller/`, create two files:

**File 1: `metadata.txt`**
```
REFERENCE METADATA
==================

Name: Anna Mueller
Topic: Renewable Energy in German Industrial Transition
Type: Exposé

Institution: University of Duisburg-Essen
Department: Engineering & Environmental Studies
Year: 2024

Pages: 7
Word Count: 3,500 (estimated)

Subject Area: Energy Transition / Renewable Energy
Related to Your Work: Yes - similar supply chain focus

Key Sections:
- Motivation
- Research Question
- Literature Overview
- Methodology
- Timeline

Why This Reference: Shows how to structure an energy-focused exposé with supply chain implications

Status: Received
Date Added: 2026-01-31
```

**File 2: PDF**
Just copy/paste the actual PDF into this folder. Name it clearly:
- `Mueller_Exposé_2024.pdf` OR
- `exposé.pdf` (simple)

### Step 3: Add Your Analysis (Optional but Recommended)

Create `notes.md`:

```markdown
# Anna Mueller — Hydrogen/Renewables Exposé Analysis

## Structural Breakdown
- **Total Pages:** 7
- **Motivation & Problem:** 1 page
- **Research Question:** 0.5 pages
- **Literature Review:** 2 pages
- **Methodology:** 1.5 pages
- **Expected Outcomes & Timeline:** 2 pages

## Table of Contents
1. Einleitung (Introduction)
2. Problemstellung (Problem Statement)
3. Forschungsfrage(n) (Research Question)
4. Stand der Forschung (Literature Review)
5. Methodischer Ansatz (Methodology)
6. Erwartete Ergebnisse (Expected Outcomes)

## Formatting Observations
- Font: Times New Roman, 12pt
- Margins: 2.5cm all sides
- Line spacing: 1.5
- Headers: Bold, hierarchical
- No images in exposé (text-focused)

## Language & Tone
- Academic German, modern active voice
- Formal but accessible
- Clear topic sentences
- Varied sentence length
- Some technical terminology but well-explained

## Strengths
- Problem statement is very clear
- Research question is specific and testable
- Literature review is concise but comprehensive
- Methodology section explains how she'll actually conduct research

## Things to Adopt
- The 2-page literature review: compact but covers state-of-the-art
- Problem statement structure: context → gap → why-it-matters
- Use of subheadings within methodology
- Clear timeline with realistic phases

## Questions for Yourself
- Should your motivation be 1 or 1.5 pages?
- How detailed should your literature review be? (She uses ~5 sources)
- Should you include diagrams/concept maps? (She doesn't in exposé)

## Statistics Extracted
- Average lines per page: ~45 (double-spaced)
- Approximate sources cited: 5-7
- Figures/Tables: 0
- Footnotes: Minimal (1-2)

**Date Analyzed:** 2026-01-31
```

### Step 4: Update the Catalog

Edit `REFERENCE-CATALOG.md` and add an entry to the appropriate section:

```markdown
### Anna Mueller — Renewable Energy Supply Chain Transition

**Type:** Exposé
**Subject Area:** Energy Transition / Supply Chain
**Institution:** University of Duisburg-Essen
**Year:** 2024
**Pages:** 7
**Folder:** `context-and-references/exposés/Anna_Mueller/`

**Why This Reference:**
Energy-focused exposé with supply chain implications. Shows structure for problem-statement-driven RQ with timeline-based methodology.

**Key Elements to Study:**
- [x] Structure
- [x] Table of Contents
- [x] Visual presentation (or lack thereof)
- [x] Literature review approach
- [x] Methodology
- [x] Results/outcomes presentation

**Status:** [x] Analyzed — see notes.md
```

### Step 5: Commit to Git

```bash
cd /c/Users/denny/Bachelorarbeit
git add context-and-references/
git commit -m "ref: Add Anna Mueller — Renewable Energy Exposé as reference"
```

---

## Detailed Instructions

### Where to Get Colleague Materials

- Ask classmates directly
- Check university thesis database/repository
- Ask your advisor for examples
- Look at department website for past work

### Naming Conventions

**Folder names:** Use underscores for spaces
- ✓ Anna_Mueller
- ✓ Jan_Bergmann
- ✗ Anna Mueller (spaces cause issues in some systems)

**PDF files:** Be descriptive
- `Mueller_Exposé_2024.pdf` (Good)
- `notes.pdf` (Unclear)
- `exposé.pdf` (OK if only one per folder)

**Notes file:** Always name it `notes.md` for consistency

### PDF Storage Considerations

**Option 1: Store PDFs in Git (Simple)**
- Pros: Everything in one repo, version controlled
- Cons: Repository gets large
- Use if: Total PDFs < 200MB

**Option 2: Store PDFs Separately (Better for Large Collections)**
- Create a cloud storage link (Google Drive, OneDrive)
- In metadata.txt, add a `Cloud Link:` field
- Example:
  ```
  Cloud Link: https://drive.google.com/file/d/[ID]/view
  ```
- Then add `.gitignore` entry:
  ```
  context-and-references/**/*.pdf
  context-and-references/**/*.docx
  ```
- Pros: Repo stays lean
- Cons: Links can break

### Analyzing a Document: What to Look For

**Structure:**
- How many main sections?
- How are they titled?
- Is there a logical flow?
- Does each section serve a purpose?

**Length Distribution:**
- Which sections get the most space?
- Is it well-balanced?
- How much is intro vs. content?

**Formatting:**
- Font choices (serif vs. sans-serif)
- Margins (narrow, standard, wide?)
- Line spacing (single, 1.5, double?)
- Use of headings (H1, H2, H3 levels?)

**Content Density:**
- Text-heavy or visually broken up?
- Many paragraphs or bulleted lists?
- Do they use images/diagrams?

**Citations:**
- How many references?
- In-text frequency?
- Are they Harvard style?

**Language:**
- Active or passive voice?
- Sentence length (short, varied, long)?
- Jargon level?

### Creating Comparative Notes

After adding 3-5 similar materials (e.g., 5 colleague exposés), create a comparative analysis:

**File:** `context-and-references/EXPOSÉ-COMPARATIVE-ANALYSIS.md`

```markdown
# Comparative Analysis: Colleague Exposés

## Page Count Distribution
- Mueller: 7 pages
- Berg: 6 pages
- Schmidt: 8 pages
- **Average: 7 pages**

## Section Length (Pages)
|  Section | Mueller | Berg | Schmidt | Average |
|----------|---------|------|---------|---------|
| Motivation | 1.0 | 1.0 | 1.5 | 1.2 |
| RQ | 0.5 | 0.5 | 1.0 | 0.7 |
| Lit Review | 2.0 | 1.5 | 2.0 | 1.8 |
| Methodology | 1.5 | 1.5 | 2.0 | 1.7 |
| Outcomes | 2.0 | 1.5 | 1.5 | 1.7 |

## Formatting Consensus
- Font: Times New Roman, 12pt (all)
- Margins: 2.5cm (all)
- Line spacing: 1.5 (all)
- Language: German (all)

## Takeaway for Your Work
Based on 5 colleague exposés:
- Plan for 6-8 pages total
- Allocate ~1 page each for intro/motivation
- ~2 pages for lit review
- ~1.5 pages for methodology
- ~1.5 pages for outcomes/timeline
```

---

## Common Issues & Solutions

### Issue: PDF is Password Protected
**Solution:** Ask your colleague for the unprotected version, or note this in metadata

### Issue: Document is in English, Yours is German (or vice versa)
**Solution:** Still useful! Note in metadata that it's a language/style reference. Analyze structure independently

### Issue: The Document is Really Long (Master Thesis)
**Solution:** Focus on specific chapters relevant to your work. Note which chapters you analyzed in your notes.md

### Issue: Document Has No Table of Contents
**Solution:** Create one yourself as you analyze. This helps you understand the structure

### Issue: Permission/Copyright Concerns
**Solution:**
- Store locally (not in public repo)
- Add note in metadata: "For personal study only"
- Don't share with others without permission

---

## Template Summary

When you add a new material, you need:

```
context-and-references/[TYPE]/[COLLEAGUE-NAME]/
├── document.pdf                    (or exposé.pdf, thesis.pdf)
├── metadata.txt                    (Essential: who/what/when/where)
└── notes.md                        (Recommended: your analysis)
```

Then update:
- `REFERENCE-CATALOG.md` — Add entry to table
- Optionally create comparative analysis file after 3+ materials

---

## Minimal vs. Thorough Approach

**Minimal (5 minutes per material):**
- Add PDF
- Add metadata.txt
- Update catalog
- Done

**Thorough (30 minutes per material):**
- Add PDF
- Add metadata.txt
- Add detailed notes.md with analysis
- Update catalog with key insights
- Extract statistics

**Recommended:** Start minimal, then add notes.md when you have time.

---

**Ready to add your first reference? Start with an exposé from a colleague in your program!**
