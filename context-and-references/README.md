# Context and References — Colleague Materials & Thesis Examples

This folder contains reference materials from colleagues, including completed theses, exposés, and thesis proposals. These serve as structural and stylistic references for your own work.

---

## Purpose

Draw inspiration and learn best practices from:
- **Structure & Organization** — How do others organize chapters, sections?
- **Table of Contents** — Which topics are typically included? How are they weighted?
- **Page Counts** — How many pages for different components (intro, lit review, findings)?
- **Visual Presentation** — Charts, figures, diagrams, formatting
- **Academic Register** — Language tone, terminology, citation density
- **Formatting & Layout** — Margin conventions, font choices, headers
- **Abstract & Introductions** — How do others hook the reader?

---

## Folder Structure

```
context-and-references/
├── README.md                          (This file)
├── REFERENCE-CATALOG.md               (Index of all materials)
│
├── exposés/                           (Colleague exposés)
│   ├── [colleague-name]/
│   │   ├── exposé.pdf
│   │   ├── notes.md                   (Your analysis of structure/approach)
│   │   └── metadata.txt               (Topic, length, institution)
│   └── [another-colleague]/
│
├── bachelor-theses/                   (Completed bachelor theses)
│   ├── [colleague-name]/
│   │   ├── thesis.pdf
│   │   ├── analysis.md                (Structure, chapter breakdown)
│   │   └── metadata.txt
│   └── [another-colleague]/
│
├── thesis-proposals/                  (Proposals & planning docs)
│   ├── [colleague-name]/
│   │   ├── proposal.pdf
│   │   ├── notes.md
│   │   └── metadata.txt
│   └── [another-colleague]/
│
└── master-theses/                     (If available for deeper reference)
    ├── [colleague-name]/
    │   ├── thesis.pdf
    │   ├── analysis.md
    │   └── metadata.txt
    └── [another-colleague]/
```

---

## How to Use This Folder

### 1. **When Adding a New Reference Material**

Create a folder with your colleague's name:
```
context-and-references/exposés/Anna_Mueller/
```

Inside, add:
- **exposé.pdf** (or thesis.pdf, proposal.pdf) — The actual document
- **metadata.txt** — Basic info about the work
- **notes.md** — Your analysis and observations

### 2. **What to Document in `notes.md`**

When analyzing a reference work, note:

```markdown
# Analysis: [Colleague Name] — [Topic]

## Structural Observations
- **Total Pages:** [X]
- **Chapter/Section Breakdown:**
  - Intro: X pages
  - Lit Review: X pages
  - Methodology: X pages
  - Results/Analysis: X pages
  - Conclusion: X pages
  - Bibliography: X pages

## Table of Contents Layout
[Copy/describe the TOC structure]

## Formatting & Presentation
- Font: [Times New Roman, etc.]
- Margins: [Standard]
- Line spacing: [1.5, double]
- Images/Figures: [Count and types]
- Tables: [Count and purpose]

## Academic Register & Language
- Tone: [Formal, conversational, technical]
- Sentence structure: [Complex, varied, simple]
- Use of passive voice: [Frequent, moderate, rare]
- Terminology: [Highly specialized, accessible, mixed]

## Key Strengths
- [What works well in this thesis?]
- [What could you adopt?]

## Areas to Learn From
- [Structural innovations]
- [Effective use of visuals]
- [Strong opening/closing]

## Your Takeaways
- Action items to apply to your own work
```

### 3. **Update the Catalog**

After adding a new reference, update `REFERENCE-CATALOG.md` with an entry.

---

## Reference Catalog Entry Template

When you add materials, include this metadata:

```
### [Colleague Name] — [Topic/Title]

**Type:** Exposé / Bachelor Thesis / Thesis Proposal / Master Thesis
**Subject Area:** [e.g., Renewable Energy, Supply Chain, Environmental Engineering]
**Institution:** [University]
**Year:** [2024/2025]
**Pages:** [X]
**Folder:** `context-and-references/[type]/[colleague-name]/`

**Why This Reference:**
[1-2 sentences on what makes this useful for your work]

**Key Elements to Study:**
- [ ] Structure
- [ ] Table of Contents
- [ ] Visual presentation
- [ ] Literature review approach
- [ ] Methodology
- [ ] Results presentation

**Status:** [ ] Not yet analyzed | [x] Analyzed — see notes.md
```

---

## Quick Analysis Checklist

When reviewing a reference material, quickly assess:

- [ ] **Structure:** Clear section progression?
- [ ] **Scope:** How much ground does it cover in X pages?
- [ ] **Balance:** Are sections well-proportioned?
- [ ] **Readability:** Is it easy to follow? Good use of headings?
- [ ] **Visuals:** Effective use of figures, tables, diagrams?
- [ ] **Citations:** Density and consistency of references?
- [ ] **Opening:** Does the introduction hook you? How?
- [ ] **Closing:** Does the conclusion synthesize well?

---

## Example Entry (For Your Hydrogen Thesis)

**Type:** Exposé
**Subject:** Hydrogen Infrastructure (or similar energy topic)
**Pages:** 5-8 typical for exposé
**Key Questions:**
- How many pages does the motivation take?
- How is the research question framed?
- How long is the literature review section?
- How detailed is the methodology?
- How are future outcomes/timeline presented?

---

## Tips for Effective Comparison

1. **Compare within categories:** Compare your exposé structure to other colleague exposés (not to full theses)
2. **Adapt, don't copy:** Use references to understand conventions, not to copy sections
3. **Note outliers:** If a colleague's work stands out, ask why—what makes it effective?
4. **Build a mental model:** After reviewing 3-5 references, patterns emerge—use those patterns
5. **Document as you go:** Don't wait until the end to analyze

---

## Storage of PDF Files

Since PDFs can be large, consider:
- **Storing locally:** Keep originals in this folder
- **Backup:** Periodically backup to external storage
- **Naming convention:** `[Name]_[Type]_[Year].pdf` (e.g., `Mueller_Exposé_2024.pdf`)

---

## Git and Large Files

If PDFs are large (>50MB total per colleague), consider:
- Adding a `.gitignore` entry for large PDFs (store separately)
- Or: Storing only metadata + links to cloud storage (Google Drive, OneDrive)

Example `.gitignore`:
```
context-and-references/**/*.pdf
context-and-references/**/*.docx
```

Then include a `drive-link.txt` or similar with cloud storage URLs.

---

**How to Get Started:**
1. Gather colleague materials (exposés, theses)
2. Create folders in the appropriate subdirectories
3. Add PDFs + metadata.txt files
4. Analyze each and add notes.md
5. Update REFERENCE-CATALOG.md
6. Commit to git

---

**Last Updated:** 2026-01-31 (Initialization)
