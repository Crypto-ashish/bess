# Module 12 — Parameter Handbook, Quality Engineering and Process FMEA

*Li-ion Cell Manufacturing: an Engineer's Course · Phase C · Evidence labels: [V] verified · [T] typical practice · [E] estimate · [P] proprietary*

**Bottom line:** your automotive quality toolkit transfers almost unchanged. What changes is (1) the **delay** between cause and effect — a defect made at slitting may only show at aging two weeks later — and (2) the **severity scale** — an escaped micro-short is a fire risk. That pushes cell plants towards 100% inline measurement, full genealogy and statistical screening at EOL.

---

## Part A — Manufacturing parameter handbook

Ranges are **windows for learning and DOE starting points**, not specifications. Labels: **[V]** sourced in the stage module, **[T]** typical practice, **[P]** set by your process spec. "Chem" = chemistry-specific; "Equip" = equipment-specific.

| Stage | Parameter | Typical range | Purpose | Effect on quality | Measurement | Control | Common deviation | Corrective action | Label |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 Materials | CAM moisture | Low hundreds of ppm or below; tighter for high-Ni | HF prevention | Gas, fade, gelation | Karl Fischer | Dry storage, exposure time | Bag left open | Re-dry or reject; MES exposure clock | [T] Chem |
| 1 | Magnetic impurities | ppb-level limits | Micro-short prevention | Self-discharge, safety | Magnetic extraction + ICP | Supplier controls, magnets | Supplier process change | 100% lot testing after PCN | [T] |
| 1 | Electrolyte water / HF | ~20 ppm / ~50 ppm order | HF control | Fade, gas | KF / titration | Closed supply | Drum seal leak | Quarantine lot | [T] |
| 2 Slurry | Solids content | NMC ~65–75%, LFP ~45–60%, anode ~40–55% | Coat weight, drying | Cracks, streaks | Moisture balance | Solvent dosing | Evaporation in tank | Adjust; cover tanks | [T] Chem |
| 2 | Viscosity at defined shear | ~1–10 Pa·s class | Coatability | Streaks, settling | Rotational viscometer | Dilution | Gelation, temp | Check pot life, temp | [T]/[P] |
| 2 | Grind (max particle) | Below ~30–50 µm | No agglomerates | Streaks, separator damage | Hegman | Dispersion, filters | Short mixing | Re-mix, filter | [T] |
| 2 | Slurry temperature | ≤ ~40 °C | Stability | Gel, SBR damage | RTD | Jacket | Cooling failure | Alarm, hold batch | [T] |
| 3 Coating | Areal loading | ~15–30 mg/cm² per side (energy cells) | Capacity, N/P | Capacity spread, plating | β/X-ray gauge | Pump closed loop | Pump drift, density change | Re-zero gauge, check slurry solids | [T] Chem |
| 3 | Coat-weight tolerance | ~±1–2% | Uniformity | Capacity spread | Gauge | Closed loop | Cross-web profile | Die adjust, oven balance | [T]/[P] |
| 3 | Line speed | Tens of m/min (20–60 m/min by Dürr model) | Throughput | Bead stability, drying | Encoder | Drive | Speed-up without oven change | Re-validate oven | [V] Equip |
| 4 Drying | Zone temperatures | ~60–150 °C, low–high–low | Drying rate | Binder migration, cracks | Thermocouples | PID | Heater failure | Alarm, stop line | [T] |
| 4 | Residual NMP | Low hundreds ppm or below | Side reactions | Gas | GC | Oven profile | Speed too high | Lower speed | [T] |
| 4 | NMP recovery | >99% | Cost, emissions | — | Mass balance | Recovery unit | Condenser fouling | Clean | [V] Equip |
| 5 Calender | Density NMC / LFP / graphite | ~3.2–3.6 / ~2.2–2.6 / ~1.5–1.7 g/cm³ | Energy vs rate | Rate, wetting, cracking | Disc mass/volume | Gap | Material change | Re-run compaction curve | [T] Chem |
| 5 | Thickness tolerance | ~±2–3 µm per side | Fit, capacity | Can fit, spread | Laser gauge | Closed loop | Roll wear | Regrind | [T] |
| 5 | Roll temperature | Ambient to ~120 °C | Densification | Springback, smearing | RTD | Heater | Uneven heating | Service | [T] |
| 6 Slitting | Burr height | Often ≤ ~10 µm | Separator protection | Shorts | Microscope / vision | Tool life | Knife wear | Change by metres | [T] |
| 6 | Width tolerance | Tenths of mm or tighter | Overhang | Plating | Vision | Knife setup, EPC | Web wander | EPC tune | [T] |
| 6 | Electrode moisture after vacuum drying | Hundreds of ppm or lower | HF | Gas, fade | KF | Recipe | Short dry | Extend recipe | [T]/[P] |
| 7 Assembly | Anode overhang | ~0.5–2 mm per side | Prevent plating | Safety | X-ray/CT | Alignment | Telescoping | EPC, tension | [T]/[P] |
| 7 | Hi-pot insulation | Hundreds of V; MΩ minimum | Short screening | Shorts | Insulation tester | Recipe | Particle | Reject; source analysis | [T] |
| 7 | Weld quality | Design-specific | Low resistance, integrity | IR, opens | Signature + pull | Generator control | Horn wear | PM by count | [P] |
| 7 | Leak rate (lid weld) | Very low (He) | Hermeticity | Moisture ingress | He MS | Laser control | Gap | Fixture | [T] |
| 8 Filling | Fill mass | Design (~1.3–2 g/Ah order) | Wetting + reserve | Fade, plating | Weigh | Pump | Pump wear | Seal change | [T]/[P] |
| 8 | Dew point at filling | Driest zone (−40 to −60 °C class) | HF | Gas | Dew-point sensors | HVAC | People load, leaks | Headcount, sealing | [T] |
| 8 | Wetting time/temperature | RT or 40–60 °C, hours | Full wetting | Plating | MES time | Recipe | Shortcut under pressure | Interlock | [V] ORNL slide |
| 9 Formation | Initial C-rate | ~0.02–0.2C | SEI quality | Plating | Cycler | Recipe | — | — | [T] |
| 9 | Later C-rate | ~0.2–0.5C | Throughput | — | Cycler | Recipe | — | — | [V] |
| 9 | Temperature | ~25–45 °C | Kinetics | Plating / side reactions | Thermocouple | Chamber | Gradient across racks | Mapping | [T] |
| 10 Degas/seal | Pouch seal temperature | ~170–210 °C class | Seal | Leak | Thermocouple | Recipe | Bar wear | Replace | [T] |
| 11 Aging | High-temp aging | ~40–60 °C, hours–days | SEI stabilisation, defect acceleration | — | Logs | AS/RS | — | — | [T] |
| 11 | RT aging duration | ~7–21 days | Self-discharge measurement | Escapes if too short | MES | Recipe | Pressure to ship | Do not shorten without validation | [T] |
| 11 | K-value limit | Fixed or mean + nσ | Micro-short screen | Escapes | OCV meter | Statistics | Temperature drift | Compensate | [T]/[P] |
| 12 Final | Insulation resistance shell-terminal | MΩ class at test voltage | Safety | Leakage | Tester | Recipe | Film damage | Reject | [T] |
| 12 | Shipping SOC (air, UN3480) | ≤30% | Transport rules | — | OCV | Recipe | — | — | [T — check IATA] |

## Part B — Quality engineering approach

### B1. Mapping your automotive toolkit

| Tool | How it is used in a cell plant |
| --- | --- |
| **APQP** | Same phases. Product design (cell design FMEA, DVP&R), process design (PFD, PFMEA, control plan), validation (run-at-rate, Cpk, cell validation tests), feedback. Cell validation takes months (cycle-life, calendar-life, abuse tests) |
| **PPAP** | Customers (pack/vehicle/ESS OEMs) require PPAP-style submissions: PSW, dimensional, material certs, capability, control plan, PFMEA, MSA, lab scope, plus electrochemical test reports |
| **PFMEA** | Severity driven by safety (thermal event) and life; AIAG-VDA Action Priority (AP) increasingly replaces RPN |
| **Control plan** | Per stage; many characteristics measured 100% inline (coat weight, thickness, fill mass, OCV, IR) |
| **SPC** | Continuous inline data → X̄-R/I-MR charts, EWMA for slow drifts; cross-web profiles; run rules |
| **Cp/Cpk** | Targets like ≥1.33 (normal) and ≥1.67 (special characteristics) as in automotive **[T]**; short-term Cp/Cpk in run-at-rate, long-term Pp/Ppk in production |
| **MSA** | Critical: coat-weight gauges, thickness gauges, checkweighers (fill mass), OCV/IR meters (µV/µΩ). GR&R and bias/linearity; temperature effects |
| **Traceability** | Cell-level genealogy back to material lots and machine parameters; roll-to-cell mapping (position on the electrode roll → cell ID) |
| **Defect management** | Inline vision defect maps on electrode rolls; marking and automatic skipping of defective sections at notching/stacking |
| **RCA / 8D** | Same; complicated by delay and need for tear-down analysis (CT, SEM, ICP) |

### B2. Special characteristics for a cell (example)

| Characteristic | Why special | Stage |
| --- | --- | --- |
| Coat weight (both electrodes) / N/P | Safety (plating) | 3 |
| Burr height | Safety (shorts) | 6 |
| Anode overhang | Safety (plating) | 7 |
| Hi-pot insulation | Safety | 7 |
| Moisture (electrodes, electrolyte, dry room) | Safety & life | 1, 6, 8 |
| Fill mass | Life | 8 |
| K-value | Safety | 11 |
| Weld integrity / leak rate | Safety & life | 7, 10 |

### B3. SPC specifics

- **Inline gauges produce huge data**; use subgrouping by roll/lane/position, and watch for **autocorrelation** (successive readings are not independent) — EWMA/CUSUM charts or residual charts are better than plain Shewhart charts for slow drifts **[T]**.
- **Cross-web profile Cpk** (each lane) and **along-web** separately.
- **EOL statistics:** dynamic limits on OCV drop and capacity per lot (outlier detection), plus lot-level trend charts.
- **Linking data:** a defect at EOL is analysed by joining cell ID → roll position → upstream parameter traces (the "digital thread", Module 14).

### B4. Control plan extract (example: cathode coating)

| Process step | Characteristic | Class | Spec | Method | Sample | Control method | Reaction plan |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Coating | Areal loading | SC | Target ± x% **[P]** | β-gauge | 100% scan | Closed loop + SPC (EWMA) | Out of limit → auto-mark section; 3 points trend → stop & check slurry solids |
| Coating | Edge profile | — | ≤ y µm above nominal **[P]** | Profile gauge | 100% | SPC | Adjust shim; segregate roll |
| Drying | Residual NMP | — | ≤ z ppm **[P]** | GC | 1 per roll | Check sheet | Hold roll; adjust oven |
| Coating | Surface defects | SC (pinholes on anode) | None > size limit | Vision | 100% | Defect map to MES | Auto-skip at notching |
| Drying | Adhesion | — | ≥ N/m **[P]** | Peel test | 1 per roll start/end | SPC | Hold roll |

## Part C — Process FMEA (major stages)

Ratings use a 1–10 scale; AP = AIAG-VDA Action Priority (H/M/L) **[E — illustrative ratings]**.

| # | Process step | Failure mode | Effect | S | Cause | O | Current prevention | Current detection | D | AP | Recommended action |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Material receipt | Metallic contamination in CAM | Micro-short, thermal event | 10 | Supplier process wear | 3 | Supplier PPAP, magnets at supplier | Lot ICP magnetic test | 5 | H | 100% lot test after PCN; line magnets with catch logging |
| 2 | Material storage | High-Ni CAM absorbs moisture | Gelation, gas | 7 | Exposure after opening | 5 | SOP | KF on sample | 5 | H | MES exposure clock, dry storage only |
| 3 | Mixing | Agglomerates | Streaks, separator puncture | 8 | Wrong sequence, short time | 4 | Recipe lock | Grind gauge per batch | 4 | M | Inline filter ΔP monitoring |
| 4 | Mixing | Gelation | Batch scrap, coating defects | 6 | Moisture, temp, pot life | 4 | Jacket cooling, pot-life rule | Viscosity checks | 4 | M | Viscosity vs time check at 2 h |
| 5 | Mixing | Metal wear debris | Micro-short | 10 | Blade/seal wear | 2 | Ceramic/WC wear parts | Magnetic filter | 5 | H | Wear-part PM by hours; catch trend |
| 6 | Coating | Coat weight low (anode) | Lithium plating | 9 | Pump drift, density change | 3 | Closed loop | 100% β-gauge | 2 | M | Gauge MSA, redundancy |
| 7 | Coating | Pinholes / uncoated spots | Local plating, corrosion | 8 | Bubbles, foil contamination | 4 | Degassing, foil spec | Vision 100% | 3 | M | Auto-skip marked sections |
| 8 | Coating | Streaks | Capacity spread, plating | 7 | Particles at die lips | 4 | Filtration | Vision, profile | 3 | M | Lip inspection per roll change |
| 9 | Drying | Binder migration / delamination | Particles, capacity loss | 7 | Drying too fast | 4 | Oven profile validation | Peel test per roll | 5 | M | Inline adhesion proxy; airflow survey PM |
| 10 | Drying | Residual solvent | Gas, fade | 6 | Speed too high | 3 | Speed–oven interlock | GC sample | 5 | M | Increase sampling during speed change |
| 11 | Calendering | Over-densification | Slow wetting, plating | 7 | Gap error, material change | 3 | Recipe per material | Thickness gauge, density sample | 4 | M | Compaction curve in PPAP |
| 12 | Calendering | Foil wrinkles | Misalignment, tab cracks | 6 | Edge stress | 5 | Edge stretching | Vision | 4 | M | Design narrower margins |
| 13 | Slitting/notching | Burr above limit | Separator puncture → short | 10 | Knife/die wear, laser beads | 4 | Tool life by metres | Sample microscopy + vision | 4 | H | Inline burr vision; tighter tool life |
| 14 | Slitting/notching | Loose particles | Micro-short | 10 | Poor extraction | 4 | Extraction, brushes | Particle counts | 5 | H | Extraction ΔP interlock |
| 15 | Vacuum drying | Residual moisture | HF, gas, fade | 8 | Short cycle, leak | 3 | Recipe, leak test | KF sample | 5 | H | Moisture sensor in chamber; exposure-time interlock |
| 16 | Winding/stacking | Misalignment / overhang loss | Plating, short | 9 | Web wander, placement error | 3 | EPC, vision | CCD + X-ray (sample or 100%) | 3 | M | 100% X-ray for new design ramp |
| 17 | Winding/stacking | Separator damage | Short | 10 | Tension spike, gripper | 3 | Tension control | Hi-pot 100% | 3 | M | Gripper PM, tension alarms |
| 18 | Tab welding (US) | Weak weld | High IR, open | 7 | Horn wear | 4 | PM by count | Signature monitoring, sample peel | 4 | M | Signature-based 100% reject |
| 19 | Laser welding | Spatter particles in cell | Micro-short | 10 | Contamination, parameters | 4 | Shields, extraction | Vision; later OCV | 6 | H | Wobble/green laser; spatter shield cleaning interval |
| 20 | Lid seal weld | Leak | Moisture ingress, leak | 8 | Gap, contamination | 3 | Fixture design | He leak 100% | 2 | L | — |
| 21 | Filling | Under-fill | Fade, plating | 8 | Pump wear, bubbles | 3 | Pump PM | 100% weighing | 2 | M | Per-station SPC |
| 22 | Filling | Moisture ingress | HF, gas | 8 | Dew-point excursion | 3 | HVAC, headcount | Dew-point monitoring | 4 | M | Interlock filling on dew point |
| 23 | Formation | Lithium plating | Capacity loss, dendrites | 9 | C-rate too high, poor wetting, cold | 3 | Validated recipe | dQ/dV analytics, capacity | 5 | H | Wetting check before formation; temperature mapping |
| 24 | Formation | Thermal event in rack | Fire | 10 | Internal short | 2 | Upstream controls | Per-cell T/V monitoring | 3 | M | Automated isolation; suppression testing |
| 25 | Degas / pouch seal | Seal channel leak | Moisture ingress over life | 8 | Electrolyte in seal area | 4 | Wipe station | Vacuum decay test | 4 | M | Seal-area protection during fill |
| 26 | Aging | Micro-short not detected | Field failure | 10 | Aging too short, fixed limits | 3 | Recipe | K-value | 5 | H | Dynamic limits, LFP SOC selection, µV meters |
| 27 | Grading | Wrong bin | Pack imbalance | 6 | Gauge drift | 3 | Calibration | MSA | 4 | L | — |
| 28 | Final test | Label/ID mismatch | Traceability loss | 7 | Handling error | 2 | Auto marking | Code verification | 2 | L | — |

**How to use:** pick the H items first; most are **detection** problems with long delays. The cheapest actions are usually **prevention at the source** (tool life, extraction, moisture interlocks) rather than more EOL testing.

## Part D — Root cause analysis and 8D in a cell plant

1. **D1–D3 Team and containment:** quarantine by genealogy (lot, roll, lane, station, date range) — this is where traceability pays for itself.
2. **D4 Root cause:** combine data analytics (which upstream variable separates good and bad cells?) with **tear-down**: CT scans for alignment/particles, SEM/EDS on particles (identify Fe/Cu/stainless), ICP for metal content, separator inspection.
3. **D5–D6 Corrective actions:** prevention at source; verify with Cpk and, for life-related issues, accelerated tests.
4. **D7 Prevent recurrence:** update PFMEA, control plan, lessons-learned database across lines and plants.
5. **D8 Closure.**

## Interview questions

1. Which characteristics would you classify as special characteristics for an EV cell and why?
2. How do you do MSA on a coat-weight gauge?
3. Why does autocorrelation matter for SPC on inline gauges?
4. Walk me through containment for a customer complaint of high self-discharge.
5. Why are many High-AP items in a cell PFMEA detection problems?

## Quiz

1. Typical Cpk target for special characteristics?
2. What replaces RPN in AIAG-VDA FMEA?
3. What tool identifies particle composition during tear-down?
4. Which chart type is good for slow drifts?
5. Name three gauges that need careful MSA in a cell plant.

<details><summary>Answers</summary>

1. ≥1.67 **[T]**.
2. Action Priority (AP).
3. SEM with EDS.
4. EWMA (or CUSUM).
5. Coat-weight gauge, thickness gauge, checkweigher, OCV/IR meter (any three).
</details>

## Hands-on exercise

Extend the PFMEA above with five failure modes for your own chosen format (cylindrical, prismatic or pouch) that are not yet listed. Rate S/O/D with your reasoning, set AP, and add actions. Then write a full control plan for Stage 8 (filling) using the template in B4.

**Next:** [Module 13 — Defects and failure analysis](13-defects-and-failure-analysis.md)
