# Kim et al. 2020 - Paper Summary: Strategic HRS Deployment for Korea

## CORE CONTRIBUTION

**Title:** Development of strategic hydrogen refueling station deployment plan for Korea

**Key Innovation:** First comprehensive nationwide HRS deployment optimization considering general roads + expressways + buses separately using lexicographic optimization

**Method:** Deployment Optimization Algorithm (DOA) with 3 sequential models:
1. **Station Number Determination** → required HRSs to hit target coverage %
2. **Max Cover Model** → maximize covered demand (priority)
3. **P-Median Model** → minimize travel time (secondary)

**Results:** Nationwide deployment strategy for Korea 2022→2030→2040 with HFCV targets

---

## KEY CHALLENGE: THE CHICKEN-AND-EGG PROBLEM

**Problem Definition:**
- HRS construction cost: $1.5-3.0M per station (10× gas station cost)
- Government budget limited → can't install all stations immediately
- Consumers won't buy HFCVs without sufficient HRS network
- Result: Circular dependency blocking deployment

**Solution Strategy:**
- Prioritize high-demand corridors (highways, urban centers, bus routes)
- Phase deployment over 18 years with interim target coverage ratios
- Sequential location optimization balancing coverage vs. travel time

---

## DEPLOYMENT OPTIMIZATION ALGORITHM (DOA)

### Step 1: Demand Estimation
- Estimate future HFCV distribution (2022/2030/2040)
- Identify demand sources: Admin offices (general roads), toll gates (expressways), bus garages (buses)
- Calculate demand per location using population & traffic data

### Step 2: Station Number Determination Model
**Objective:** Minimize number of stations needed to cover γ% of demand

**Key Parameters:**
- **R** = max travel time to covered station (typically 15-30 min)
- **S** = max travel time from uncovered demand to nearest station (fallback)
- **γ** = target coverage ratio (e.g., 80%, 90%)
- **C** = station capacity (finite, not infinite)

**Constraints:**
- At least γ×Ei vehicles from source i covered
- Uncovered vehicles within distance S of nearest station (safety net)
- Station capacity respected (xij ≤ C×zj)
- Previously installed stations must remain open (continuity)

### Step 3: Max Cover Model
**Given:** Number of stations determined in Step 2
**Objective:** Maximize number of HFCV within reachable distance

**Priority:** Coverage maximization is more important than travel time minimization

### Step 4: P-Median Model
**Objective:** Among all solutions maximizing coverage, minimize total travel time

**Use:** Secondary optimization to select most convenient station locations for drivers

---

## KOREA-SPECIFIC APPLICATION

### Government Targets

| Year | Passenger FCEVs | Buses | Stations Targeted |
|---|---|---|---|
| 2022 | 30,000 | 7,200 | ~100 |
| 2030 | 620,000 | 70,000 | ~1,000 |
| 2040 | 2,000,000 | 200,000 | ~2,000+ |

### Network Structure

**General Roads:** Admin office locations (demand sources) → Gas station rest areas (candidate sites)
- Coverage target: 15-20 min drive radius
- Serves: Passenger cars, taxis, urban delivery

**Expressways:** Highway toll gates → Service plazas & rest areas
- Coverage target: Long-haul freight/passenger routes
- Bus capacity: 210 km range with 21 kg hydrogen; farthest Korea cities = 551 km → no inter-city bus expressway refueling needed

**Buses:** Bus garages (demand + candidate sites same)
- Only 1 station per bus garage required (single trip refueling)
- No expressway bus stations needed (intra-city + limited range)

---

## MODEL SOPHISTICATION VS PRIOR WORK

### Previous Limitations (Prior Studies)
- ❌ Focused on either general roads OR expressways (not both)
- ❌ Assumed infinite station capacity (unrealistic)
- ❌ Ignored bus operations entirely
- ❌ Used simplified demand models (e.g., population only)

### Kim2020 Advances
- ✅ Integrated general roads + expressways + buses in one framework
- ✅ Finite capacity constraints (realistic)
- ✅ Three-stage optimization (number → coverage → travel time)
- ✅ Distinguishes covered vs. uncovered HFCVs with fallback distance S
- ✅ Continuous station operation requirement (real constraint)
- ✅ Representative demand sources + candidate sites

---

## MATHEMATICAL MODEL CORE (Simplified)

**Notation:**
- I = demand sources (admin offices, toll gates, garages)
- J = candidate sites (rest areas, service plazas, garages)
- Ei = HFCVs at source i
- tij = travel time source i to site j
- C = station capacity (kg/unit)

**Station Number Determination Model:**
```
Minimize: Σ zj (total stations)

Subject to:
- Σ xij ≥ γ * Ei  (cover target %)
- xij ≤ Ei * aij  (can only assign if reachable)
- Σ xij ≤ C * zj  (capacity constraint)
- Must have ≥1 station within S minutes of all demand (safety)
```

**Then apply Max Cover → P-Median sequentially**

---

## KEY RESULTS FOR YOUR THESIS

### Nationwide Deployment Strategy

**2022 Deployment:** ~100 stations prioritizing:
- Seoul metropolitan (highest density)
- Busan-Daegu-Incheon corridors
- Express highways (Seoul-Busan, Seoul-Jeonju)

**2030 Expansion:** ~1,000 stations achieving:
- 80-90% coverage of urban/expressway demand
- Regional hub clusters

**2040 Target:** ~2,000+ stations achieving:
- Near-universal coverage
- Mature hydrogen economy

### Coverage Progression

- 2022: ~30% national coverage (major corridors)
- 2030: ~70-80% coverage (cities + highways)
- 2040: ~95%+ coverage (ubiquitous)

### Phased Installation Advantage

- Spreads capital investment over 18 years
- Allows demand growth to justify subsequent phases
- Earlier phases establish core network (corridor effect)
- Bus routes (7,200 → 70,000 → 200,000) drive utilization

---

## CONNECTION TO YOUR THESIS FRAMEWORK

### Dimension: Spatial Planning & Network Design

**This paper directly addresses:**
- Optimal location methodology (general applicability)
- Phased deployment strategy (scales with vehicle adoption)
- Differentiated network segments (urban/highway/bus)

**For Your Thesis:**
- Use as case study for practical deployment optimization
- Cite methodology for spatial planning section
- Reference Korea's targets for regional comparison (EU vs. Korea vs. Australia)

### Cross-Paper Integration

**Kim2020 (Spatial) + Wu2024 (Economics) + Isaac2023 (Optimization):**
- Isaac: Which optimization method? (Flow-based, P-median, Max-cover)
- Kim: How to apply it nationwide (phased, multi-segment)
- Wu: What does each location cost? (supply mode impact)

---

## PRACTICAL IMPLEMENTATION INSIGHTS

### Demand Source Definition (Critical)

**General Roads:** Admin offices (every district)
- Rationale: People work/live near admin centers; representative demand
- Advantage: Systematic, government data available
- Limitation: Doesn't capture true car distribution

**Expressways:** Existing toll gates
- Rationale: Already established stopping points
- Advantage: Infrastructure exists; drivers familiar with locations
- Limitation: May not optimize for highway traffic patterns

**Buses:** Bus garages
- Rationale: Central refueling point; operational efficiency
- Advantage: Demand and supply location identical
- Limitation: Simplifies real bus route variations

### Continuous Operation Requirement

**Key insight:** If HRS installed in 2022, must remain operational in 2030 & 2040
- Prevents repeated shut-downs/relocations (inefficient)
- Creates sunk cost justification for later expansion
- Strategic phasing requires long-term commitment

---

## LIMITATIONS & REALISM TRADE-OFFS

**Simplified Aspects:**
- Ignores detailed site costs, land availability
- Doesn't model driver behavior near expressway exits
- Assumes uniform station capacity (real stations vary)
- Doesn't account for refueling time queues
- Population-based demand proxy (crude)

**Realistic Advances:**
- ✅ Finite capacity (not infinite)
- ✅ Three-segment network differentiation
- ✅ Phased installation over realistic timeline
- ✅ Coverage vs. travel time trade-off
- ✅ Safety net distance (S parameter) for uncovered HFCVs

---

## NUMERICAL INSIGHT: KOREA'S SCALE

**Country Context:**
- Population: ~52 million
- Area: ~100,000 km²
- Highway network: Major expressways + local roads
- Vehicle ownership: ~20M registered vehicles

**By 2040:**
- HFCV penetration: ~10% of fleet (2M vehicles)
- Station density: 1 HRS per 25,000-50,000 people
- Comparable to current US gas station density (~150,000 gas stations for 330M people)
- Bus hydrogen adoption: Earlier & faster (fleet ops vs. individual consumers)

---

## KEY TAKEAWAYS FOR EXPOSÉ

1. **Chicken-and-Egg Problem is Real:** $1.5-3.0M per station cost makes simultaneous deployment impossible

2. **Phased Deployment is Necessary:** 18-year rollout justified by matching infrastructure to vehicle adoption

3. **Network Segmentation Matters:** General roads, expressways, buses have different optimization requirements

4. **Optimization Models are Practical Tools:** Can operationalize deployment strategy (not just theoretical)

5. **Coverage-Travel Time Trade-off:** Can't maximize both; prioritize coverage, then optimize convenience

6. **Korea as Reference Case:** Ambitious targets (2M HFCVs by 2040) show large-scale deployment feasibility

---

**Paper #6 Analysis: ✓ COMPLETE**

**Total papers analyzed:** 6/9 (67% complete)

**Next:** Papers 7-9 (accelerated summaries for Samsun2022, Kim2023, Atabay2024)
