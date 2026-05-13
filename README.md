# CL103-EdgeAI-GCC-GoToMarket-Strategy

# Client (CL103) — Edge AI Go-To-Market Strategy
## Business Analysis & Strategic Consulting Engagement

**Analyst:** Ved Redkar | Co-Founder, Visionize Consultancy LLP
**Client:** Client (CL103) — Edge AI hardware venture, Dubai, UAE
**Engagement type:** BA & Strategic Consulting — Market Analysis,
Requirements Elicitation, Process Mapping, Business Case Development
**Timeline:** 2025
**Stakeholder:** Founder & CEO — Ex South Asia Director,
Korean AI MNC. C-suite, highly technical, fully remote engagement.

> Note: Financial modelling figures have been redacted from this
> repository at the client's commercial sensitivity level. Frameworks,
> methodologies, and process artefacts are published in full.

---

## Project Summary

Client had developed an Edge AI compute box powered by the Axelera
Metis accelerator, targeting GCC smart city infrastructure deployments.
The founder had deep technical expertise but no structured go-to-market
strategy, no market validation framework, and no clear product
positioning relative to the incumbent NVIDIA Jetson-class platform.

This engagement involved conducting senior stakeholder elicitation in a
single remote session, synthesising global and regional Edge AI market
intelligence, performing competitive gap analysis, defining functional
and non-functional requirements for the product positioning, and
delivering an 18-page strategic business case with a phased 18-month
go-to-market roadmap.

**Outcome:** 18-page strategic document delivered covering market
analysis, competitive positioning, productisation framework, and phased
go-to-market roadmap with feasibility-gated phases.

---

## Problem Statement

Client faced three interconnected problems:

**1. Positioning ambiguity** — The product was marketed as a generic
compute box applicable to retail, logistics, surveillance, and robotics.
This breadth diluted clarity for ISVs and SIs who needed deployment-
specific assurance before adoption.

**2. No validation proof** — Without structured pilot engagements,
benchmark data, or published case studies, the founder had no evidence
to present to enterprise buyers. In infrastructure procurement, proof
precedes purchase.

**3. No structured go-to-market** — The founder was approaching the
market without a sequenced strategy. In a market reshuffling rapidly
around power efficiency and deployment economics, an unstructured
approach risked losing the credibility window before it opened.

**Root cause:** The product existed at the hardware layer but had no
deployment intelligence, no market-validated positioning, and no
structured pathway from concept to production deployment.

---

## My Role

- **Business Analyst & Strategic Consultant**
- Conducted single-session C-suite elicitation — extracted full project
  scope from one remote video call
- Performed independent market research across GCC Edge AI landscape
- Produced competitive gap analysis — incumbent vs Axelera architecture
- Defined functional and non-functional requirements for product SKUs
- Designed 5-phase go-to-market roadmap with feasibility gate conditions
- Developed productisation framework — hardware layer vs deployment layer
- Produced 18-page strategic business case for founder decision-making

---

## 🛠️ BA Techniques Applied

| Technique | Application |
|---|---|
| Requirements elicitation | Single C-suite remote session — structured questions to extract full scope |
| Functional requirements | Defined what each deployment SKU must do — stream capacity, pipeline support, use case coverage |
| Non-functional requirements | Defined how it must perform — thermal certification, IP rating, MTBF, power envelope, lifecycle warranty |
| As-Is process mapping | Mapped current unstructured go-to-market — no ICP, no validation, no proof |
| To-Be process design | Designed structured 5-phase roadmap with gate conditions |
| BPMN process modelling | As-Is and To-Be diagrams produced |
| Gap analysis | Competitive gap mapped across 5 dimensions vs NVIDIA Jetson incumbent |
| MoSCoW prioritisation | All strategic requirements prioritised — Must/Should/Could/Won't |
| Business case development | 18-page document structured as problem → options → recommendation → benefits → risks |
| Feasibility assessment | Gate conditions defined between each phase — technical and commercial feasibility |
| Requirements traceability | Every strategic requirement traced to core objective — defensible market foothold in 18 months |
| Change impact assessment | NVIDIA → Axelera migration impact analysed for ISVs — engineering cost, CUDA dependency, ONNX portability |
| Stakeholder management | Single C-suite stakeholder, remote, time-scarce — adapted communication style accordingly |

---

## Tools Used

| Tool | Purpose |
|---|---|
| Draw.io | BPMN As-Is and To-Be process diagrams |
| Excel | TCO financial modelling (figures redacted) |
| MS Office | Strategic document production |
| Web research | GCC Edge AI market intelligence synthesis |

---

## Requirements Overview

### Functional Requirements
What each deployment SKU must do:

| FR ID | Requirement | Priority |
|---|---|---|
| FR-001 | Support minimum 8 simultaneous IP camera streams (Traffic SKU) | Must Have |
| FR-002 | Run ANPR pipeline validated and benchmarked | Must Have |
| FR-003 | Support ONNX model format for ISV cross-platform portability | Must Have |
| FR-004 | Provide SDK integration support documentation for ISV onboarding | Must Have |
| FR-005 | Deliver workload-specific benchmark sheet per SKU | Should Have |
| FR-006 | Support co-branded case study publication with ISV partner | Should Have |
| FR-007 | Enable MOU or RFP participation structure with SI partner | Should Have |
| FR-008 | Publish 2 public production case studies by month 18 | Could Have |

### Non-Functional Requirements
How it must perform:

| NFR ID | Requirement | Category | Priority |
|---|---|---|---|
| NFR-001 | Sustained operation at 50°C ambient temperature — certified | Reliability | Must Have |
| NFR-002 | IP54+ certification — validated not claimed | Compliance | Must Have |
| NFR-003 | MTBF documentation published | Reliability | Must Have |
| NFR-004 | Power draw within defined envelope under sustained inference | Performance | Must Have |
| NFR-005 | Lifecycle warranty programme defined and published | Reliability | Should Have |
| NFR-006 | Thermal stress test documentation available to ISV/SI | Reliability | Should Have |
| NFR-007 | Deployment timelines reduced vs GPU-heavy workflows | Performance | Should Have |

---

## Competitive Gap Analysis

Full analysis → [`/artefacts/gap-analysis.md`](./artefacts/gap-analysis.md)

### Summary — Axelera vs NVIDIA Jetson-class

| Dimension | NVIDIA Jetson incumbent | Axelera Metis alternative | Gap |
|---|---|---|---|
| Power consumption | Higher sustained wattage | Lower sustained wattage | Structural advantage at scale |
| Ecosystem | CUDA — strong, creates lock-in | ONNX-based — portable | Lower switching friction |
| Thermal management | Higher heat generation | Lower heat generation | Cabinet design simplification |
| UPS requirement | Larger capacity needed | Smaller capacity sufficient | Infrastructure cost reduction |
| Flexibility | Multi-model, multi-framework | Fixed-function optimised | Trade-off — lower breadth, higher efficiency |
| Market positioning | Dominant — pilots to infrastructure | Challenger — no production proof yet | Proof gap must be closed first |

---

## MoSCoW Prioritisation

Full table → [`/artefacts/moscow-prioritisation.md`](./artefacts/moscow-prioritisation.md)

| Priority | Strategic Requirement |
|---|---|
| Must Have | Define workload-validated SKUs — Traffic, Surveillance, Smart Parking |
| Must Have | Build internal benchmarking capability before external engagement |
| Must Have | Achieve 2 signed technical validation engagements by month 6 |
| Should Have | Co-author technical whitepaper with ISV partner by month 9 |
| Should Have | Structured SI collaboration — MOU or RFP participation by month 12 |
| Could Have | GITEX presence with validated deployment story by month 18 |
| Won't Have | Broad marketing campaign before deployment proof exists |

---

## Process Diagrams (BPMN)

### As-Is — Unstructured Go-To-Market
Pre-engagement: hardware-spec positioning, no ICP, no validation
data, stalled pipeline.

![As-Is BPMN](./artefacts/diagrams/asis-bpmn.png)

### To-Be — Structured 5-Phase Roadmap
Post-engagement: phased go-to-market with feasibility gates,
ISV-first validation, SI engagement only after proof exists.

![To-Be BPMN](./artefacts/diagrams/tobe-roadmap-bpmn.png)

Full written process descriptions →
[`/artefacts/asis-tobe-process.md`](./artefacts/asis-tobe-process.md)

---

## 5-Phase Go-To-Market Roadmap

| Phase | Timeline | Objective | Gate condition |
|---|---|---|---|
| Phase 1 — Internal readiness | Months 0–3 | Define SKU, benchmark capability, master SDK, narrow use cases | Clear product definition + benchmark sheet before any external conversation |
| Phase 2 — ISV validation | Months 3–6 | Approach filtered ISVs, structured 60-day technical validation engagement | 2 signed technical validation engagements |
| Phase 3 — Proof generation | Months 6–9 | Complete deployments, generate performance data, co-author whitepaper | Measurable publishable data before SI conversations |
| Phase 4 — SI engagement | Months 9–12 | Approach regional SIs with validated TCO modelling and RFP positioning | One structured SI collaboration — MOU or RFP participation |
| Phase 5 — Scale deployment | Months 12–18 | Target production deployment, publish case studies, GITEX with validated story | Two public case studies published |

---

## Productisation Framework

### The Core Insight
The product was being positioned as a generic compute box —
*"works everywhere."* This diluted clarity for buyers.

The BA recommendation was to separate two distinct layers:

**Hardware layer** — constant across all verticals
- CPU, accelerator, RAM, storage, cooling, OS
- Never changes per customer — manufacturing simplicity

**Deployment layer** — workload-specific packaging
- Configuration validated for specific use case
- Performance envelope defined and benchmarked
- Thermal certification documented
- Reference architecture provided
- Support package attached

### Deployment SKU Examples

| SKU | Configuration | Validated for |
|---|---|---|
| Traffic SKU | 8 stream optimised | ANPR, vehicle detection, traffic analytics |
| Surveillance SKU | 6 stream optimised | Perimeter detection, night vision, people counting |
| Smart Parking SKU | 4 stream, low-power mode | Bay detection, LPR, occupancy analytics |

### Why This Builds Moat
Anyone can copy hardware specs. Few will invest in workload
validation, thermal certification, reference architecture
documentation, and structured integration support. The deployment
layer becomes defensible knowledge — not a marketing exercise.

Full productisation framework →
[`/artefacts/business-case-summary.md`](./artefacts/business-case-summary.md)

---

## Outcome & Impact

| Deliverable | Detail |
|---|---|
| Strategic document | 18-page research and go-to-market framework delivered |
| Competitive gap analysis | 5-dimension framework — Axelera vs NVIDIA incumbent |
| MoSCoW requirements | 7 strategic requirements prioritised |
| Go-to-market roadmap | 5-phase, 18-month, feasibility-gated |
| Productisation framework | Hardware layer vs deployment layer model |
| Business case | Structured for C-suite decision making |
| Post-delivery | Client lost touch — outcome unverified |

**Honest reflection:** The absence of a follow-up feedback loop is a
documented lesson from this engagement. A structured review session
2 weeks post-delivery should have been proposed and agreed upfront.
This practice has been applied to all subsequent engagements.

---

## 📁 Repository Structure
