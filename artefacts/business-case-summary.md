# Business Case Summary & Productisation Framework
**Project:** GCC Edge AI Go-To-Market Strategy
**Client:** Dubai-based Edge AI hardware venture (anonymised)
**BA:** Ved Redkar | Visionize Consultancy LLP
**Version:** 1.0

---

## Business Case Overview

### Problem
The client had developed a technically capable Edge AI compute platform
with a genuine structural advantage in power efficiency and thermal
performance vs the NVIDIA Jetson-class incumbent. However, zero market
proof, zero ISV integrations, zero SI relationships, and unclear
product positioning meant the advantage was commercially invisible.

### Objective
Achieve a defensible market foothold in GCC smart city infrastructure
within 18 months, starting from zero brand equity.

### Options Considered

**Option 1: Broad market approach (status quo)**
Continue approaching all verticals simultaneously with hardware-spec
positioning. No structural change to go-to-market.
*Assessment:* High risk. Diluted focus, no proof generation pathway,
competing against established incumbents on their strongest ground.
Rejected.

**Option 2: Vertical focus with phased validation**
Narrow to 2–3 vision-centric, infrastructure-heavy verticals. Build
proof through structured ISV validation before SI engagement. Gate
each phase on tangible evidence.
*Assessment:* Higher effort in Phase 1 but structurally sound.
Creates a defensible proof pathway and positions the client as an
infrastructure solution rather than a hardware vendor. Recommended.

**Option 3: Direct end-customer sales**
Bypass ISV and SI pathway and approach end customers directly.
*Assessment:* Infrastructure procurement at scale goes through SIs.
Direct sales bypass the procurement pathway and are not viable at
the client's current credibility level. Rejected.

### Recommended Option
Option 2 — vertical focus with phased validation.

---

## Benefits Realisation

### Quantified benefits
- Energy cost reduction at scale vs NVIDIA incumbent
  (specific figures redacted — commercially sensitive)
- UPS capacity reduction at scale
  (specific figures redacted)
- Cabinet density improvement
  (specific figures redacted)

### Structural benefits (not directly quantified)
- Thermal simplification — smaller fans, reduced ventilation,
  less stress on sealed roadside cabinets in 45–50°C conditions
- Reduced long-term hardware degradation — lower sustained wattage
  means lower thermal stress on components over 5-year lifecycle
- Lower ISV switching friction — ONNX portability vs CUDA lock-in
- Deployment intelligence moat — workload validation and reference
  architecture documentation are defensible knowledge assets

---

## Risk Register

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| NVIDIA reduces power consumption or adjusts pricing | Medium | High | Accelerate deployment-layer differentiation — move from box supplier to infrastructure solution component |
| ISV migration friction higher than expected | Medium | High | Absorb engineering cost during 60-day validation — reduce barrier to entry |
| Certification timelines extend beyond Phase 1 | Medium | Medium | Initiate certification process at month 0 — do not wait until Phase 1 completion |
| SI conversations premature — damage credibility | Low | High | Gate conditions enforced — SI engagement does not begin until proof exists |
| Market reshuffles rapidly — new entrants | Medium | Medium | Deployment-layer differentiation builds moat — harder to replicate than hardware specs |
| Founder bandwidth — solo execution | High | High | Phase 1 is internal only — no external commitments until readiness confirmed |

---

## Productisation Framework

### The Core Problem with Generic Positioning
Pre-engagement, the product was positioned as:
*"High-performance edge AI compute for retail, logistics,
surveillance, and robotics."*

This positioning has two structural problems:

1. **Dilutes procurement clarity** — ISVs and SIs cannot evaluate
   a product against their specific workload requirements without
   workload-specific validation data.

2. **Vulnerable to market shuffle** — if positioned purely as an
   alternative hardware vendor, any NVIDIA pricing or performance
   adjustment makes the product replaceable.

---

### The Two-Layer Model

The recommended productisation framework separates the product into
two distinct layers:

#### Hardware Layer — constant across all verticals
- CPU (RK3588)
- Axelera Metis accelerator
- RAM and storage configuration
- Power input and management
- Cooling system
- Network ports
- Operating system (Ubuntu)

This layer never changes per customer. Manufacturing remains simple,
inventory remains manageable, support scales cleanly.

#### Deployment Layer — workload-specific packaging
- Workload configuration validated for specific use case
- Performance envelope defined and benchmarked
- Thermal certification documented for deployment environment
- Reference architecture provided per vertical
- Integration support package defined
- Lifecycle warranty terms specified

---

### Deployment SKU Definitions

#### Traffic SKU
| Attribute | Specification |
|---|---|
| Stream capacity | 8 IP cameras simultaneous |
| Primary workload | ANPR, vehicle detection, traffic analytics |
| Benchmark validated | FPS, latency, power draw at 45°C |
| Reference architecture | Roadside cabinet deployment diagram |
| Thermal certification | 50°C sustained — documented |
| Target buyer | Traffic management ISVs, municipal SIs |

#### Surveillance SKU
| Attribute | Specification |
|---|---|
| Stream capacity | 6 IP cameras optimised |
| Primary workload | Perimeter detection, people counting, night vision |
| Benchmark validated | FPS, accuracy, latency at rated ambient |
| Reference architecture | Fixed-installation deployment diagram |
| Target buyer | Security ISVs, public safety SIs |

#### Smart Parking SKU
| Attribute | Specification |
|---|---|
| Stream capacity | 4 streams, low-power mode optimised |
| Primary workload | Bay detection, LPR, occupancy analytics |
| Power configuration | Optimised for smaller UPS — extended battery backup |
| Reference architecture | Parking structure deployment diagram |
| Target buyer | Smart city ISVs, parking infrastructure SIs |

---

### Why Deployment-Layer Differentiation Builds Moat

Anyone can copy hardware specifications. Procurement teams can read
a datasheet. Few will invest in:

- Workload validation across target use cases
- Real deployment benchmarking at rated ambient conditions
- Thermal certification documentation
- Reference architecture per vertical
- Structured ISV integration support
- Published case material from production deployments

The deployment layer becomes defensible knowledge. It embeds the
client deeper in the value chain — moving from *box supplier* to
*infrastructure solution component*. That is structurally harder
to replace than a competitive hardware specification.

---

### Analogy: Automotive Platform Strategy
The same engine platform powers a police vehicle, an ambulance,
and a taxi fleet. The engine is constant. The configuration,
validation, certification, and deployment documentation differ
per application.

The client's hardware is the engine. The deployment SKUs are
the application-specific configurations built on top of it.

---

## Lessons Learned

**Lesson 1: Propose a structured review session upfront.**
The engagement ended at document delivery with no formal feedback
loop. A structured 2-week post-delivery review should have been
proposed and agreed during the initial elicitation session. This
practice has been applied to all subsequent engagements.

**Lesson 2: Single-session elicitation requires rigorous preparation.**
With only one stakeholder session available, elicitation questions
had to be structured to surface assumptions, constraints, priorities,
and success criteria simultaneously. A pre-session hypothesis
framework — prepared before the call — maximised extraction from
limited stakeholder time.

**Lesson 3: Intellectual honesty builds credibility with senior
stakeholders.**
The document explicitly acknowledged that the strategy assumed zero
market credibility and that the founder's existing relationships
could compress the timeline significantly. Framing recommendations
as structured hypotheses rather than confident prescriptions was
appropriate given the single-session elicitation constraint and the
founder's superior domain knowledge.
