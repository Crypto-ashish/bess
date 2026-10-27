# Module 16 — Capstone: Interview Guide, Glossary and Resources

*Li-ion Cell Manufacturing: an Engineer's Course · Phase D · Evidence labels: [V] verified · [T] typical practice · [E] estimate · [P] proprietary*

**Bottom line:** you are ready when you can (1) walk the line from powder to pallet and explain *why* each control exists, (2) translate every battery quality problem into the APQP/PFMEA/SPC language you already speak, and (3) put a cost on a yield, uptime or capex decision.

---

## Part A — Capstone project

**Design, on paper, a 5 GWh/yr LFP prismatic cell line for India.** Use your exercises from Modules 1–15.

| Deliverable | Content | From module |
| --- | --- | --- |
| 1. Cell design sheet | 280 Ah LFP: loadings, densities, N/P, overhangs, fill mass | 3, 4, 5, 7 |
| 2. Process flow diagram | All 12 stages with inspection points | 0 |
| 3. Equipment list | Machine counts by stage, OEM shortlist | 10 |
| 4. Line balance | Takt, cycle times, buffers, formation channels, aging positions | 6, 8, 10 |
| 5. Layout | Zones, dew points, flows, fire compartments, expansion | 11 |
| 6. PFMEA + control plan | Top 30 failure modes, special characteristics, reaction plans | 12 |
| 7. Defect playbook | Symptom → stage → data → action | 13 |
| 8. Cost model | Capex, $/kWh, sensitivities, break-even utilisation | 14 |
| 9. Supply plan | Indian vs imported materials and equipment, risks | 1, 15 |
| 10. Ramp-up plan | FAT/SAT, run-at-rate, yield learning curve, staffing | 10, 14 |

Present it as a 15-slide deck or a 10-page document — the format a plant director or interviewer would expect.

## Part B — Technical interview preparation guide

### B1. How interviews for cell-plant roles usually run **[T]**

1. **Fundamentals:** cell components, chemistries, SEI, why moisture matters.
2. **Process depth:** one or two stages in detail (the one you claim expertise in).
3. **Quality:** PFMEA, SPC, Cpk, 8D, MSA with battery examples.
4. **Problem-solving case:** "self-discharge rejects doubled — what do you do?"
5. **Commissioning/ramp-up:** FAT/SAT, run-at-rate, OEE.
6. **Cost/business:** where cost comes from; capex/yield trade-offs.
7. **Behavioural:** cross-functional work with OEM technicians (often Chinese/Korean), shift leadership, safety culture.

### B2. Question bank with answer outlines

| # | Question | What a strong answer covers |
| --- | --- | --- |
| 1 | Walk me through the cell process. | Three blocks; 12 stages; why dry room; formation as bottleneck; where defects are created vs detected |
| 2 | Why PVDF/NMP for cathode, water for anode? | Electrochemical stability at potentials; NMP dissolves PVDF; cost and toxicity; water-based cathode efforts |
| 3 | What controls coat weight? | Pump-metered flow, web speed, width; β/X-ray gauge closed loop; N/P safety link |
| 4 | Explain binder migration. | Drying physics; low–high–low; adhesion loss; how to detect (peel) |
| 5 | Porosity vs density? | Formula; energy vs rate; Bruggeman; wetting time |
| 6 | Burr specification? | Separator thickness; tool life by metres; inspection; SC classification |
| 7 | Winding vs stacking? | Speed, space use, stress, tabs; format fit |
| 8 | Why hi-pot before filling? | Detect shorts cheaply; voltage/limits; false-pass risk |
| 9 | Fill mass setting? | Pore volume + reserve; g/Ah; weighing MSA; Cpk |
| 10 | What is SEI and why slow formation? | EC reduction; lithium loss; plating risk; ORNL evidence on fast formation trade-offs |
| 11 | K-value testing? | OCV drift; fixed vs dynamic limits; LFP flat curve; temperature compensation |
| 12 | Self-discharge escape case | Containment by genealogy; data join; tear-down SEM/EDS; source fix; PFMEA update |
| 13 | Dry room design? | Dew point; desiccant wheel; pressure cascade; moisture loads; energy |
| 14 | Special characteristics of a cell? | Coat weight/N/P, burr, overhang, moisture, fill mass, K-value, welds |
| 15 | OEE on a coater vs a stacker? | Splices/roll changes vs micro-stops; quality losses as marked sections |
| 16 | Biggest cost levers? | Material/yield, capex/utilisation; labour minor; numbers from Module 14 |
| 17 | Formation sizing? | Channels = rate × hours ÷ availability; energy recovery |
| 18 | How do you run a material change? | PCN, PPAP-style revalidation: compaction curve, slurry behaviour, formation efficiency, life tests |
| 19 | India's ecosystem? | PLI status, Exide commissioning, imports, component scheme; announced vs operating capacity |
| 20 | Why do you, from automotive, fit here? | APQP/PFMEA/SPC rigour, commissioning, costing; humility on electrochemistry; examples |

### B3. Your story (suggested framing)

- **Bridge:** "Eight years in automotive product development and costing — should-cost, BOM analysis, PPAP/APQP, ECN ownership — plus paint-shop quality where environment control and defect Paretos rule. A cell plant combines the two: a paint-shop-like environment problem and a cost problem dominated by materials and yield."
- **Proof:** bring the cost model, the PFMEA and the capacity tracker from this course.

## Part C — Glossary

| Term | Meaning |
| --- | --- |
| ACIR | AC internal resistance, usually measured at 1 kHz |
| Active material | Material that stores lithium (cathode CAM, anode AAM) |
| Aging | Holding cells to stabilise SEI and screen self-discharge |
| Agglomerate | Cluster of particles not broken apart in mixing |
| Areal capacity | mAh per cm² of electrode |
| Areal loading (coat weight) | mg of dry coating per cm² |
| AS/RS | Automated storage and retrieval system |
| β-gauge | Beta-ray gauge measuring coat weight |
| BET | Specific surface area by gas adsorption |
| Binder | Polymer holding particles together and to foil (PVDF, CMC/SBR) |
| Binder migration | Binder carried to the surface during fast drying |
| Blade cell | BYD's long thin prismatic LFP cell |
| Burr | Raised metal edge from cutting |
| Calendering | Compressing electrodes between rolls |
| CAM | Cathode active material |
| CEI | Cathode–electrolyte interphase |
| CID | Current interrupt device in cylindrical caps |
| CMC | Carboxymethyl cellulose (anode thickener/dispersant) |
| Coating window | Stable operating region of a slot die |
| Comma coater | Knife-over-roll coater |
| Conversion cost | Cell cost minus materials |
| CTP | Cell-to-pack design |
| DCIR | DC internal resistance from a current pulse |
| Degassing | Removing formation gas before final seal |
| Dew point | Temperature at which air moisture condenses; dry-room metric |
| dQ/dV | Differential capacity analysis |
| Dry electrode | Solvent-free electrode process |
| Dry room | Room with very low dew point |
| DVA | Domestic value addition (PLI condition) |
| EC / EMC / DMC | Ethylene, ethyl methyl, dimethyl carbonate (solvents) |
| EIS | Electrochemical impedance spectroscopy |
| EOL | End-of-line test |
| EPC | Edge position control (web guiding) |
| FAT / SAT | Factory / site acceptance test |
| FEC / VC | Fluoroethylene / vinylene carbonate (SEI additives) |
| First-cycle efficiency | Discharge ÷ charge capacity on first cycle |
| Flotation dryer | Oven where the web floats on air jets |
| Formation | First controlled charge that forms SEI |
| Gelation | Slurry turning to gel (PVDF + base/moisture) |
| Genealogy | Full traceability of a cell's materials and process data |
| Gigafactory | GWh-scale cell plant |
| Grading | Sorting cells by capacity, IR, OCV |
| Grind gauge (Hegman) | Measures largest particles in slurry |
| Gurley | Separator air permeability |
| HAZ | Heat-affected zone of laser cut |
| He leak test | Helium mass-spectrometer leak detection |
| Hi-pot | High-voltage insulation test |
| Hot calendering | Calendering with heated rolls |
| ICP-OES/MS | Elemental analysis method |
| Intermittent coating | Coating with gaps along the web |
| Jelly roll | Wound electrode assembly |
| K-value | OCV drop rate during aging (mV/day) |
| Karl Fischer | Moisture titration |
| Lamination stacking | Laminating electrode–separator units before stacking |
| LFP / NMC / NCA / LTO | Cathode/anode chemistries |
| LiPF₆ | Electrolyte salt; hydrolyses to HF |
| Lithium plating | Metallic lithium deposited on anode |
| Mandrel | Core on which electrodes are wound |
| MES | Manufacturing execution system |
| Micro-short | Small internal short causing self-discharge |
| N/P ratio | Anode-to-cathode capacity ratio |
| NMP | N-methyl-2-pyrrolidone solvent |
| Notching | Cutting tab shapes into electrode margins |
| OCV | Open-circuit voltage |
| OEE | Overall equipment effectiveness |
| Overhang | Anode beyond cathode / separator beyond anode |
| PCN | Product/process change notification |
| PLI (ACC) | Production-linked incentive for advanced chemistry cells |
| Porosity | Void fraction of electrode |
| Pot life | Time a slurry stays usable |
| Pouch | Laminated-foil cell housing |
| Prismatic | Rigid rectangular can cell |
| PVDF | Polyvinylidene fluoride binder |
| Residual lithium | LiOH/Li₂CO₃ on high-Ni cathode surfaces |
| SBR | Styrene-butadiene rubber binder |
| Seal pin | Pin welded into prismatic fill port |
| SEI | Solid electrolyte interphase on the anode |
| Separator | Porous film between electrodes |
| Shutdown | Separator pore closure on heating |
| Slitting | Cutting rolls into lanes |
| Slot die | Pre-metered coating head |
| Solids content | Mass fraction of solids in slurry |
| Springback | Thickness recovery after calendering |
| Tabless | Full-edge current collection in cylindrical cells |
| Takt time | Available time ÷ required output |
| Tap charge | Small initial charge after filling |
| Telescoping | Axial shift of layers in a jelly roll |
| Tortuosity | Path-length factor for ion transport |
| Ultrasonic welding | Solid-state welding of foil stacks |
| UN 38.3 | Transport test standard for lithium cells |
| Wetting | Electrolyte penetration into pores |
| Z-fold | Stacking with zig-zag continuous separator |

## Part D — Recommended resources

### D1. Books **[T — well-known titles; check editions]**

| Title | Why |
| --- | --- |
| Korthauer (ed.), *Lithium-Ion Batteries: Basics and Applications*, Springer, 2018 | Includes production chapters by German industry and academia |
| Kirby Beard (ed.), *Linden's Handbook of Batteries*, 5th ed., McGraw-Hill, 2019 | Reference for chemistries and cell design |
| Yoshio, Brodd, Kozawa (eds.), *Lithium-Ion Batteries: Science and Technologies*, Springer, 2009 | Classic materials and cell technology |
| Newman & Balsara, *Electrochemical Systems*, Wiley | Theory behind porous electrodes (optional, deep) |

### D2. Papers and guides

| Reference | Use |
| --- | --- |
| PEM RWTH & VDMA, *Production Process of a Lithium-Ion Battery Cell*, 5th ed. (free) — [link](https://battery-news.de/en/2026/02/12/pem-and-vdma-update-guide-to-battery-cell-production/) | Whole process |
| Kwade et al., *Nature Energy* 2018 — [doi](https://doi.org/10.1038/s41560-018-0130-3) | Process–structure–property |
| Liu et al., *iScience* 2021 — [doi](https://doi.org/10.1016/j.isci.2021.102332) | Cost, energy, throughput per step |
| Wood et al., *Joule* 2019 — [doi](https://doi.org/10.1016/j.joule.2019.11.018) | Formation |
| Wood, ORNL NAATBatt 2019 slides — [pdf](https://assets-002.noviams.com/novi-file-uploads/naatbatt/Conference_Material/2019/W2-D_Wood_NAATBatt-2019-Presentation_Final.pdf) | Formation and wetting data |
| Zhang et al., electrode drying review, *Adv. Energy Mater.* 2022 — [preprint](https://discovery.ucl.ac.uk/id/eprint/10139917/3/Shearing_Main%20article_As%20submitted_26.10.2021.pdf) | Drying |
| *A Flexible Model for Benchmarking the Energy Usage of Automotive Lithium-Ion Battery Cell Manufacturing*, *Batteries* 2021 (SINTEF) — [record](https://sintef.no/en/publications/publication/1892466) | Plant energy |
| Degen et al., *Nature Energy* 2023, energy consumption of current and future cell production **[T — not opened]** | Energy |
| Duffner et al., *Nature Energy* 2021, post-Li-ion compatibility with Li-ion lines **[T — not opened]** | Sodium-ion comparison |
| Hawley & Li, *Journal of Energy Storage* 2019, electrode manufacturing review **[T — not opened]** | Electrode processes |
| IEEFA & JMK, ACC PLI assessment, Jan 2026 — [report](https://ieefa.org/resources/assessing-indias-incentive-scheme-enhance-battery-manufacturing-ecosystem) | India policy |
| BNEF Battery Price Survey 2025 — [press release](https://about.bnef.com/insights/clean-energy/lithium-ion-battery-pack-prices/) | Prices |

### D3. Videos, courses and communities **[T — search and verify availability]**

| Resource | Use |
| --- | --- |
| *The Limiting Factor* (YouTube) | Deep dives into cell design and manufacturing (cylindrical, tabless, dry electrode) |
| PEM RWTH Aachen and Fraunhofer FFB channels/webinars | Production research talks |
| The Battery Show India / Europe conference talks | Industry practice, equipment makers |
| Volta Foundation, *The Battery Report* (annual, free) | Industry overview |
| Faraday Institution reports | Manufacturing and supply-chain studies |
| NPTEL (IIT) courses on electrochemical energy storage | Indian-context fundamentals |
| Equipment OEM application notes (Dürr, Bühler, Hirano, Manz, Trumpf) | Machine-level practice |

## Final self-assessment

- [ ] I can draw the 12-stage flow from memory with environments and inspection points.
- [ ] I can derive porosity, N/P, takt, formation channels and cost per kWh by hand.
- [ ] I can write a PFMEA line and a control-plan line for any stage.
- [ ] I can explain three ways a metallic particle reaches a cell and how each is stopped.
- [ ] I can state India's operating vs announced cell capacity with sources and dates.
- [ ] I have the capstone pack ready to show in an interview.

**Back to start:** [Module 0 — Roadmap and line overview](00-roadmap-and-line-overview.md)
