# HRS Thesis Framework Design Document

**Purpose:** Design the bullet-point framework to replace the text-based concept map in the exposé

**Status:** Design phase - ready for implementation in LaTeX

**Target Integration:** In `expose_bachelor.tex` after bibliography section (replacing current Concept Map section)

---

## Design Decision: Hierarchical Outline (Option A)

The hierarchical outline structure is selected because:
- **Clear visual hierarchy** - Easy for readers to scan and understand thesis structure
- **Reduces complexity** - Simpler than the current text-box format
- **Mappable** - Each framework section clearly maps to 1-2 core papers
- **Professional** - Standard academic format, no TikZ complexity needed
- **Flexible** - Easy to modify during thesis writing

---

## Framework Structure

### Main Title
**Thesis Framework: Wasserstofftankstellen-Implementierung und Herausforderungen**
(Hydrogen Refueling Stations: Implementation and Challenges)

### Subtitle
Strategien zur Überwindung regulatorischer, logistischer und technischer Hürden im globalen Kontext
(Strategies for Overcoming Regulatory, Logistical, and Technical Barriers in Global Context)

---

## Three Core Dimensions

### Dimension 1: HERAUSFORDERUNGEN (Challenges)
**Goal:** Identify the three main barrier categories the thesis addresses

```
HERAUSFORDERUNGEN (Challenges)
│
├─ Regulatorische Hürden (Regulatory Barriers)
│  └─ Standards, Zertifizierung, grenzüberschreitende Harmonisierung
│     [Core Paper #6: Regulatory Frameworks & Standards]
│     [Core Paper #10: EU Policy & Institutional Context]
│
├─ Logistische Hürden (Logistical Barriers)
│  └─ H₂-Transport, Versorgungskette-Integration, Speicherung
│     [Core Paper #1: Supply Chain Integration]
│     [Core Paper #2: Logistical & Technical Challenges]
│
└─ Technische Hürden (Technical Barriers)
   └─ Zuverlässigkeit, Wartung, Kompressor- und Kühltechnologie
      [Core Paper #2: Logistical & Technical Challenges]
      [Core Paper #5: Technical Reliability & Maintenance]
```

### Dimension 2: ANALYSE-FRAMEWORK (Analysis Framework)
**Goal:** Show how thesis analyzes and addresses the challenges

```
ANALYSE-FRAMEWORK (How we analyze the challenges)
│
├─ Räumliche Planung & Optimierung (Spatial Planning & Optimization)
│  └─ Standortwahl, Netzwerktopologie, Korridor-basierte Deployment
│     [Core Paper #3: Spatial Planning & Corridor Optimization]
│     [Core Paper #7: Strategic Network Design]
│
├─ Wirtschaftliche Bewertung (Economic Assessment)
│  └─ CAPEX/OPEX, NPV, ROI, Rentabilitäts-Szenarien
│     [Core Paper #4: Economic Viability & Cost-Benefit Analysis]
│     [Core Paper #9: Techno-Economic Literature Reviews]
│
└─ Globaler Marktkontext (Global Market Context)
   └─ Regionale Deployment-Trends, strategische Unterschiede
      [Core Paper #8: Global Market Insights]
      [Core Paper #9: Techno-Economic Literature Reviews]
```

### Dimension 3: INTEGRATIONS-SZENARIEN (Integration Scenarios)
**Goal:** Show how HRS integrate into existing infrastructure under different models

```
INTEGRATIONS-SZENARIEN (Integration Scenarios)
│
├─ Korridor-basiert (Corridor-Based)
│  └─ HRS entlang Hauptverkehrsachsen (z.B. TEN-T-Netzwerk in EU)
│     [Core Paper #3: Spatial Planning]
│     [Core Paper #10: EU Policy Context]
│
├─ Urbane Cluster (Urban Clusters)
│  └─ Stadtnahe HRS-Netzwerke für Busse, Taxis, Flotten
│     [Core Paper #7: Strategic Network Design]
│     [Core Paper #8: Global Market Insights]
│
└─ Industrie-Hubs (Industrial Hubs)
   └─ Hafen- und Logistikzentren für schwere Nutzfahrzeuge
      [Core Paper #1: Supply Chain Integration]
      [Core Paper #8: Global Market Insights]
```

---

## Integration with 5 Thesis Focus Areas

The framework maps to the original 5 thesis focus areas:

| Thesis Focus Area | Framework Dimension | Relevant Papers |
|---|---|---|
| **1. Regulatorische Hürden** | Dimension 1 + Dimension 2 | #6, #10 |
| **2. Logistische Hürden** | Dimension 1 + Dimension 2 | #1, #2 |
| **3. Technische Hürden** | Dimension 1 + Dimension 2 | #2, #5 |
| **4. Szenarien für Integration** | Dimension 3 | #3, #7, #8 |
| **5. Kosten-Nutzen-Bewertung** | Dimension 2 | #4, #9 |

---

## LaTeX Implementation

### Current Concept Map (TO BE REPLACED)
Lines 295-367 in `expose_bachelor.tex`

### New Framework Section (REPLACEMENT)

```latex
\section*{Konzeptioneller Rahmen}
\addcontentsline{toc}{section}{Konzeptioneller Rahmen}

Die Arbeit strukturiert sich entlang von drei Dimensionen der HRS-Implementierung:

\subsection*{1. Herausforderungen (Challenges)}

Die Implementierung von Wasserstofftankstellen steht vor drei Haupthürden:

\begin{itemize}
\item \textbf{Regulatorische Hürden:} Fragmentierung von Standards (ISO, nationale
Vorschriften), Zertifizierungsprozesse, und grenzüberschreitende Regelungslücken
\cite{RegPaper6,RegPaper10}

\item \textbf{Logistische Hürden:} H\textsubscript{2}-Transportmodi (Pipeline, Trailer,
On-site Produktion), Versorgungskettenintegration von Produktion zu HRS, und
Speicher-/Dispensing-Technologien \cite{LogPaper1,LogPaper2}

\item \textbf{Technische Hürden:} Zuverlässigkeit und Wartungsanforderungen,
Kompressor- und Kühltechnologie, sowie Skalierbarkeit und Modularität
\cite{TechPaper2,TechPaper5}
\end{itemize}

\subsection*{2. Analyse-Framework (Analysis Framework)}

Zur Analyse dieser Herausforderungen nutzt die Arbeit drei komplementäre Methoden:

\begin{itemize}
\item \textbf{Räumliche Planung \& Optimierung:} Standortwahl, Netzwerk-Topologie
und Deployment-Szenarien für unterschiedliche geografische Kontexte
\cite{SpatialPaper3,NetworkPaper7}

\item \textbf{Wirtschaftliche Bewertung:} Kostenstruktur-Analyse (CAPEX/OPEX),
Net Present Value (NPV), Return on Investment (ROI), sowie Sensitivitätsanalyse
für verschiedene Finanzierungsszenarien \cite{EconPaper4,ReviewPaper9}

\item \textbf{Globaler Marktkontext:} Regionale Deployment-Trends, strategische
Unterschiede zwischen Europa, Asien-Pazifik und Australien, sowie Markt-Treiber
und Adoption-Barrieren \cite{MarketPaper8,ReviewPaper9}
\end{itemize}

\subsection*{3. Integrationsszenarien (Integration Scenarios)}

Die Thesis untersucht drei Hauptszenarien für die Integration von HRS in bestehende
Infrastrukturen:

\begin{itemize}
\item \textbf{Korridor-basiert:} HRS entlang von Hauptverkehrsachsen
(z.B. TEN-T-Netzwerk in der EU), mit Fokus auf Long-Haul-Transport
\cite{SpatialPaper3,EUPolicyPaper10}

\item \textbf{Urbane Cluster:} Stadtnahe HRS-Netzwerke für städtische Mobilität
(Busse, Taxis, Flotten), mit kleineren Stationen und höherer Nutzungsfrequenz
\cite{NetworkPaper7,MarketPaper8}

\item \textbf{Industrie-Hubs:} Hafen- und Logistikzentren mit Fokus auf
Schwertransport und lokale Versorgungsketten \cite{SupplyChainPaper1,MarketPaper8}
\end{itemize}

\vspace{0.5cm}

\noindent\textbf{Synthese:} Aus der Analyse dieser drei Dimensionen und
Szenarien werden regionsabhängige Strategien und Handlungsempfehlungen
abgeleitet, die Investoren, Policymaker und Infrastrukturbetreiber bei der
effizienten HRS-Implementierung unterstützen.
```

---

## Paper Mapping Instructions

**When integrating 10 core papers, use these citation keys:**

| Content Area | Citation Key | Usage in Framework |
|---|---|---|
| #1 Supply Chain Integration | SupplyChainPaper1 | Integrationsszenarien (Industrie-Hubs) |
| #2 Logistical & Technical | LogPaper2 | Herausforderungen (Logistik + Technisches) |
| #3 Spatial Planning | SpatialPaper3 | Analyse-Framework (Räumliche Planung) |
| #4 Economic Viability | EconPaper4 | Analyse-Framework (Wirtschaftliche Bewertung) |
| #5 Technical Reliability | TechPaper5 | Herausforderungen (Technisches) |
| #6 Regulatory Frameworks | RegPaper6 | Herausforderungen (Regulatorisches) |
| #7 Strategic Network Design | NetworkPaper7 | Analyse-Framework (Netzwerk) + Szenarien |
| #8 Global Market Insights | MarketPaper8 | Analyse-Framework (Markt) + Szenarien |
| #9 Techno-Economic Reviews | ReviewPaper9 | Analyse-Framework (Wirtschaft + Markt) |
| #10 EU Policy Context | EUPolicyPaper10 | Herausforderungen (Regulatorisches) + Szenarien |

---

## Advantages Over Current Concept Map

| Aspect | Current (Text Boxes) | New (Hierarchical Outline) |
|---|---|---|
| **Clarity** | Confusing structure, hard to scan | Clear hierarchy, easy to follow |
| **Readability** | Complex visual layout | Clean bullet-point format |
| **Maintenance** | Hard to update, TikZ complexity | Simple text, easy to modify |
| **Paper Integration** | Difficult to map papers | Clear citation placement |
| **Space Efficiency** | Takes 1.5 pages | Takes 0.75-1 page |
| **Professional Look** | Generic boxes | Academic standard format |

---

## Testing the Framework

After implementing in LaTeX, verify:
- [ ] All 10 papers are cited in framework section
- [ ] Each paper appears in at least one relevant section
- [ ] No citations to "TBD" or placeholder text
- [ ] Hierarchical nesting is clear (main bullet → sub-bullet → description)
- [ ] All German text is grammatically correct
- [ ] Framework integrates logically with Chapter 1-6 of thesis

---

## Alternative Layouts (Reference Only)

### Option B: Process Flow (Not Selected)
Shows HRS deployment as a sequence:
1. IDENTIFY BARRIERS → 2. DEVELOP SCENARIOS → 3. EVALUATE VIABILITY → 4. RECOMMEND STRATEGIES

**Disadvantage:** Linear format doesn't capture the interconnected nature of regulatory, logistical, technical, and economic factors

### Option C: Matrix View (Not Selected)
Rows = Regulatory | Logistical | Technical | Economic
Columns = Barriers | Scenarios | Economics

**Disadvantage:** Matrix becomes crowded with 10 papers, harder to read

---

## Final Notes

- **Status:** Ready for LaTeX implementation
- **Timeline:** Implement on Day 7 of Phase 1 Rebuild
- **Dependencies:** Requires 10 finalized core papers with citation keys
- **Integration:** Replace lines 295-367 in `expose_bachelor.tex`
- **Review:** User should review framework alignment with thesis narrative before compilation

**Last Updated:** 2026-02-13
**Version:** 1.0 - Final Design

