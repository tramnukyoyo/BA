# Genovese et al. 2023 - Paper Summary: HRS Standards and Regulations

## 1. PAPER BASICS

**Title:** Current standards and configurations for the permitting and operation of hydrogen refueling stations

**Authors:** Matteo Genovese, Viviana Cigolotti, Elio Jannelli, Petronilla Fragiacomo

**Institutions:** University of Calabria, ENEA Italy, University of Naples "Parthenope"

**Journal:** International Journal of Hydrogen Energy, Volume 48 (2023), pages 19357-19371

**DOI:** 10.1016/j.ijhydene.2023.01.324

**Publication Date:** March 2, 2023

**Type:** Comprehensive regulatory and standards review

**Focus:** Complete landscape of HRS standards for design, operation, safety, and permitting at global, European, and national levels

---

## 2. KEY CONTRIBUTIONS

This paper fills a critical regulatory gap by:

1. **Comprehensive standards overview:** First systematic analysis of HRS equipment and operating standards
2. **Multi-level regulation mapping:** Global (ISO/IEC/SAE) + European (CEN/CENELEC) + National (Italy) frameworks
3. **Safety engineering foundation:** Detailed hydrogen safety principles for standard development
4. **Equipment lifecycle coverage:** Production → Storage → Compression → Dispensing standards
5. **Implementation barriers identified:** Regulatory gaps and obstacles to HRS deployment
6. **Permitting guidance:** Practical insights for HRS developers and regulators

---

## 3. HYDROGEN SAFETY FUNDAMENTALS

### Physical Properties Relevant to Standards

| Property | Hydrogen | Methane | Gasoline |
|---|---|---|---|
| Lower Heating Value (kWh/kg) | 33.33 | 13.89 | 12.36 |
| Flame Temperature (K) | 2318 | 2148 | 2473 |
| Flammable Range (vol % in air) | 4.0-75.0 | 5.3-15.0 | 1.0-7.6 |
| Ignition Energy (mJ) | 0.02 | 0.29 | 0.24 |
| Density Ratio vs Air | 0.07 | 0.55 | 4.0 |

**Key Safety Characteristics:**
- ✅ **Advantage:** Low density → rapid dispersion, doesn't accumulate near ground
- ⚠️ **Challenge:** Wide flammability range (4-75%), low ignition energy
- ⚠️ **Challenge:** Rapid flame propagation, invisible flames (burns in UV spectrum)

### Critical Hazard Phenomena

**Deflagration-to-Detonation Transition (DDT):**
- Flame accelerates from subsonic to supersonic speeds (up to 800 m/s)
- Pressure spike reaches 30× ambient pressure
- Most severe hydrogen hazard in confined spaces

**Pressure-Dependent Safety Distance:**
- Storage pressure directly affects hazard distance
- At 700 bar: danger distance to 4% hydrogen = 42 m
- At 1 bar: danger distance to 4% hydrogen = 2 m
- Relationship follows square-root pressure dependency (Table 2, paper)

**Emergency Response Sequence:**
1. Hydrogen release → 2. Dispersion → 3. Confined accumulation (critical) → 4. Ignition → 5. Fire/explosion/DDT

---

## 4. HRS CONFIGURATIONS & EQUIPMENT FRAMEWORK

### Compressed Gaseous Hydrogen (GH2) Stations

**Supply Options:**
- Tube trailers (200-500 bar)
- Pipelines (typically 20 bar)
- On-site production: Steam Methane Reforming (SMR) or Water Electrolysis (WE) at 20 bar

**Station Components:**
1. **Hydrogen Source** (20-50 bar inlet)
2. **Compressors** (increase to ~950 bar for storage)
3. **Storage Tanks** (horizontal/vertical, ~350-700 bar)
4. **Pre-cooling** (to ~-40°C)
5. **High-Pressure Buffer Tanks (HPBT)** (mitigate pulsing)
6. **Dispenser** (delivers at 700 bar)

**Typical Daily Capacity:** 100-520 kg compressed GH2

### Liquid Hydrogen (LH2) Stations

**Supply:** Trucked cryogenic tanks (~4 tons/delivery)

**Station Components:**
1. **Cryogenic Storage** (insulated, -253°C, 0.6-35 MPa)
2. **Boil-off Handler** (compressor for headspace gas)
3. **Cryogenic Pump** (optional, for high-pressure path)
4. **Evaporator** (gasify liquid)
5. **Pre-cooler** (~-40°C dispenser approach)

**Critical Challenge:** Boil-off losses (1-3%/day for small tanks), air moisture ingress risk

**Typical Daily Capacity:** >1000 kg LH2 (more dense than GH2)

### On-Site Production Configurations

**Alkaline Water Electrolysis (WE):**
- Lower cost, mature technology
- Typical production: 60 kg/day units
- Eliminates external supply dependency
- Suitable for decentralized networks

**Advantages:** Reliability, low breakdowns, reduced waste

**Challenges:** Complexity, additional safety systems, higher capital if high-capacity needed

---

## 5. GLOBAL STANDARDS FRAMEWORK

### ISO (International Standards Organization)

**Relevant Technical Committees:**
- ISO/TC 197 — Hydrogen technologies (PRIMARY for HRS)
- ISO/TC 220 — Cryogenic vessels
- ISO/TC 58 — Gas cylinders
- ISO/TC 22/SC 41 — Gaseous fuels-specific issues

**Core HRS Standards (ISO 19880 series):**

| Standard | Scope |
|---|---|
| ISO 19880-1 to 19880-9 | General & specific requirements for HRS design, operation, maintenance |
| ISO 14687 | Hydrogen fuel quality - product specifications |
| ISO 19983 | Safety of hydrogen separation and purification systems |
| ISO/TR 15916 | Fundamental safety considerations for hydrogen systems |

**Coverage Areas:**
1. **Production:** On-site hydrogen generation (WE, SMR) + separation/purification
2. **Storage:** Both gaseous and liquid hydrogen systems
3. **Dispensing:** Fueling protocols, equipment specifications
4. **General Applications:** Safety, quality, maintenance procedures

**Status:** LH2 standards more mature; GH2 standards still under development

### IEC (International Electrotechnical Commission)

**Relevant Technical Committees:**
- IEC/TC 31 — Explosion-proof equipment
- IEC/TC 69 — Electrical power transfer for vehicles & trucks
- IEC/TC 105 — Fuel cell technology

**HRS-Applicable Standards:**

| Standard | Application |
|---|---|
| IEC 60079 series | Explosive gas atmospheres (HRS relevant) |
| IEC 80079 series | Equipment for explosive atmospheres |
| IEC 60204 | Safety of machinery - electrical equipment |
| IEC 60529 | Degrees of protection (IP ratings) |

**Focus:** Electrical safety, ignition source prevention, emergency systems

### SAE (Society of Automotive Engineers)

**Primary Committee:** FC Standards Committee

**Critical HRS Standards:**

| Standard | Scope |
|---|---|
| **SAE J2601** | Light-duty vehicle hydrogen fueling protocol (MOST ADOPTED) |
| SAE J2600 | Safety for fueling connection devices |
| SAE J2700 | Hydrogen fuel vehicle terminology |

**SAE J2601 Details:**
- Specifies dispenser-to-vehicle interface protocols
- Defines pressure profiles, flow rates, safety parameters
- Covers self-diagnosis and performance monitoring
- Continuously updated for technology advances

**Status:** Industry standard for safe & interoperable fueling

---

## 6. EUROPEAN STANDARDS FRAMEWORK (CEN/CENELEC)

**Governing Bodies:**
- CEN (European Committee for Standardization) — General standards
- CENELEC (European Committee for Electro-Technical Standardization) — Electrical standards
- **Status:** Voluntary, but member states must consider when implementing EU law

**Relevant Technical Committees:**
- CEN/CLC/TC 6 — Hydrogen (PRIMARY)
- CEN/TC 23 — Transportable gas cylinders
- CEN/TC 69 — Industrial valves
- CEN/TC 197 — Pumps
- CEN/TC 234 — Gas infrastructure
- CEN/TC 235 — Gas pressure regulators
- CEN/TC 236 — Manually operated shut-off valves

**Key European Standards:**

| Category | Standard | Scope |
|---|---|---|
| **Production & Supply** | EN 17533, EN 1797 | Gas supply systems (</>16 bar), hydrogen injection into grid |
| **Storage (Gaseous)** | EN 17533 | Gaseous hydrogen tank specifications |
| **Storage (Liquid)** | EN 1797 | Cryogenic tank requirements, insulation |
| **Compression** | EN 12583 | Hydrogen compressor requirements (under approval) |
| **Dispensing (Outdoor)** | EN 17127 | Outdoor HRS dispensing procedures |
| **Dispensing (FCEV)** | EN 16380, EN 17268 | Vehicle interface connectivity |
| **Hydrogen Quality** | EN 17124 | Hydrogen purity and quality specs |
| **Multifuel** | CEN/CLC Guide 38 | HRS co-located with other alternative fuels |

**Development Status:** Many standards still being drafted or completed; GH2 standards lagging behind LH2

---

## 7. ITALIAN REGULATORY FRAMEWORK

### National Context

**Opportunities:**
- Access to clean energy sources (solar, wind, hydroelectric)
- Existing natural gas infrastructure (repurposing potential)
- Geographic hub for Middle East/Africa hydrogen imports

**Regulatory Framework:**
- **National Decree n. 1657 (Dec 16, 2016):** Implements EU Directive 2014/94/EU
- Recognizes hydrogen as alternative fuel
- Target: HRS network by December 31, 2025

**Critical Gaps:**
- ❌ Liquid hydrogen handling NOT permitted (no standards)
- ❌ Pipeline-supplied hydrogen NOT permitted
- ❌ Methodology for safety distances NOT defined
- ❌ Ventilation strategies NOT addressed

**Oversight:** National Fire Corps (Corpo Nazionale dei Vigili del Fuoco) responsible for safety approvals

### Current Italian Standards Available

| Standard | Scope |
|---|---|
| UNI ISO 14687:2020 | Hydrogen fuel quality - product specifications |
| UNI ISO 19880-1:2020 | Gaseous hydrogen - HRS basic specifications |
| UNI ISO/TR 15916:2018 | Fundamental safety considerations |

**Status:** Limited to 3 core standards; infrastructure still lagging

---

## 8. KEY QUOTES FOR CITATION

**On regulatory gap:**
"The literature lacks a systematic analysis of HRS equipment and operating standards. Researchers, policymakers, and HRS operators could find this information relevant for planning the network's future expansion."

**On hydrogen safety uniqueness:**
"Hydrogen has low ignition energy, a rapid flame speed, poor flame visibility, is colorless and odorless, and has a wide range of flammability...However, since hydrogen has a density that is approximately one-fourteenth that of air, it dissipates swiftly in open regions."

**On global standard status:**
"Notably, a number of standards for different components and equipment are now being defined and are currently under development. LH2 technology seems to have a greater degree of maturity in terms of published standards, but numerous GH2 standards, which cover the majority of the hydrogen use, are in the process of being drafted or completed."

**On SAE J2601 importance:**
"SAE J2601 is a technical standard developed by the SAE that provides specifications for the dispensing of hydrogen fuel to vehicles...Adoption of this standard supports and ensures the safe and efficient transfer of hydrogen, promotes interoperability between hydrogen filling stations and automobiles, and fosters the expansion of the hydrogen fuel cell sector."

**On Italian regulatory obstacles:**
"Despite the enormous potential [for Italy], numerous regulatory and other impediments remain in the way of the full development of green hydrogen in Italy."

---

## 9. HRS OPERATIONAL HAZARDS & STANDARD SAFETY REQUIREMENTS

### Public Incident Database

**Recent Accidents Documented:**
- Santa Clara, CA (2019): Liquid hydrogen truck leak → explosion, 3-month network disruption
- Oslo, Norway (2019): High-pressure storage facility explosion
- Hydrogen Tool Portal: Comprehensive incident database available

**Lesson:** Real-world accidents drive standard updates; standards lag behind operational experience

### Safety Design Approach

**Traditional Risk Assessment:** Limited by insufficient operational data (early market)

**Recommended Approach:** Safety-oriented standards with iterative design verification against acceptance criteria

**Key Safety Systems:**
1. Ventilation (natural/forced) in leak events
2. Ignition source elimination
3. Leak detection & pressure reduction
4. Fire suppression equipment
5. Thermal Pressure Relief Device (TPRD) with correct sizing

**TPRD Design Innovation:** Variable aperture TPRD design being researched to balance flame length vs. storage pressure

---

## 10. CONNECTION TO YOUR THESIS FRAMEWORK

### Dimension 1: Regulatory Barriers

**This paper directly addresses:** Regulatory landscape as barrier to HRS deployment

**Key findings:**
- ✅ Global standards framework exists (ISO/IEC/SAE)
- ✅ European standards largely complete (CEN/CENELEC)
- ⚠️ Major gaps in national regulations (especially Italy)
- ⚠️ Liquid hydrogen permitting obstacles
- ⚠️ Safety distance calculation methodologies not standardized

**For your thesis:** Use to document regulatory complexity as implementation barrier

### Dimension 2: Policy & Institutional Framework

**This paper enables:** Understanding of multi-level regulatory coordination

**Coordination challenge:** Global standard (ISO) → European implementation (CEN) → National adoption (UNI) → Local permitting (Fire Corps)

**Integration gaps:** Standards exist but permitting processes incomplete

### Dimension 3: Technology Readiness & Standards Harmonization

**This paper demonstrates:** Technology readiness varies by component/region

**Status Matrix:**
- ✅ GH2 dispensing standards mature (SAE J2601, ISO 19880)
- ⚠️ LH2 standards mature BUT implementation barriers exist
- ⚠️ On-site electrolysis standards still developing
- ⚠️ Safety engineering methodology standardizing

---

## 11. LIMITATIONS & CONTEXT

### Temporal Factors

- Paper published 2023; standards landscape evolving rapidly
- EU Hydrogen Strategy driving new standard development
- Italy regulatory framework outdated (last major update 2018)

### Geographic Specificity

- Focus on Europe/Italy; US/Asia/Japan standards mentioned but not deeply analyzed
- Italian framework may not reflect other EU countries' progress
- Regulatory comparison incomplete (Germany, France not detailed)

### Standard Maturity Variation

- GH2 standards more complete than emerging technologies (PEM electrolyzers)
- Standards documentation may require proprietary access (ISO standards expensive)
- Implementation practices may diverge from formal standards

---

## 12. READY FOR YOUR WORK

This paper is **excellent for:**

1. **Regulatory Barrier Analysis Chapter:**
   - Document regulatory landscape as implementation obstacle
   - Show multi-level coordination requirements
   - Identify critical gaps (Italy, LH2 permitting)

2. **Policy & Institutional Framework:**
   - Standard development process overview
   - Global harmonization efforts
   - National adoption bottlenecks

3. **Technical Standards Reference:**
   - Complete list of applicable standards by component
   - SAE J2601 protocol for dispensing (cite for safety equivalence)
   - ISO 19880 framework for design/operation

4. **Implementation Guidance:**
   - Safety engineering principles
   - Hazard identification methodology
   - Permitting pathway insights

---

## 13. INTEGRATION WITH OTHER PAPERS

**Genovese2023 (Standards) + Genovese2024 (Operations):**
- Standards define requirements; Genovese2024 shows real-world compliance
- Together: "Here's what regulations require; here's how they perform in practice"

**Genovese2023 + Wu2024 + Isaac2023:**
- Regulatory framework + Economic viability + Spatial optimization
- Complete deployment strategy: Where to place (Isaac) + How to operate (Wu) + How to permit (Genovese2023)

**Genovese2023 + Raeesi2024:**
- Regulatory requirements apply to supply chain design
- Must comply with standards across production → storage → dispensing (Raeesi2024) AND permitting (Genovese2023)

---

## 14. KEY TAKEAWAYS FOR THESIS

1. **Regulatory maturity varies significantly:** GH2 standards complete; LH2 permitting problematic; on-site production still evolving

2. **Multi-level coordination required:** Global standards alone insufficient; national/local permitting critical

3. **Safety engineering is systematic:** Standards provide methodology, not just equipment specs

4. **Italy as case study:** Shows how regulatory gaps can impede deployment despite technology readiness

5. **Harmonization opportunity:** Global standards exist; implementation bottleneck is political/regulatory, not technical

6. **Public safety & standards evolution:** Recent accidents (2019) driving standard updates; continuous learning cycle

---

## 15. PRACTICAL APPLICATION

### For Exposé Section on Regulatory Framework

**Structure:**
1. Introduce: HRS standards gap identified by authors (state of knowledge in 2023)
2. Present: Global framework (ISO/IEC/SAE coordinated approach)
3. Analyze: European progress (CEN/CENELEC) vs. national implementation gaps
4. Case study: Italy regulatory obstacles (lessons for implementation)
5. Conclude: Standards exist; permitting/coordination are barriers, not technology

### Key Numbers for Thesis

- **3 ISO/TC committees** developing HRS standards
- **8 CEN/CENELEC technical committees** with HRS-relevant standards
- **700 bar dispensing** standard (SAE J2601)
- **42 m safety distance** at 700 bar (vs. 2 m at 1 bar)
- **Flammable range:** 4-75% hydrogen in air (wide → hazardous)
- **Recent accidents:** 2019 Santa Clara (3-month disruption), Oslo incidents

---

**Paper #5 Analysis: ✓ COMPLETE**

**Total papers analyzed:** 5/9 (56% complete)

**Next:** Paper #6 (Kim2020) — Strategic deployment in Korea (detailed summary)
