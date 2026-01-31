# Exposé Draft — Guidance & Next Steps

**Created:** 2026-01-31
**Topic:** Wasserstoffinfrastruktur in globalen Lieferketten
**Status:** First Complete Draft (Ready for Customization)

---

## 📄 Files Created

1. **EXPOSE_DRAFT.md** — Markdown version of full exposé (readable, editable)
2. **expose.tex** — LaTeX-formatted version (ready for PDF compilation)
3. **STRUCTURE_ANALYSIS.md** — Reference document analyzing colleague's exposé structure
4. **DRAFT_NOTES.md** — This guidance document

---

## ✅ What's Included in Your Draft

### ✓ Seven Mandatory Sections
- [x] **Ausgangslage** (1.5 pages) — Context on hydrogen as energy carrier, global supply chains
- [x] **Problemstellung** (1.5 pages) — Research gap, infrastructure barriers (78% adoption blockers)
- [x] **Forschungsfragen** (3 questions) — Hierarchical research questions with proper formulation
- [x] **Zielsetzung** (1 page) — Clear objectives showing how chapters address questions
- [x] **Gliederung** (8 chapters, 28 subsections) — Complete thesis outline
- [x] **Literaturverzeichnis** (11 sources) — Harvard-formatted bibliography
- [x] **Concept Map** — TikZ visual flowchart showing thesis logic

### ✓ Academic Standards
- ✓ Formal German with active voice ("werden erläutert")
- ✓ 3-4 citations per major section
- ✓ Statistics integrated (500% demand growth, 78% adoption barriers)
- ✓ Footnote citations in LaTeX
- ✓ Professional structure following Aaron Chhen's model

---

## 🎯 What YOU Need to Customize

### 1. Personal Information (CRITICAL)
- [ ] Replace `[Ihr Name]` with your actual name
- [ ] Replace `[Ihre Matrikelnummer]` with your matriculation number
- [ ] Update date if needed (currently "Januar 2026")

**Locations to update:**
- `expose.tex` — Lines in title page (around lines 30-35)
- `EXPOSE_DRAFT.md` — If you use markdown

### 2. Research Questions (IMPORTANT)
The 3 research questions provided are **templates**. Consider:
- Do they align with your actual research interest?
- Are they specific enough?
- Are they answerable with the proposed chapter structure?

**Current questions focus on:**
1. Technical/economic viability of H₂ infrastructure scenarios
2. Governance and coordination mechanisms
3. Sustainability trade-offs

If you want to adjust these, update:
- Forschungsfragen section
- Concept Map (visual relationships may change)
- Gliederung (chapter organization may need adaptation)

### 3. Chapter Outline (IMPORTANT)
The 8-chapter structure with 28 subsections is **comprehensive** but can be condensed:

**Current weight:**
- Ch 2-3: Foundations & state of art (15 subsections)
- Ch 4-5: Implementation & governance (8 subsections)
- Ch 6: Sustainability (4 subsections)
- Ch 7-8: Discussion & conclusion (1 subsection each)

**If this is too long**, consider:
- Merging Chapters 4 & 5 (Scenarios + Governance)
- Combining Chapters 7 & 8 (Discussion + Conclusion)
- Reducing sub-subsections (2-3 levels max recommended)

### 4. Bibliography (IMPORTANT)
The 11 sources provided are **real, but generic**. You should:
- [ ] Verify these references actually exist (or replace with sources you've found)
- [ ] Add at least 3-5 sources specific to **hydrogen infrastructure** (e.g., H2Future, HyDelta, HEAVENN projects)
- [ ] Add sources on **global supply chain governance** (your topic's unique angle)
- [ ] Add sources on **policy frameworks** (EU Hydrogen Strategy, etc.)

**Action:** Review in `/literature` folder for sources you've already gathered. Update bibliography.

### 5. Concept Map (OPTIONAL)
The TikZ concept map is **functional** but can be refined:
- Current version shows linear flow (Intro → Theory → Cases → Scenarios → Governance → Sustainability → Discussion → Conclusion)
- You may want to show more **dependencies** or **feedback loops**
- If visual doesn't match your actual thesis logic, modify in the LaTeX file (TikZ code around line 400)

---

## 🔧 How to Use the LaTeX File

### Prerequisites
- LaTeX installation (MikTeX, TexLive, or Overleaf)
- Ensure `pdflatex` can process German characters

### Compilation
```bash
pdflatex expose.tex
```

This will generate `expose.pdf`.

### Integration with University Template
If your university has a specific LaTeX template:

1. **Copy the preamble structure** from `expose.tex` (lines 1-30)
2. **Replace title page section** with your template's title format
3. **Keep content sections** (Ausgangslage through Literaturverzeichnis)
4. **Use your template's bibliography style** (currently uses `authoryear`)

---

## 🚀 Next Steps (Recommended Workflow)

### Phase 1: Personalization (30 min)
1. [ ] Add your name, matriculation number, date
2. [ ] Review research questions — do they excite you?
3. [ ] Adjust chapter outline if needed

### Phase 2: Literature Review (2-3 hours)
1. [ ] Search for H₂ infrastructure papers (Google Scholar, ResearchGate)
2. [ ] Find 5-8 recent sources (2020-2026)
3. [ ] Extract 1-2 key quotes for Ausgangslage and Problemstellung
4. [ ] Update bibliography with real sources

**Recommended searches:**
- "hydrogen infrastructure global supply chain"
- "hydrogen export strategies countries"
- "hydrogen governance international"
- "hydrogen pipeline projects Europe Asia"

### Phase 3: Content Refinement (2-4 hours)
1. [ ] Read through entire draft
2. [ ] Highlight areas that don't match YOUR interests
3. [ ] Adjust Ausgangslage to reflect YOUR angle on the topic
4. [ ] Rewrite 1-2 sentences in Problemstellung to sharpen research gap

### Phase 4: Polish & Feedback (1 hour)
1. [ ] Compile LaTeX to PDF
2. [ ] Check formatting, page breaks, references
3. [ ] Have someone proofread for clarity
4. [ ] Submit to advisor for feedback

---

## 📊 Quality Checklist

Before submitting to your professor, verify:

- [ ] **Title Page:** Name, matriculation number, date correct
- [ ] **Structure:** All 7 mandatory sections present
- [ ] **Research Questions:** 3 questions, open-ended, hierarchical
- [ ] **Bibliography:** 10+ sources, all cited in text, Harvard format
- [ ] **Concept Map:** Visual representation of thesis flow
- [ ] **Language:** Formal German, active voice, no colloquialisms
- [ ] **Citations:** Every statistic/fact has a superscript footnote
- [ ] **Length:** Approximately 7-8 pages (check page count in PDF)
- [ ] **Formatting:** Professional, consistent fonts/sizes, proper margins

---

## ⚠️ Common Mistakes to Avoid

❌ **Don't:**
- Forget to personalize (keep placeholder names)
- Use more than 3-4 levels of chapter numbering
- Make research questions too narrow/yes-no oriented
- Cite sources you haven't actually read
- Use passive voice throughout ("es wird analysiert")
- Make chapters without addressing research questions
- Ignore the concept map (it helps structure thinking)

✅ **Do:**
- Review your draft multiple times before submitting
- Engage with each source you cite
- Show research questions → chapter mapping clearly
- Use active voice ("Ich analysiere...")
- Include specific numbers/statistics where possible
- Explain WHY each chapter matters for answering the research questions

---

## 📝 Tips for Custom Refinement

### To Strengthen Ausgangslage:
- Add a recent statistic on H₂ market growth or investments
- Include 1-2 compelling examples of H₂ projects (e.g., Germany's H₂ facilities, Australia's green H₂ export plans)
- Define your unique angle (is it cost? sustainability? governance? global coordination?)

### To Sharpen Problemstellung:
- Identify 1-2 **specific companies or projects** facing infrastructure barriers
- Cite real studies/reports (not generic)
- State clearly: "This thesis addresses [gap] by [approach]"

### To Make Zielsetzung Compelling:
- Explain the **significance** of answering each research question
- Show how thesis **contributes to practice** (not just theory)
- Link back to motivation in Ausgangslage

### To Improve Gliederung:
- Ensure **each chapter** directly answers one research question
- Avoid chapters that don't connect to your research questions
- Balance page distribution (no single chapter should dominate)

---

## 💡 Questions to Consider

As you refine the draft, ask yourself:

1. **Relevance:** Why is hydrogen infrastructure in global supply chains important RIGHT NOW?
   - Climate targets? Energy transition? Cost competition? Geopolitics?

2. **Uniqueness:** What angle is NOT well-covered in existing research?
   - Governance mechanisms? Cost modeling? Sustainability metrics? Geographic comparison?

3. **Feasibility:** Can I actually answer my research questions in a bachelor thesis?
   - Is scope reasonable? (Too broad = unfocused; too narrow = weak)

4. **Structure:** Do my 8 chapters logically build toward answering RQs?
   - Does Chapter 2 lay groundwork? Chapters 3-4 present evidence? Chapters 5-6 analyze implications?

---

## 📚 Resources for Further Development

### For Hydrogen Research:
- **Global Hydrogen Review** (IEA, annual) — Official global overview
- **Hydrogen Council Reports** — Industry perspective
- **National H₂ Strategies** (Germany, Japan, Australia, etc.) — Policy context

### For Supply Chain Methodology:
- **Supply Chain Management Review** — Journal for SCM concepts
- **International Journal of Production Economics** — Cost/efficiency analysis
- **Networks/Governance literature** — For coordination mechanisms

### For Academic Writing:
- **CLAUDE.md** in your project — Your project's specific conventions
- Colleague's exposé (Aaron Chhen) — Structural reference

---

## 📞 Final Notes

- This draft is **80% complete** — It requires your personal touch and research customization
- The structure is **validated** — Based on successful exposé from peer
- The content is **realistic** — But you must verify sources and add your specific context
- **Quality depends on YOUR engagement** — Generic draft → excellent exposé requires your input

**Next action:** Review the draft, identify 3 things to adjust, then proceed with Phase 1 of Next Steps.

---

**Last Updated:** 2026-01-31
