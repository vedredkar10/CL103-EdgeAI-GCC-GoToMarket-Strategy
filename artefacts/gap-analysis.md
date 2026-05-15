# Competitive Gap Analysis
**Project:** GCC Edge AI Go-To-Market Strategy
**Client:** Dubai-based Edge AI hardware venture (anonymised)
**BA:** Ved Redkar | Visionize Consultancy LLP
**Version:** 1.0

---

## Methodology
Gap analysis was conducted through structured desk research and
stakeholder elicitation. The incumbent platform (NVIDIA Jetson-class
GPU) was mapped across five structural dimensions against the client's
Axelera Metis-based platform. Gaps were identified where the client's
architecture offered a structural advantage, and where gaps remained
that required closing before enterprise adoption was viable.

---

## Dimension 1: Power Consumption & Efficiency

| Factor | NVIDIA Jetson incumbent | Axelera Metis platform | Gap type |
|---|---|---|---|
| Sustained inference draw | Higher wattage | Lower wattage | Client advantage |
| Annual energy cost (30 nodes) | Higher | Lower | Client advantage |
| Annual energy cost (500 nodes) | Significantly higher | Significantly lower | Client advantage at scale |
| Cooling multiplier impact | Higher — more heat generated | Lower — less heat generated | Client advantage |
| UPS capacity required | Larger | Smaller | Client advantage |

**Gap insight:** Power efficiency advantage is modest at small scale
but compounds significantly across distributed deployments of 100+
nodes. The enterprise message is not electricity savings alone — it
is infrastructure complexity reduction. Lower power draw enables
smaller fans, reduced ventilation design, smaller UPS, denser cabinet
configuration, and lower long-term hardware degradation in 45–50°C
outdoor conditions.

**Note:** Specific wattage and cost figures redacted.

---

## Dimension 2: Ecosystem & ISV Integration

| Factor | NVIDIA Jetson incumbent | Axelera Metis platform | Gap type |
|---|---|---|---|
| Dominant framework | CUDA — proprietary | ONNX — open standard | Neutral |
| ISV ecosystem maturity | Large — established | Small — emerging | Client gap |
| Migration friction | None — ISVs already optimised | Moderate — model conversion required | Client gap |
| Engineering time to integrate | Low for CUDA-native ISVs | Higher — ONNX conversion + validation | Client gap |
| Lock-in effect | High — CUDA dependency | Low — ONNX portability | Client advantage |

**Gap insight:** The client faces a classic challenger adoption
problem. ISVs are optimised around CUDA stacks. Switching requires
engineering investment, validation cycles, and risk. The client must
reduce this friction by providing SDK support, integration
documentation, and structured 60-day technical validation engagements
that absorb the ISV engineering cost. Without this, the efficiency
advantage alone is insufficient to drive adoption.

---

## Dimension 3: Thermal Management & Reliability

| Factor | NVIDIA Jetson incumbent | Axelera Metis platform | Gap type |
|---|---|---|---|
| Heat generation under load | Higher | Lower | Client advantage |
| Cabinet thermal design complexity | More complex | Simpler | Client advantage |
| Extended temperature certification | Available for some SKUs | Required — must be certified | Client gap (must close) |
| IP certification | Available | Required — must be certified | Client gap (must close) |
| MTBF documentation | Available | Required — must be documented | Client gap (must close) |

**Gap insight:** The client's lower power draw creates a structural
thermal advantage — less heat means simpler cabinet design, smaller
fans, and reduced stress on sealed roadside enclosures in 45–50°C
GCC ambient conditions. However, this advantage cannot be claimed
without formal certification. Extended temperature and IP54+
certification are non-negotiable prerequisites for enterprise
infrastructure procurement — they are qualification criteria, not
differentiators.

---

## Dimension 4: Market Positioning & Proof

| Factor | NVIDIA Jetson incumbent | Axelera Metis platform | Gap type |
|---|---|---|---|
| Production deployments | Large-scale, documented | None yet | Critical client gap |
| Case studies published | Multiple | None | Critical client gap |
| SI relationships | Established | None | Critical client gap |
| ISV integrations | Hundreds | None | Critical client gap |
| Brand credibility | High | Zero | Critical client gap |

**Gap insight:** This is the most critical gap cluster. The client
has zero proof, zero relationships, and zero credibility in the
market at engagement start. The 18-month roadmap is specifically
designed to close this gap systematically — validation before proof,
proof before SI engagement, SI engagement before scale deployment.
Attempting to skip phases collapses the credibility pathway.

---

## Dimension 5: Product Positioning Clarity

| Factor | NVIDIA Jetson incumbent | Axelera Metis platform | Gap type |
|---|---|---|---|
| Target vertical clarity | Broad — all verticals | Broad — all verticals (pre-engagement) | Client gap |
| Workload-specific SKUs | Available | Not defined (pre-engagement) | Client gap |
| Deployment documentation | Extensive | None | Client gap |
| Reference architecture | Published | Not available | Client gap |
| TCO modelling tools | Available | Not available | Client gap |

**Gap insight:** Pre-engagement, the client was positioning the
product identically to the incumbent — *"works everywhere."* This
dilutes procurement clarity for ISVs and SIs who need workload-
specific assurance. The productisation framework recommendation
addresses this gap by defining deployment-layer SKUs on top of a
constant hardware platform, moving positioning from hardware-spec
to workload-defined.

---

## Gap Priority Matrix

| Gap | Severity | Closes by phase |
|---|---|---|
| No production deployments | Critical | Phase 3 |
| No ISV integrations | Critical | Phase 2 |
| No SI relationships | Critical | Phase 4 |
| Extended temperature certification missing | High | Phase 1 |
| IP54+ certification missing | High | Phase 1 |
| MTBF documentation missing | High | Phase 1 |
| Positioning too broad | High | Phase 1 |
| No workload-specific SKUs | High | Phase 1 |
| ISV migration friction | Medium | Phase 2 |
| No reference architecture | Medium | Phase 2 |
| No TCO modelling tools | Medium | Phase 3 |
