# Raeesi et al. 2024 - Paper Summary

## 1. PAPER BASICS

**Title:** Hydrogen supply chain and refuelling network design: assessment of alternative scenarios for the long-haul road freight in the UK

**Authors:** Ramin Raeesi, Christa Searle, Nazmiye Balta-Ozkan, Laura Marsiliani, Mi Tian, Philip Greening

**Journal:** International Journal of Hydrogen Energy, Volume 52 (2024), pages 667-687

**DOI:** 10.1016/j.ijhydene.2023.03.474

**Focus:** UK hydrogen supply chain design for heavy goods vehicles (HGVs) in long-haul road freight

---

## 2. KEY CONTRIBUTIONS

This paper addresses **Supply Chain Integration** for hydrogen refueling stations by:

1. **Grid-free modeling approach** - Unlike previous grid-based models, this proposes spatially-explicit locations for HRSs with flexible hydrogen flow
2. **End-to-end supply chain design** - Considers production → storage → transport → distribution as integrated system
3. **Underground storage options** - First to systematically evaluate salt caverns, underground pipes, and lined rock caverns
4. **Policy scenarios** - Tests different H2-HGV penetration levels (1-100%) and safety stock decisions
5. **Decision support tools** - Generates penetration curves and cost sensitivities for policymakers

---

## 3. METHODOLOGY

### Problem Statement

They developed an **optimization-based methodology** to design a hydrogen supply chain that:
- Minimizes total cost per kg of H2 delivered at pump
- Satisfies all HRS daily demands
- Considers production, storage, transportation, and distribution constraints

### The Supply Chain Model

**4 Key Components:**

1. **Hydrogen Production**
   - Blue hydrogen: SMR with CCUS, ATR with CCUS, ATR-GHR with CCUS (300 MW and 1000 MW scales)
   - Green hydrogen: Alkaline electrolysis, PEM electrolysis, Solid oxide electrolysis (10 MW scale)

2. **Hydrogen Storage**
   - Overground: Compressed gas tanks (700 MPa)
   - Underground: Underground pipes (UGP), Lined Rock Caverns (LRC), Salt Caverns (SC)

3. **Transportation**
   - Tier I: Production → Storage (via tube trailers)
   - Tier II: Storage → HRSs (via tube trailers)
   - Tube trailer capacity: 300-2000 kg CH2

4. **Distribution Through HRSs**
   - 539 candidate HRS locations identified in GB
   - Located at: warehouses (75%), service stations (12.5%), ports (12.5%)

### Planning Horizons

Three time periods analyzed: 2025, 2035, 2050

---

## 4. DEMAND ANALYSIS

### UK HGV Hydrogen Demand

**Starting point:** 2019 UK diesel demand for HGVs = 6,179,000 tonnes

**Converted to hydrogen energy equivalent:**
- 5,252,150,000 liters of diesel
- 49,020,066,667 kWh annual energy demand (at full conversion)

**HRS Location Allocation:**
- 382 warehouse facilities (>9,000 m²)
- 111 HGV service stations
- 46 ports
- **Total: 539 candidate HRS locations**

**Demand distribution formula:**
Energy demand per facility = (Warehouse area / Total warehouse area) × Total hydrogen demand

---

## 5. KEY FINDINGS & RESULTS

### Finding 1: Cost Optimization Results

| Year | Cost per kg H2 (Blue) | Cost per kg H2 (Green) | Key Technology |
|------|---|---|---|
| 2025 | €3.64 - €5.28 | €8.61 - €18.00 | SMR with CCUS |
| 2035 | €4.37 | €7.08 | ATR-GHR with CCUS |
| 2050 | €3.64 | €6.14 | ATR-GHR with CCUS |

**By 2050 at 20% penetration:** €3.64/kg hydrogen at pump

### Finding 2: Storage Cost Savings

**Underground storage advantage:**
- Bulk geological storage (salt caverns, LRC, UGP) saves **up to 65%** compared to overground only
- Storage dominates capital costs: **43% of total CAPEX**
- But is only **8% of daily operating costs**

### Finding 3: H2-HGV Penetration Optimization

**Key insight:** Cost is NOT always lower with higher penetration

- **Optimal penetration level:** 13% (lowest cost achieved)
- **Sweet spot:** 10-80% penetration range (€3.5-€4.0/kg)
- **Problem:** At penetration <5%, costs spike sharply
- **Why?:** Tradeoff between increased demand (needs more facilities) vs. equipment utilization

**Policy implication:** Don't blindly push for 100% penetration—there's an optimal economic point around 13%

### Finding 4: Safety Stock Period Impact

**Safety stock is critical for supply chain resilience:**

- **1 day stock:** Very vulnerable to disruptions, but lowest cost
- **5 days stock:** Turning point where slope increases sharply (good maturity balance point)
- **9 days stock:** Higher cost (~€3.5/kg) but better for early-stage HSC reliability
- **30 days stock:** Significantly higher costs

**Policy implication:** Early HSC needs 9-day safety stock; mature HSC can operate with 5-day stock

### Finding 5: Tube Trailer Capacity

Cost improvement with larger capacity (diminishing returns):
- 300-900 kg: Sharp cost decrease
- 900-1800 kg: Moderate improvement
- >1800 kg: No additional benefit

**Recommendation:** 900-1800 kg is the practical sweet spot

### Finding 6: Production Technology Preference

**When both blue & green allowed:**
- Blue hydrogen ALWAYS chosen (0% green hydrogen)
- Why? Green hydrogen electricity costs are too high (operational cost = 56% of total daily cost)

**When green hydrogen only:**
- Costs increase 1.7x compared to blue
- SOE (Solid Oxide Electrolysis) at 10 MW is most efficient

**When blue only:**
- ATR-GHR with CCUS at 300 MW is most cost-effective

---

## 6. COST BREAKDOWN (Baseline Scenario 2050)

### Capital Costs (€ millions)
| Component | Amount | % of Total |
|-----------|--------|-----------|
| Production | ~€1,136M | 13% |
| Storage | ~€149M | (included below) |
| Total CAPEX | ~€2,485M | 100% |

### Daily Operating Costs
| Component | % of Daily Cost |
|-----------|-----------------|
| Production | 56% |
| Storage | 8% |
| Transport | 23% |
| Distribution/HRS | 13% |

---

## 7. PRACTICAL INSIGHTS FOR YOUR THESIS

### Directly Useful For:

1. **Supply Chain Integration Chapter**
   - Real-world UK case study
   - Quantified cost breakdowns
   - Spatially-explicit optimization approach

2. **Economic Viability Analysis**
   - Cost curves by penetration level
   - Cost sensitivity to safety stock
   - Cost sensitivity to transport capacity
   - Comparison of blue vs. green hydrogen economics

3. **Logistical Barriers & Solutions**
   - Addresses "chicken-and-egg" problem quantitatively
   - Shows optimal HGV penetration levels
   - Documents underground storage potential

4. **Regional Implementation Strategies**
   - UK case study can support EU context
   - Shows importance of location optimization
   - Demonstrates impact of policy decisions (penetration, safety stock)

5. **Framework Application**
   - Demonstrates integration scenario concept (corridor-based deployment)
   - Shows how economic viability depends on multiple factors
   - Provides decision-support methodology

---

## 8. LIMITATIONS TO NOTE

- **UK-specific:** Uses UK diesel demand data; needs adjustment for other regions
- **No LCA analysis:** Doesn't include lifecycle emissions (only implicit through carbon cost)
- **Grid-free approach new:** Limited peer comparison; no validation against existing grid models
- **Assumes consistent demand:** Real demand would fluctuate with HGV adoption
- **Green hydrogen costs:** Uses 2021 data; may be outdated with recent cost reductions

---

## 9. KEY QUOTES FOR CITATION

1. **On supply chain design importance:**
   "Designing an economically viable and competitive Hydrogen Supply Chain (HSC) to meet the end-user demand is a significant challenge and relies primarily on the optimal configuration and sizing of required facilities and infrastructure."

2. **On production cost fraction:**
   "Hydrogen production cost can be contributing to as low as 10% of the total cost of the hydrogen delivered at pump, as other value adding activities (particularly, storage and transport) can add significantly to the ultimate cost."

3. **On optimal penetration:**
   "There is an optimal penetration level (which is interestingly low enough to address the ever-ongoing chicken and egg situation), and increasing this would not essentially lead to improved cost of hydrogen at pump."

4. **On storage savings:**
   "Inclusion of bulk geographical storage options in the design of the HSC can save up to around 65% in the cost of each kg hydrogen distributed at pump."

---

## 10. DATA FOR YOUR THESIS

### UK HGV Hydrogen Demand (2019 baseline)
- Annual diesel: 6,179,000 tonnes
- Annual energy: 49,020,066,667 kWh
- Converted HRS locations: 539 candidate sites

### Cost Estimates (2050, Blue Hydrogen)
- Minimum cost: €3.64/kg (at 20% penetration)
- Storage cost dominance: 43% of CAPEX, 8% of OPEX
- Production cost: Only 13% of CAPEX, but 56% of OPEX

### Optimal Operating Parameters
- H2-HGV penetration: 13% (optimal), 10-80% (practical range)
- Safety stock: 5 days (mature HSC), 9 days (early stage)
- Tube trailer capacity: 900-1800 kg (optimal range)

---

## 11. CONNECTION TO YOUR THESIS FRAMEWORK

**Dimension 1 - Challenges (Regulatory, Logistical, Technical):**
- Addresses **logistical barriers**: transport modes, cost structures, network optimization
- Touches on **technical barriers**: storage technologies, compression options
- Relevant to **economic feasibility**: quantifies costs and break-even points

**Dimension 2 - Analysis Framework (Spatial, Economic, Global):**
- **Spatial Planning:** Spatially-explicit HRS optimization
- **Economic Assessment:** Detailed cost-benefit analysis with sensitivity curves
- **Global Context:** UK case generalizable to other regions

**Dimension 3 - Integration Scenarios (Corridor, Urban, Industrial):**
- Demonstrates **corridor-based** approach (long-haul HGV routes)
- Shows **industrial hub** potential (ports, warehouses)
- Economic comparison helps choose scenario

---

## 12. READY FOR YOUR WORK

This paper is **excellent for:**
- Section on supply chain economics
- Case study example of optimization methodology
- Cost data and breakdowns
- Scenario analysis framework
- Policy-relevant findings (penetration curves, safety stock decisions)

