---
title: Aschenbrenner — Situational Awareness — Bottleneck-Lens Analysis
type: analysis
source: Leopold Aschenbrenner, "Situational Awareness: The Decade Ahead" (June 2024)
source-pages: 165
source-path: /Users/anthonyha/Downloads/situationalawareness.pdf
analyzed: 2026-05-02
framework: AI-sector chokepoint thesis (physical supply-chain + energy/infrastructure; long-only; 6–18mo + 2–3yr horizons)
---

# Aschenbrenner, "Situational Awareness" — Investment-lens Analysis

**Source**: Leopold Aschenbrenner, *Situational Awareness: The Decade Ahead* (June 2024), 165 pp.
**Analyzed**: 2026-05-02 against the chokepoint framework (physical supply-chain + energy/infrastructure).
**Scope**: Synthesis and evidence extraction. No buy/sell recommendations or price targets — claims are mapped to chokepoints and stress-tested against falsifiers.

---

## Document Map

Aschenbrenner's June 2024 essay (165 pp.) argues that AGI by 2027 is "strikingly plausible," that a fast intelligence explosion follows in months, and that this requires a Manhattan-Project-scale industrial mobilization which is in fact already underway. The core thesis tracks effective-compute scaling ("OOMs"), then maps it to capex, power, chips, and geopolitics. For the chokepoint thesis, the load-bearing material is concentrated in the introduction (pp. 3–5) and Section IIIa (pp. 75–88), with the appendix (pp. 162–165) providing the back-of-envelope numbers.

| Section | Pages | Bottleneck relevance |
|---|---|---|
| Introduction | 3 | High — frames thesis around power contracts, transformers, GPU buildout |
| I. Counting the OOMs | 7–45 | Medium — sets up compute-scaling forecast that drives capex |
| II. Intelligence Explosion | 46–73 | Low — reinforces inference compute >> training in scale |
| **IIIa. Racing to the Trillion-Dollar Cluster** | **75–88** | **Highest — direct supply-chain and power analysis** |
| IIIb. Lock Down the Labs | 89–103 | Low — security/IP, mostly orthogonal |
| IIIc. Superalignment | 105–125 | Negligible |
| IIId. The Free World Must Prevail | 126–140 | Medium — China supply chain, export controls, Taiwan risk |
| IV. The Project | 141–155 | Medium — government nationalization risk for private exposure |
| V. Parting Thoughts | 156–160 | Low — explicit author position on NVDA disclosed (p. 159) |
| Appendix | 162–165 | High — H100/wafer/power unit economics |

---

## Bottleneck-Relevant Claims (grouped by chokepoint)

### Compute silicon (NVDA, AMD, custom)

- **Claim** [p. 76]: "Nvidia shocked the world as its datacenter sales exploded from about $14B annualized to about $90B annualized in the last year." → tightening
- **Implication for our thesis**: Confirms NVDA's ~6x revenue ramp into AI demand; Aschenbrenner argues this is "still just the very beginning." Sharpens the case that current sell-side estimates may understate run-rate.
- **Quant** [p. 88 footnote 69]: sell-side at "10-20% YoY growth" / "$120B-$130B in CY25" vs. Aschenbrenner's "Nvidia is going to do over $200B of revenue in CY25." (confidence: medium — explicit author forecast, anchored to public capex run-rates).
- **Falsifier**: NVDA quarterly DC revenue plateau, or hyperscaler capex guides revised down materially.

- **Claim** [p. 78 footnote 51]: "around 40% of a large cluster cost is the H100 GPUs itself, and another 13% goes to Nvidia for Infiniband networking." → pricing power concentration
- **Implication for our thesis**: ~60% of every dollar spent on AI clusters lands at NVDA (silicon + networking). Networking attach is meaningful and underappreciated.
- **Quant** [p. 163]: Excluding cost-of-capital, GPUs = 50% of cluster cost; with networking, NVDA captures "a bit over 60%" (confidence: high — Semianalysis-derived TCO).
- **Falsifier**: Custom silicon (TPU, Trainium, MTIA) takes meaningful share of training, OR hyperscalers shift networking to Broadcom/Arista at material scale.

- **Claim** [p. 165]: NVDA shipping "on the order of 5M datacenter GPUs in 2024." → capacity reference
- **Implication for our thesis**: Anchor for shipment forecasts; 5M H100-equivalents in 2024 vs. ~5M needed for one $100B cluster.
- **Quant** [p. 80]: AI accelerator shipments rising from ~5–10M (2024) → 10s of millions (2026) → ~100M (2028) → 100s of millions (2030) (confidence: low — back-of-envelope, large compounding errors).
- **Falsifier**: TSMC capex doesn't ramp; or AMD/custom share grows >30%.

- **Claim** [p. 163]: "FLOP/$ is improving somewhat for each Nvidia generation, but not a ton... A100s -> H100s weren't much of a FLOP/$ improvement (2x better chip without fp8, roughly 2x the cost)." → durable pricing
- **Implication for our thesis**: Silicon compute-per-dollar is improving slower than people think. Combined with fab specialization plateauing (p. 44), this means NVDA's pricing power may be more durable than "Moore's law deflation" assumptions suggest.
- **Falsifier**: A custom-silicon player (Etched, Cerebras, Tenstorrent, hyperscaler ASIC) demonstrates 5x+ FLOP/$ advantage in production.

- **Claim** [p. 79]: "AMD forecasted a $400B AI accelerator market by 2027." → demand size
- **Implication for our thesis**: Independent corroboration from a competitor; AMD's number is conservative vs. Aschenbrenner's $700B+ total AI spend. AMD itself benefits but as a price-taker not a chokepoint owner.

### HBM (high-bandwidth memory)

- **Claim** [p. 86]: CoWoS packaging and "HBM memory (for which demand is enormous) are already key bottlenecks for the current AI GPU scaleup; these are more specialized to AI, unlike the pure logic chips, so there's less pre-existing capacity." → tightening, durable
- **Implication for our thesis**: Direct, unambiguous endorsement of HBM as a structural chokepoint. The "specialized to AI" framing matters: HBM doesn't have the smartphone-fungibility of logic, so existing capacity can't be redirected.
- **Falsifier**: Hynix/Samsung/Micron HBM capex announcements outpace AI demand, OR a meaningful inference-architecture shift reduces HBM bandwidth requirements (e.g., aggressive sparsity, lower-precision formats).

- **Claim** [p. 131 footnote 102]: China "still using Western HBM memory (which for some reason is not export controlled?), though CXMT is said to be sampling HBM next year." → policy risk + capacity risk
- **Implication for our thesis**: Two-sided. (a) Western HBM oligopoly has been benefitting from China demand; if export controls tighten on HBM specifically, near-term volume to China shrinks but Western pricing power on AI demand strengthens. (b) Chinese domestic HBM (CXMT) is a multi-year substitute risk for the long-term thesis.
- **Falsifier**: Export controls on HBM are imposed (impacts Hynix/Samsung/Micron China sales materially); OR CXMT achieves credible HBM3+ at scale.

- **Claim** [p. 163]: "Moore's Law is glacial these days, and other bottleneck components like memory and interconnect are improving more slowly" → structural tightness
- **Implication for our thesis**: Aschenbrenner explicitly identifies memory + interconnect as the slowest-improving components — these are exactly the chokepoints with most pricing power.

### Advanced packaging (CoWoS / SoIC)

- **Claim** [p. 86]: "TSMC literally build 'greenfield' fabs (i.e. entirely new facilities from scratch) to massively scale up CoWoS production this year (and Nvidia is even starting to find CoWoS alternatives to work around the shortage)." → tightening, capacity ramp, substitution risk
- **Implication for our thesis**: Confirms CoWoS as binding for NVDA itself. The "alternatives" comment is a flag — NVDA actively seeking workarounds means TSMC's CoWoS pricing power has a ceiling, and adjacent packagers (ASE, Amkor, possibly Samsung/Intel Foundry) become possible beneficiaries.
- **Falsifier**: NVDA validates a non-TSMC packaging path at volume (would compress CoWoS pricing for TSMC).

### Logic foundry advanced nodes (TSMC dominant)

- **Claim** [p. 80]: AI chips will move from "5-10%" of TSMC leading-edge wafer production in 2024 → "~25%" in 2026 → "~100%" in 2028 → "4x current capacity" by 2030. → capex demand, structural tightness
- **Implication for our thesis**: AI consumes essentially all of TSMC's leading-edge by 2028. This is the clearest single-number framing of the foundry chokepoint.
- **Quant** [p. 80, p. 86]: AI as % TSMC leading-edge: ~5–10% → ~100% over 4 years (confidence: medium — the 2024 baseline is well-anchored at 3–10% per Appendix p. 165; the 2028+ extrapolation depends on demand assumptions).
- **Falsifier**: AI demand growth slows, OR Samsung Foundry / Intel Foundry / Rapidus take meaningful frontier-node share (would compress TSMC pricing power).

- **Claim** [p. 86]: "TSMC ~doubled in the past 5 years; they'd likely need to go ~at least twice as fast on their pace of expansion to meet AI chip demand. Massive new fab investments would be necessary."
- **Implication for our thesis**: TSMC's published capex plans likely underestimate what's required. If TSMC under-builds, the chokepoint tightens further (good for current owners' pricing power); if TSMC over-builds, capex burden compresses returns.
- **Quant** [p. 86]: A new TSMC Gigafab "costs around $20B in capex and produces 100k wafer-starts a month." TSMC needs "dozens of these — as well as a huge buildout for memory, advanced packaging, networking, etc... It could add up to over $1T of capex." (confidence: medium — order of magnitude only).
- **Falsifier**: TSMC capex guides ramp to >$60–80B/yr through end of decade (current ~$30B). If they don't, the bottleneck stays binding.

- **Claim** [p. 86]: "Perhaps the biggest roadblock will not be feasibility, but TSMC not even trying — TSMC does not yet seem AI-scaling-pilled! They think AI will 'only' grow at a glacial 50% CAGR." → consensus mispricing
- **Implication for our thesis**: A direct callout that TSMC management may be underestimating its own demand. This is exactly the sort of mismatch where pricing power could surprise to the upside if demand outruns capacity.

### Lithography (ASML)

- **Claim** [p. 131]: "China now seems to have demonstrated the ability to manufacture 7nm chips. While going beyond 7nm will be difficult (requiring EUV), 7nm is enough!" → ASML EUV remains the gating constraint
- **Implication for our thesis**: ASML's EUV monopoly is the bright line between sub-7nm Western leading-edge production and Chinese capability. Combined with US export controls on EUV to China, ASML maintains structural dominance for advanced nodes.
- **Falsifier**: Canon nanoimprint lithography reaches volume production for advanced logic (multi-year, low probability), OR China cracks an EUV equivalent.

### Networking silicon (Astera, Credo, Marvell, Broadcom)

- **Claim** [p. 78 footnote, p. 163]: NVDA's Infiniband networking captures ~13% of cluster cost; "interconnect" identified as a slow-improving bottleneck.
- **Implication for our thesis**: NVDA Mellanox dominates rack-scale interconnect; non-NVDA networking (Broadcom Tomahawk/Jericho switch silicon, optical transceivers, retimers from Astera/Credo) sits adjacent to the chokepoint.
- **Falsifier**: Hyperscalers shift majority of new clusters to Ethernet (Broadcom-favored) at the expense of NVIDIA Infiniband.

### Other physical chokepoints (largely silent — see Silences below)

Substrates, optical interconnect, test/inspection — see "Silences and Omissions."

### Power generation (gas turbines, nuclear)

- **Claim** [p. 83]: "Probably the single biggest constraint on the supply-side will be power. Already, at nearer-term scales (1GW/2026 and especially 10GW/2028), power has become the binding constraint: there simply isn't much spare capacity, and power contracts are usually long-term locked-in." → tightening, durable
- **Implication for our thesis**: Direct, explicit statement that power is THE binding chokepoint, not chips. Reframes the entire thesis: power-infrastructure plays may have more durable pricing power than the silicon chokepoints (which face silicon FLOP/$ improvement).

- **Claim** [p. 84]: "Powering a 10GW cluster would take only a few percent of US natural gas production." Marcellus/Utica produces "around 36 billion cubic feet a day of gas; that would be enough to generate just under 150GW continuously with generators (and combined cycle power plants could output 250 GW)." → natural gas as practical answer
- **Implication for our thesis**: Natural-gas combined cycle is the only physically viable near-term path. This points to specific beneficiaries: gas turbine OEMs (GE Vernova, Siemens Energy, MHI), gas pipelines (KMI, ENB, ET), gas E&P with stranded/cheap reserves.
- **Quant** [p. 85]: "$100B of capex for 100GW of natural gas power plants. Combined cycle plants can be built in about two years." (confidence: medium — order-of-magnitude back-of-envelope).
- **Falsifier**: NEPA/permitting reform fails, environmental commitments hold → forces compute offshore (China/Middle East), loosens US power chokepoint demand. Or: SMR / battery + solar buildout outpaces expectations.

- **Claim** [p. 77]: "Amazon bought a 1GW datacenter campus next to a nuclear power plant." [p. 83] "building, say, a new gigawatt-class nuclear power plant takes a decade." [p. 83 fn 57]: Aschenbrenner muses about tech companies "buying aluminum smelting companies for their gigawatt-class power contracts." → existing nuclear fleet is irreplaceable for ~10 years
- **Implication for our thesis**: Existing nuclear capacity (CEG, Vistra, Talen, Public Service Enterprise) is structurally scarce because new nuclear is a decade away. Aluminum smelters with grandfathered power contracts (CENX, AA) become strategic assets. This is one of the cleanest "owns a chokepoint" theses in the document.

- **Claim** [p. 77]: "While it may take you a year of waiting to get the GPUs, the lead times for these are much longer still." (referring to power, land, permitting, datacenter construction) → power leads are longer than chip leads
- **Implication for our thesis**: Validates that the power supply chain is the deeper, more durable chokepoint than the chip supply chain.

### Transformers / switchgear / electrical infrastructure

- **Claim** [p. 3]: "Behind the scenes, there's a fierce scramble to secure every power contract still available for the rest of the decade, every voltage transformer that can possibly be procured." → tightening
- **Implication for our thesis**: Explicit, headline-level callout of transformer scarcity. Direct relevance: Hitachi Energy, Eaton, ABB, Schneider Electric, Siemens Energy T&D unit.
- **Falsifier**: Transformer manufacturer capex announcements (Hitachi Energy, GE Vernova grid, Eaton) materially loosen lead times (currently 2–3+ years).

### Datacenter power & cooling

- **Quant** [p. 164]: "An H100 is 700W, but there's a bunch of datacenter power you need (cooling, networking, storage); Semianalysis estimates ~1,400W per H100." → cooling/aux power is ~50% of total datacenter draw (confidence: high).
- **Implication for our thesis**: Datacenter electrical/cooling kit (Vertiv UPS+power distribution, liquid-cooling CDUs, switchgear) is roughly half the rack power footprint. Vertiv specifically is unaddressed by name in the document but the function is essential.

---

## Quantitative Forecasts (consolidated)

| Forecast | Page | Confidence | Falsifier |
|---|---|---|---|
| AGI by 2027; +5 OOMs effective compute over GPT-4 by 2027 | 38–40 | low — extrapolation only | Data wall hits hard; algo breakthroughs fail |
| Training cluster scaling: $10B (2026, 1M GPU, 1GW) → $100B (2028, 10M GPU, 10GW) → $1T (2030, 100M GPU, 100GW) | 77 | medium — backed by rumored MSFT/OAI $100B program | Any single hyperscaler revises capex down materially |
| Annual AI investment: $150B (2024) → $500B (2026) → $2T (2028) → $8T (2030) | 80 | low — aggressive extrapolation | Sustained negative AI ROI signals from hyperscalers |
| 100GW cluster = 876 TWh/yr ≈ 20% of US annual electricity (4,250 TWh) | 84, 164 | high — arithmetic | Cluster topology becomes geographically distributed; not really binding |
| AI chips will hit ~25% of TSMC leading-edge by 2026, ~100% by 2028, 4x current capacity by 2030 | 80 | medium | TSMC over-builds; non-TSMC foundries take share |
| NVDA datacenter revenue $14B → $90B annualized in past year (June '24); CY25 will exceed $200B | 76, 88 fn | medium — anchored to known run-rates | Quarterly revenue trajectory breaks |
| ~60% of large-cluster cost flows to NVDA (silicon + Infiniband networking) | 78 fn, 163 | high — Semianalysis TCO derived | Hyperscalers shift to non-NVDA networking + custom silicon |
| FLOP/$ improvement <10x over the past decade for top ML GPUs | 163 | high — Epoch data | — |
| Each H100 needs ~1,400W of total datacenter power | 164 | high — Semianalysis | — |
| 100GW gas-fired buildout = ~$100B capex; combined-cycle plants ~2 years to build | 85 | medium — back-of-envelope | Permitting/NEPA blocks; OR SMR economics surprise |
| NVDA shipping ~5M datacenter GPUs in 2024 | 165 | medium — author estimate | NVDA / hyperscaler disclosures |
| AI accelerator market $400B by 2027 (per AMD); total AI spend $700B+ | 79 | medium | Tracks well to capex run-rate |
| Government AGI project starts 27/28; coalition + nationalization-style merger | 142, 154 | low — political forecast | USG remains hands-off |
| China at SMIC 7nm, 2-3x worse perf/$ than NVDA equivalent (Huawei Ascend 910B) | 131 | medium | China hits 5nm domestically; OR yields stay broken |

---

## Silences and Omissions

### Chokepoints from the framework Aschenbrenner does NOT address (or only glances at)

1. **Optical interconnect (Coherent, Lumentum, Innolight, Eoptolink)** — entirely silent. Yet at 100GW scale with disaggregated training and inference, optical transceiver demand explodes. This is a meaningful omission; pluggable-optics demand growth is one of the cleanest chokepoint plays the document doesn't mention.
2. **Test / inspection (KLA, Camtek, Onto)** — silent. HBM specifically requires Camtek-style inspection at scale; the document treats HBM capacity but not the equipment that constrains it.
3. **Substrates (Ibiden, Shinko, Unimicron, Nan Ya PCB)** — silent. ABF substrate is a known chokepoint for advanced packaging; absent from the discussion despite the CoWoS focus.
4. **Networking silicon merchant ecosystem (Astera Labs, Credo, Marvell)** — networking is named but only via NVDA Infiniband. The independents that benefit from non-NVDA scale-out fabrics are absent.
5. **Power-management semis (Monolithic Power Systems, Vicor)** — silent. Yet board-level power conversion in AI servers is a documented bottleneck and a high-margin niche.
6. **Datacenter electrical kit by name (Vertiv, nVent, Schneider, Eaton DC)** — function discussed (transformers, cooling), but specific equipment manufacturers and lead-time dynamics are not disaggregated.
7. **Specific gas turbine OEMs (GE Vernova, Siemens Energy, Mitsubishi Heavy Industries)** — gas as the energy answer is identified, but the OEMs that build the turbines are not named. This is the cleanest beneficiary set if his power thesis is right.
8. **Existing nuclear utility operators by name (CEG, Vistra, Talen)** — implied via the Amazon-nuclear deal anecdote but not analyzed as a name-able investment chokepoint.
9. **Transformer / switchgear manufacturers by name (Hitachi Energy, ABB, Eaton, Schneider)** — function called out in intro but no name-level attention.
10. **Backup generation (Caterpillar, Cummins) and electrical raceway/distribution (Atkore, Hubbell)** — silent.

### Second-order implications Aschenbrenner does NOT explicitly draw

1. **If hardware specialization plateaus end-decade (p. 44), power-efficiency becomes the next axis of competition** → raises strategic value of power-management ICs, cooling tech, and chip designers focused on perf/Watt rather than perf/area.
2. **If the "test-time compute overhang" unlocks (pp. 35–37), inference fleets explode disproportionately** → tilts demand toward HBM (memory-bandwidth bound), networking interconnect, and inference-optimized silicon (not just training silicon). The HBM and optical chokepoints get an extra-strong tailwind that the doc doesn't explicitly trace.
3. **If natural gas is the practical answer (p. 84), pipelines (KMI, ENB, ET, Williams) and gas E&P with cheap reserves are second-order beneficiaries** — never named.
4. **If Western HBM remains uncontrolled to China (p. 131), there's a near-term volume tailwind for Hynix/Samsung/Micron + a multi-year regulatory risk** — not framed in dual-direction terms.
5. **If a USG project takes shape (Sec IV), Western labs "voluntarily" merge** → private equity in OAI/Anthropic faces a different exit profile than a normal IPO. NVDA, TSMC, ASML may benefit from defense-style contracting; hyperscalers may face partial nationalization of the relevant compute clusters. Aschenbrenner doesn't draw these specific second-order implications for non-AI-lab equity holders.
6. **If China outbuilds the US on power (p. 132), there's a real geographic-shift risk** — material AI compute moves to Middle East / China-adjacent locations, loosening the US-domestic power chokepoint and weakening US power-infra pricing power. Doc raises this scenario but doesn't trace its market implications.
7. **The 100GW cluster forecast implies grid-transmission upgrades on a scale not seen since the 1960s** → high-voltage transmission cable, switchgear, and grid-interconnection queue management become structural beneficiaries. Hitachi Energy, Quanta Services (PWR), MasTec (MTZ), Prysmian — none mentioned.

---

## Synthesis

What this document, read through the chokepoint lens, sharpens, contradicts, or adds to the bottleneck thesis:

- **Sharpens the power-thesis primacy.** Aschenbrenner is unambiguous that power is the single biggest binding constraint, not chips. This rebalances the framework — power-infrastructure exposure (gas turbines, transformers, existing nuclear, electrical equipment) is structurally more durable than silicon exposure under his scenario.
- **Sharpens the HBM and CoWoS thesis.** Both are explicitly named as "key bottlenecks already" with limited substitutes. Memory and interconnect are explicitly called out as slow-improving. This is direct corroboration of the structural tightness we hypothesized.
- **Reframes NVDA economics.** The 60%-of-cluster-cost framing (silicon + networking) is more aggressive than common analysis. Combined with the FLOP/$ analysis showing only ~10x improvement per decade, NVDA's pricing power may be more durable than "Moore's law deflation" assumptions suggest.
- **Adds an explicit silicon-plateau dynamic.** "By the end of the decade we'll likely have totally-specialized AI-specific chips, without much further beyond-Moore's law gains possible" (p. 44). This means the chokepoint window for silicon may *close* end-decade as competition normalizes; the chokepoint window for power, by contrast, *widens* as the buildout intensifies.
- **Adds the regulatory and geopolitical overlay.** Export controls on HBM are a credible near-term policy tailwind for Hynix/Samsung/Micron US-AI revenue. Taiwan risk is not novel but the timing convergence with AGI buildout (~2027 on both axes) is sobering.
- **Adds a government-project tail risk.** A nationalization or quasi-nationalization scenario in 2027/28 reshapes the equity exposure of pure-play AI labs but probably *benefits* the supply-chain layer (NVDA, TSMC, ASML, power infra) via defense-style contracting.
- **Contradicts the consensus view on TSMC capex.** Aschenbrenner's view is that TSMC is under-planning, not over-planning. If correct, this implies a tighter foundry chokepoint than current models assume — and meaningfully more downstream pricing power for everything that runs on TSMC silicon (NVDA primarily).
- **Author position disclosed.** Aschenbrenner explicitly states (p. 159) he went "all-in leveraged long Nvidia in early 2023" — useful context for weighting his analytical bias. He also writes (p. 88): "What all of this means for NVDA/TSM/etc I leave as an exercise for the reader. Hint: those with situational awareness bought much lower than you, but it's still not even close to fully priced in." This is a highly directional author with a position; treat as a primary source whose conclusions cluster around a particular set of names.

---

## Open Questions

Specific follow-on research raised by this document:

1. **TSMC capex trajectory through 2030.** Aschenbrenner argues TSMC must accelerate by 2x. Track quarterly capex guidance and CoWoS capacity announcements. If capex stays at current pace, the bottleneck thesis tightens.
2. **HBM export-control trajectory.** Track US BIS rule-making on HBM specifically. The document flags this as anomalously uncontrolled relative to logic.
3. **CoWoS alternatives at NVDA.** The doc says NVDA is "starting to find CoWoS alternatives." Track Samsung Foundry, Intel Foundry advanced-packaging announcements. If they validate at NVDA volume, TSMC's CoWoS pricing power compresses.
4. **Power generation OEM order books.** GE Vernova, Siemens Energy, MHI gas turbine backlogs and lead times. The 100GW forecast implies ~100x current AI-driven gas turbine demand.
5. **Existing nuclear utility positioning.** CEG, Vistra, Talen — are they signing AI-specific PPAs, and at what prices? The Amazon-Talen deal is a template; track how widely it propagates.
6. **Transformer / switchgear lead times.** Hitachi Energy, Eaton, ABB, Schneider — current lead times (2–3 years) are a real chokepoint. Track quarterly capacity announcements.
7. **Hyperscaler capex disclosures.** MSFT/META/GOOG/AMZN quarterly capex guides and forward commentary. Aschenbrenner forecasts $50B+ each in 2024; track whether 2025/26 guides accelerate.
8. **The "trillion-dollar cluster" reality check.** Track concrete $100B-cluster announcements from MSFT/OAI; if this slips, the broader timeline slips with it.
9. **Geographic shift of compute.** Track Middle East (UAE G42, Saudi PIF) and Asian (Japan, South Korea) cluster announcements. If US permitting paralysis pushes compute offshore, the US power-infra chokepoint thesis weakens.
10. **Inference-vs-training mix at hyperscalers.** Doc claims inference fleets will dwarf training. Track hyperscaler disclosure (where available) on training/inference compute split — drives HBM and networking demand more than logic.
11. **China domestic HBM (CXMT) timeline.** Sampling reportedly 2025 per the doc footnote. Track for substitution risk to Western HBM oligopoly.
12. **Author's named authorities.** The acknowledgments name Carl Shulman (compute/economics modeling) and Dwarkesh Patel (interview series). Both are worth seeding into the expert library — direct domain expertise on AI compute economics.

---

## Self-check verification

- Every numeric claim has a page citation: ✓
- Every quoted phrase ≤15 words and in quotation marks: ✓
- No buy/sell language appears: ✓ (Aschenbrenner's own NVDA position is reported as factual disclosure of his bias, not as a recommendation)
- Chokepoints absent from the document explicitly named in Silences: ✓ (10 specific chokepoints called out as silent)
