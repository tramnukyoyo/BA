# CLAUDE.md — Project Rules & Conventions

## Project Context

**Bachelor Thesis Topic:** Wasserstoffinfrastruktur in globalen Lieferketten
**English Title:** Hydrogen Infrastructure in Global Supply Chains: Implementation Strategies and Challenges

**Primary Deliverable:** High-quality Exposé for professor approval, followed by full thesis

---

## 1. Language Protocol

- **Interaction:** English
- **Thesis Output:** German (Academic German, modern active voice)
  - Example: "Ich analysiere..." instead of "Es wird analysiert"
  - Formal register, precision over colloquialism
  - Consistent terminology throughout

---

## 2. Tech Stack

- **Typesetting:** LaTeX (university template provided in `/template`)
- **Bibliography:** BibTeX with Harvard citation style
- **Version Control:** Git (atomic commits per work session)
- **Source Management:** PDFs and text snippets in `/literature` with summaries

---

## 3. Citation Style

- **Format:** Harvard Style (author-date)
- **Management:** Consistent bibliography file
- **In-text:** (Author Year) format
- **References:** Alphabetical, complete metadata

---

## 4. Workflow: Source-Driven Drafting

- You (user) provide: PDFs, text excerpts, research findings
- I (Claude) analyze and integrate into draft sections
- Iterative refinement: feedback → revise → commit
- All sources logged in `/literature` with key quotes and summaries

---

## 5. GSD Mode

- **Task Tracking:** TODO.md (single source of truth)
- **Work Structure:** Sprints (14-day cycles for Exposé, then thesis chapters)
- **Session Protocol:** Every session starts with sprint status update
- **Commits:** Atomic — each meaningful work unit gets a commit
- **Progress:** TODO.md updated before each session transition

---

## Folder Structure

```
.
├── expose/                  # Exposé in progress
├── thesis/                  # Full thesis chapters (after approval)
├── literature/              # Source summaries, key quotes, PDFs metadata
├── template/                # University LaTeX template
├── scripts/                 # Automation (bibliography management, etc.)
├── TODO.md                  # Sprint task tracking
├── CLAUDE.md                # This file
└── .planning/               # GSD planning artifacts (optional)
```

---

## Interaction Checklist

Before each session:
- [ ] Review current sprint status in TODO.md
- [ ] Confirm next task priority
- [ ] Check for new source materials in `/literature`

After each work block:
- [ ] Update TODO.md with completed tasks
- [ ] Commit changes with clear message
- [ ] Document any findings or decisions

---

**Last Updated:** Session Start (2026-01-31)
