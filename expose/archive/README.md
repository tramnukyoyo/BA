# Expose Archive

**Status:** Outdated files and compilation artifacts (Phase 1 Rebuild)

This folder contains files that are no longer actively used in the Phase 1 Exposé rebuild:

## Archived Files

### Old LaTeX Versions
- `expose.tex` - Original exposé version (general H₂ infrastructure focus)
- `exposé.tex` - French language version
- `expose.pdf`, `exposé.pdf` - Old compiled PDFs
- Compilation artifacts: `*.aux`, `*.log`, `*.out`, `*.toc`, `*.bcf`, `*.bbl`, `*.synctex`, `*.run.xml`

### Old Documentation/Drafts
- `DRAFT_NOTES.md` - Development notes from original phase
- `EXPOSE_DRAFT.md` - Draft content (old structure)
- `EXPOSE_BACHELOR.md` - Old bachelor thesis outline
- `outline.md` - Preliminary outline
- `research-question.md` - Old RQ formulation
- `STRUCTURE_ANALYSIS.md` - Old structure analysis
- `expose_final.pdf` - Previous final version

### Test/Build Logs
- `compile_test.log`, `compile_test2.log` - LaTeX compilation tests
- `texify.log` - Build process log

## What to Keep

**Active files in root `expose/` folder:**
- `expose_bachelor.tex` - Current main LaTeX document (HRS-focused, UPDATED)
- `references_h2_CORE.bib` - NEW core bibliography (9 HRS papers)
- `references_h2.bib` - OLD bibliography (kept as supplementary reference)
- `FRAMEWORK_DESIGN.md` - Framework design reference

## What Changed in Phase 1 Rebuild

**Content shift:** General hydrogen infrastructure → HRS-specific implementation

**Key updates:**
- expose_bachelor.tex: Restructured with HRS-specific focus (Ausgangslage, Problemstellung, RQs, Gliederung)
- references_h2_CORE.bib: NEW file with 9 peer-reviewed HRS papers (2020-2024)
- Bibliography reference: Updated to use references_h2_CORE.bib

## How to Use Archived Files

### Option 1: Reference Only
If you need to check old content for context:
1. Read files from `archive/` folder
2. Do NOT include in LaTeX compilation

### Option 2: Delete
Once Phase 1 is confirmed complete:
1. Delete entire `archive/` folder
2. Can always restore from git history if needed

---

**Created:** 2026-02-13 (Phase 1 Rebuild - Cleanup)
**Size:** Reduced root folder from 30+ files to 6 active files
