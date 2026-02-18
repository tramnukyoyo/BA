# Wu et al. 2024 - Paper Summary

## 1. PAPER BASICS

**Title:** Economic analysis of hydrogen refueling station considering different operation modes

**Authors:** Ling Wu, Zhentao Zhu, Yi Feng, Wenyi Tan

**Institutions:** School of Economics and Management, Nanjing Institute of Technology, Nanjing, China; International Joint Laboratory of Green & Low Carbon Development, Jiangsu Province, China

**Journal:** International Journal of Hydrogen Energy, Volume 52 (2024), pages 1577-1591

**DOI:** 10.1016/j.ijhydene.2023.09.164

**Publication Date:** October 3, 2023 (available online); Accepted September 15, 2023

**Type:** Empirical economic analysis with life-cycle cost modeling

**Focus:** Comprehensive cost-benefit analysis of HRS operation under four different supply configurations

---

## 2. KEY CONTRIBUTIONS

This paper provides a **comprehensive economic analysis framework** for HRS viability by:

1. **Two life-cycle analysis models:**
   - Annualized cost model for hydrogen transportation (novel approach)
   - Levelized cost of hydrogen (LCOH) model for HRS operations

2. **Four operation mode comparison:**
   - On-site hydrogen production (water electrolysis)
   - Off-site with pipeline transportation
   - Off-site with long tube trailer transportation
   - Off-site with liquid hydrogen tanker transportation

3. **Distance-dependent cost analysis:**
   - Evaluates 6 distances: 50, 100, 200, 300, 500, 1000 km
   - Analyzes pipeline capacity utilization impact (100%, 70%, 50%, 20%)
   - Provides distance-based optimal mode recommendations

4. **Chinese context application:**
   - Based on China's HRS cost data and policy framework
   - References China's target of 35 CNY/kg hydrogen price
   - Tests against China's 5 million CNY subsidy policy

5. **Cost structure transparency:**
   - Detailed breakdown of capital costs, operating costs, feedstock costs
   - Separates fixed vs. variable cost components
   - Shows cost sensitivity to key parameters

---

## 3. METHODOLOGY

### Life-Cycle Analysis Approach

**Stage 1: Construction/Setup** (Year 0)
- Equipment procurement
- Installation engineering
- Land and civil construction
- Vehicle and pipeline acquisition

**Stage 2: Operation & Maintenance** (Years 1-20)
- Ongoing maintenance and repairs
- Labor costs
- Rent and management
- Insurance

**Stage 3: Cost Recovery** (End of life)
- Equipment salvage value (assumed 10% of CAPEX)
- Revenue from hydrogen sales
- Government subsidies (China: 5 million CNY per station)

### Model 1: Annualized Cost (AC)

**Formula:**
```
AC = [CAPEX × (r(1+r)^N) / ((1+r)^N - 1)] + OPEX + FEEDX - [L × (r(1+r)^N) / ((1+r)^N - 1)]
```

Where:
- CAPEX = Construction costs
- OPEX = Annual operation costs
- FEEDX = Annual feedstock costs
- N = Station operation period (20 years)
- r = Social discount rate (5%)
- L = Salvage value

**For Vehicle Transportation:**
- ACv = Vehicle purchase annualized cost
- ACf = Fuel + toll costs
- ACvm = Vehicle maintenance
- ACve = Electricity for compression/liquefaction
- ACl = Labor costs

**For Pipeline Transportation:**
- ACp = Pipeline construction annualized cost
- ACpm = Pipeline maintenance
- ACpe = Electricity for compression
- ACl = Labor costs

### Model 2: Levelized Cost of Hydrogen (LCOH)

**Formula:**
```
LCOH = [CAPEX + Σ(OPEX + FEEDX) / (1+r)^t - L / (1+r)^N] / [Σ QH2 / (1+r)^t]
```

Where:
- QH2 = Annual hydrogen supply volume
- t = Year (1 to N)
- All costs discounted to present value

**Interpretation:** Average cost per kg of H2 delivered at pump over entire 20-year lifecycle

---

## 4. HRS CONFIGURATION & PARAMETERS

### Test Case: 500 kg/day Refueling Capacity

**Physical specifications:**
- Hydrogen storage: 2 × 500 kg fixed cylinders (1000 kg total capacity)
- Compressor: 45 MPa working pressure
- Dispenser: 35 MPa, 2 hydrogenation guns
- Area required: 1000 m² (off-site), 2000 m² (on-site)
- Staffing: 6 people (off-site), 8 people (on-site)

**Economic parameters:**
- Operating cycle: 20 years
- Social discount rate: 5%
- Operating days/year: 350 days
- Operating hours/day: 12 hours
- Equipment maintenance fee: 3% of equipment cost
- Labor cost: 100,000 CNY/person/year
- Electricity price: 0.6 CNY/kWh
- Residual value (salvage): 10% of CAPEX
- Government subsidy (China): 5 million CNY per station
- Target H2 price (China): 35 CNY/kg

---

## 5. OPERATION MODES & HYDROGEN TRANSPORTATION

### Mode 1: Long Tube Trailer (Off-Site Production)

**Specification:**
- Working pressure: 20 MPa
- Capacity: 350 kg per fill
- Transportation efficiency: 75%

**Cost components (Table 3 parameters):**
- Vehicle purchase: 100 × 10⁴ CNY
- Fuel consumption: 0.25 L/km
- Fuel price: 7 CNY/L
- Tolls: 0.6 CNY/km
- Drivers/stevedores: 3 people
- Annual salary: 100,000 CNY/person

**Cost results by distance:**
| Distance | Cost (CNY/kg) |
|----------|---------------|
| 50 km | 3.91 |
| 100 km | 5.04 |
| 200 km | 7.29 |
| 300 km | 9.55 |
| 500 km | 14.05 |
| 1000 km | 25.32 |

**Performance characteristics:**
- Lowest cost within 270 km vs. liquid tanker
- Uneconomical beyond 300 km (LCOH >35 CNY/kg)
- Cost drivers: fuel (25%), tolls, labor (37% total)

### Mode 2: Liquid Hydrogen Tanker (Off-Site Production)

**Specification:**
- Capacity: 4000 kg per trip
- Power consumption: 11 kWh/kg (for liquefaction)
- Temperature maintenance: -253°C during transport
- Energy density: 8.5 MJ/L
- Evaporation losses: Account for energy intensity

**Cost components (Table 4 parameters):**
- Tanker purchase: 300 × 10⁴ CNY
- Drivers/stevedores: 3 people
- Electricity for liquefaction: 0.6 CNY/kWh

**Cost results by distance:**
| Distance | Cost (CNY/kg) |
|----------|---------------|
| 50 km | 8.53 |
| 100 km | 8.63 |
| 200 km | 8.84 |
| 300 km | 9.05 |
| 500 km | 9.47 |
| 1000 km | 10.53 |

**Performance characteristics:**
- Insensitive to distance (electricity 60% of cost)
- Economical up to 1000 km (cost stable ~8-10 CNY/kg)
- Best for 300-1000 km range (outperforms tube trailer)
- Lower LCOH than tube trailer despite lower efficiency (due to large capacity: 4000 kg vs 350 kg)

### Mode 3: Pipeline Transportation (Off-Site Production)

**Specification:**
- High-pressure pure hydrogen pipeline
- Construction cost (China): 5.36 million CNY/km average
- Maintenance: 10% of total investment
- Compressor power: 750 kW
- Lifespan: 20 years
- Material: Low-carbon steel (hydrogen embrittlement resistance)

**Cost components (Table 5 parameters):**
- Pipeline cost: 536 × 10⁴ CNY/km
- Capacity: 10 × 10⁴ tons/year
- Operating hours: 5 h/d

**Cost results by distance AND capacity utilization:**

| Distance | 100% Util. | 70% Util. | 50% Util. | 20% Util. |
|----------|-----------|---------|---------|---------|
| 50 km | 1.40 | 1.50 | 1.63 | 2.31 |
| 100 km | 1.63 | 1.82 | 2.08 | 3.45 |
| 200 km | 2.08 | 2.47 | 2.99 | 5.72 |
| 300 km | 2.54 | 3.12 | 3.90 | 7.99 |
| 500 km | 3.45 | 4.42 | 5.72 | 12.54 |
| 1000 km | 5.72 | 7.67 | 10.27 | 23.92 |

**Performance characteristics:**
- **LOWEST cost at 100% utilization** (0.66-5.72 CNY/kg for 50-1000 km)
- Highly sensitive to capacity utilization (2.54 → 7.99 CNY/kg at 300 km)
- At 20% utilization, cost approaches tube trailer (not cost-competitive)
- High upfront CAPEX but lowest marginal cost per kg
- Future-proof: Costs drop dramatically as HRS network grows (→100% utilization)

**Key insight:** Pipeline viability depends on **network scale and coordination**. Works only with sufficient HRS density to achieve high utilization rates.

### Mode 4: On-Site Hydrogen Production (Water Electrolysis)

**Specification:**
- Technology: Alkaline electrolysis (mature, lower cost than PEM)
- Strategy: Off-peak valley electricity (lower rates)
- Rated power: 5 MW electrolyzer
- Efficiency: 70%
- Operating hours: 5 h/day
- Electricity price (valley): 0.3 CNY/kWh

**Cost components (Table 6 parameters):**
- Alkaline electrolyzer cost: 201 × 10⁴ CNY/MW
- Replacement cycle: 10 years
- Replacement cost: 301.5 × 10⁴ CNY
- Water consumption: 0.0178 m³/kg
- Water price: 3.32 CNY/m³

**Cost result:**
```
LCOH (on-site) = 35.24 CNY/kg
```

**Performance characteristics:**
- **NOT ECONOMICAL** - exceeds China's 35 CNY/kg target
- Electricity costs dominate (even at low 0.3 CNY/kWh valley rate)
- Electrolyzer capital + replacement costs are major factor
- Main drivers of cost:
  - Power: ~300.5 CNY/kg (>50%)
  - Electrolyzer replacement: ~301.5 × 10⁴ CNY over 20 years
  - Water costs: negligible

**Critical insight:** On-site production currently uneconomical even with:
- Lowest valley electricity rates
- Mature alkaline technology
- 500 kg/day scale
- Government subsidy considered

**Viability pathway:** Requires either:
1. Much lower electricity prices (renewable-only production)
2. Higher capacity factor (currently only 5 hrs/day)
3. Technological breakthrough (higher efficiency)

---

## 6. COMPREHENSIVE ECONOMIC RESULTS

### Finding 1: Transportation Mode Economics

**Off-site stations (external hydrogen):**
- Hydrogen supply costs: **>50% of total LCOH**
- Hydrogen purchase: 10 CNY/kg (industrial by-product)
- As distance increases, supply cost fraction grows

**Cost ranking (LCOH at 300 km distance):**
1. Pipeline (100% util.): **23.35 CNY/kg** ✓ BEST
2. Liquid tanker: **30.62 CNY/kg**
3. Tube trailer: **31.12 CNY/kg**
4. On-site production: **35.24 CNY/kg** ✗ WORST

### Finding 2: Distance-Based Optimal Mode Selection

**0-270 km:** Long tube trailer < Liquid tanker
**270-1000 km:** Liquid tanker < Long tube trailer
**0-1000 km (if high util.):** Pipeline < All others

**Specific thresholds:**
- **Tube trailer economical:** Within 300 km only
- **Liquid tanker economical:** Throughout 0-1000 km range
- **Pipeline economical:** Requires 100% capacity utilization
- **On-site:** Uneconomical at all scales tested

### Finding 3: Total HRS LCOH by Mode

**Off-site station with various transportation:**

| Mode | LCOH Range | Notes |
|------|-----------|-------|
| Pipeline (100%) | 22.21-26.53 CNY/kg | Best for 0-1000 km |
| Liquid tanker | 30.10-32.10 CNY/kg | Stable, long-range capable |
| Tube trailer | 25.48-46.89 CNY/kg | Economical only <300 km |
| On-site electrolysis | 35.24 CNY/kg | Uneconomical |

**All off-site modes meet China's 35 CNY/kg target** within economically viable distances

**On-site production cannot meet target** under current conditions

### Finding 4: Cost Structure Analysis

**Off-site station with tube trailer (100 km distance):**
- Hydrogen purchase: 56.8%
- Transportation: 18.9%
- Equipment CAPEX: 12.6%
- Operating: 8.5%
- Other: 3.2%

**Off-site station with liquid tanker (100 km):**
- Hydrogen purchase: 49.2%
- Electricity for liquefaction: 38.1%
- Equipment CAPEX: 8.0%
- Transportation/other: 4.7%

**Off-site station with pipeline (100 km, 100% util.):**
- Hydrogen purchase: 58.5%
- Pipeline infrastructure (annualized): 28.4%
- Equipment CAPEX: 7.9%
- Operating: 5.2%

**On-site production station:**
- Electricity costs: ~55% (even at 0.3 CNY/kWh valley rate)
- Electrolyzer capital: ~35%
- Water/other: ~10%

### Finding 5: Pipeline Utilization Sensitivity

**Pipeline transportation cost vs. utilization rate (300 km distance):**

| Utilization | Cost (CNY/kg) | Relative Cost |
|---------|---------|----------|
| 100% | 2.54 | 100% (baseline) |
| 70% | 3.12 | 123% |
| 50% | 3.90 | 153% |
| 20% | 7.99 | 315% |

**Implication:** At low network density (20% utilization), pipeline becomes uncompetitive with truck transport. **Critical mass needed for pipeline viability.**

---

## 7. PRACTICAL IMPLICATIONS FOR YOUR THESIS

### Directly Useful For:

1. **Economic Viability Chapter**
   - Quantified LCOH for each operation mode
   - Distance-dependent cost analysis
   - Sensitivity analysis framework

2. **Supply Chain Economics**
   - Hydrogen sourcing cost breakdown
   - Transportation mode trade-offs
   - Infrastructure investment amortization

3. **Policy & Investment Analysis**
   - Government subsidy adequacy assessment
   - Break-even analysis for each mode
   - Risk factors (utilization rate, electricity price)

4. **Regional Implementation Strategy**
   - Which mode optimal for each distance range
   - Infrastructure coordination needed for pipelines
   - Cost-competitive deployment timeline

5. **Techno-Economic Comparison**
   - On-site vs. centralized production economics
   - Technology maturity vs. cost curves
   - Improvement potential for each technology

---

## 8. COST SENSITIVITY ANALYSIS

### Variables Analyzed:

1. **Hydrogen source distance:** Primary variable (50-1000 km)
2. **Pipeline capacity utilization:** 20%, 50%, 70%, 100%
3. **Transportation efficiency:** 75% (tube), 85% (tanker)
4. **Electricity prices:** 0.3 CNY/kWh (valley), 0.6 CNY/kWh (regular)
5. **Hydrogen purchase price:** 10 CNY/kg (industrial by-product)

### Critical Sensitivity Findings:

**Most sensitive parameters:**
1. Pipeline utilization rate (cost varies 2.5x: 2.54 → 7.99 CNY/kg)
2. Hydrogen transportation distance (varies 2x: 8.53 → 10.53 for liquid tanker)
3. Hydrogen source price (>50% of LCOH for off-site)
4. Electricity price (dominates on-site production costs)

**Less sensitive:**
- Vehicle type/capacity (within range tested)
- Operating hours (within 0-12 hours tested)
- Staff numbers (relatively small % of cost)

---

## 9. KEY QUOTES FOR CITATION

1. **On cost dominance:**
   "Hydrogen supply costs account for over 50% of the LCOH for off-site station"

2. **On on-site production viability:**
   "On-site hydrogen production by water electrolysis is not economical at a cost of 35.24 CNY/kg" (above China's 35 CNY/kg target)

3. **On optimal operation mode:**
   "Among the four operation modes, off-site station with pipeline transportation is the most economical mode"

4. **On distance-based optimization:**
   "When the transportation distance is within 270 km, the cost of long tube trailer transportation is lower than that of liquid hydrogen tanker, and the cost of liquid hydrogen tanker is lower if it exceeds 270 km"

5. **On pipeline utilization importance:**
   "The cost advantage increases as pipeline capacity utilization rate reaches 100%, but decreases as it drops to 20%"

6. **On future infrastructure potential:**
   "In the range of 0~1000 km, the cost of pipeline transportation is the lowest. Although currently HRSs are not yet popular and the stations are scattered...with the development of the hydrogen industry, the hydrogen pipeline will eventually become the best choice"

7. **On economic viability:**
   "The profitability of HRSs is an important indicator of whether investors invest in the construction of HRSs" (implication: current on-site production makes investment risky)

---

## 10. DATA FOR YOUR THESIS

### CAPEX for 500 kg/day HRS (China context)

**Off-site station:**
- Equipment total: ~1,319 × 10⁴ CNY
- Construction/land: ~250 × 10⁴ CNY
- Total CAPEX: ~2,200-2,500 × 10⁴ CNY (excluding transportation/pipeline)
- Gov. subsidy: 5 × 10⁴ CNY
- Net investment: ~1,700-2,000 × 10⁴ CNY

**On-site station:**
- Electrolyzer: 201 × 10⁴ CNY
- Other equipment: ~1,319 × 10⁴ CNY
- Construction/land: ~350 × 10⁴ CNY
- Total CAPEX: ~3,000+ × 10⁴ CNY (larger land requirement)
- Gov. subsidy: 5 × 10⁴ CNY
- Net investment: ~2,500+ × 10⁴ CNY

### LCOH Results Summary

**Off-site (best case - pipeline, 100 km, 100% util.):**
- 22.44 CNY/kg (€2.82/kg at exchange rate 1:8)

**Off-site (typical - liquid tanker, 500 km):**
- 31.05 CNY/kg (€3.88/kg)

**Off-site (worst economical - tube trailer, 300 km):**
- 31.12 CNY/kg (€3.89/kg)

**On-site (electrolyzer):**
- 35.24 CNY/kg (€4.41/kg) - UNECONOMICAL

### Operating Parameters

- **Station capacity:** 500 kg/day = 175,000 kg/year
- **Operating cycle:** 20 years
- **Break-even hydrogen price (China target):** 35 CNY/kg
- **Operating margin needed:** 2-4 CNY/kg (assuming revenue ≥ LCOH)

---

## 11. CONNECTION TO YOUR THESIS FRAMEWORK

### Dimension 2: Analysis Framework (Economic Assessment)

**This paper directly addresses:** Economic Viability assessment

**Specific contributions:**
- Provides comprehensive cost-benefit methodology (annualized + LCOH models)
- Compares multiple operation modes economically
- Shows distance-dependent cost curves
- Demonstrates cost sensitivity to key parameters (utilization, distance, energy)

### Dimension 1: Challenges (Economic Feasibility & Logistics)

**Logistical barriers quantified:**
- On-site production currently not economically viable
- Long-distance transportation (>300 km) requires liquid/pipeline options
- Network coordination critical for pipeline economics (utilization sensitivity)

**Economic barriers identified:**
- Hydrogen sourcing cost dominates (>50% of LCOH)
- Electricity costs prevent on-site competitiveness
- High capital costs require scale or subsidies

### Dimension 3: Integration Scenarios (Economic Viability by Type)

**Corridor scenario (long-haul):**
- Liquid tanker optimal: Constant cost over distance (~9-10 CNY/kg)
- Pipeline optimal if >20% utilization

**Industrial Hub scenario (concentrated demand):**
- Pipeline optimal: Can achieve 100% utilization with demand clustering
- Lowest costs: 22-25 CNY/kg

**Urban cluster scenario (distributed demand):**
- Liquid tanker optimal: Handles multiple small stations economically
- Tube trailer for short distances (<270 km)

---

## 12. LIMITATIONS & CONTEXT

### Geographic Context

- **China-specific:** Uses Chinese equipment costs, electricity rates, labor costs
- **CNY pricing:** Must convert for European context (typical 8:1 EUR exchange rate in 2023)
- **Labor costs:** Chinese 100,000 CNY/year ≈ €12,500; European costs ~€35,000-50,000+

### Technology & Cost Assumptions

- **Electrolyzer:** 70% efficiency (alkaline) - PEM electrolysis would be higher cost
- **Valley electricity:** Assumes 0.3 CNY/kWh available - not all regions have this
- **Industrial H2 price:** 10 CNY/kg assumes sufficient feedstock availability
- **No CO2 costs included:** Blue hydrogen CCUS not explicitly modeled

### Market & Policy Context

- **Subsidy:** 5 million CNY per station assumed - actual policy may vary
- **Scale:** 500 kg/day is small scale; larger stations (1000+ kg/day) may show different economics
- **Time frame:** 20-year operation period; may be shorter/longer in practice

### Model Limitations

- **Perfect foresight:** Assumes all parameters known at start
- **Static demand:** Doesn't model demand growth over time
- **No uncertainty:** Doesn't include risk factors (fuel availability, demand volatility)
- **Salvage value:** Assumed 10% of CAPEX; actual recovery may vary

---

## 13. READY FOR YOUR WORK

This paper is **excellent for:**

1. **Economic viability assessment chapter:**
   - Methodological models for life-cycle costing
   - Data on real HRS costs and operating parameters
   - Sensitivity analysis framework

2. **Comparison of operation modes:**
   - Quantified cost advantage/disadvantage of each
   - Distance-based decision framework
   - Utilization rate impact on pipeline economics

3. **Policy recommendations:**
   - Subsidy adequacy assessment
   - Technology choice guidance (on-site vs. external)
   - Infrastructure coordination requirements

4. **Supply chain cost breakdown:**
   - Transparency on where costs lie (hydrogen 50%, electricity 25-40%, etc.)
   - Capital vs. operating cost trade-offs
   - Scaling cost behavior

---

## 14. INTEGRATION NOTES

### With Other Papers:

**Wu2024 + Raeesi2024:**
- Raeesi: Supply chain logistics (UK HGV case, 539 HRS network)
- Wu: Economics of different supply modes
- Together: Complete picture of supply chain economics

**Wu2024 + Isaac2023:**
- Isaac: Optimal HRS locations (spatial optimization)
- Wu: Cost of delivering H2 to those locations
- Together: Location optimization considering cost

---

## 15. NEXT STEPS FOR YOUR THESIS

### Chapter Integration:

1. **Chapter 2 (Herausforderungen - Economic Barriers):**
   - Cite on-site production uneconomical finding
   - Note hydrogen sourcing cost dominance

2. **Chapter 4 (Wirtschaftliche Bewertung - Economic Assessment):**
   - Use LCOH models as analytical framework
   - Apply distance-based mode selection logic
   - Reference specific cost figures

3. **Chapter 5 (Integrationsszenarien - Scenario Analysis):**
   - Use mode selection to differentiate scenarios
   - Apply cost sensitivity analysis to different deployment strategies

---

**Paper #3 Analysis: ✓ COMPLETE**

**Key value for thesis:** Provides quantified economics for HRS viability analysis; critical for demonstrating feasibility of deployment strategies.

---

