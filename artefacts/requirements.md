# Functional & Non-Functional Requirements
**Project:** GCC Edge AI Go-To-Market Strategy
**Client:** Dubai-based Edge AI hardware venture (anonymised)
**BA:** Ved Redkar | Visionize Consultancy LLP
**Version:** 1.0

---

## Context
Requirements were elicited during a single structured remote session
with the founder and CEO. Given the time-scarce nature of C-suite
engagement, requirements were extracted through targeted elicitation
questions and validated against the strategic document delivered
post-session.

Requirements are split into two categories:
- Functional requirements — what each deployment SKU must do
- Non-functional requirements — how the system must perform

---

## Functional Requirements

### FR-001: Traffic SKU — Stream Capacity
**Requirement:** The Traffic SKU must support a minimum of 8
simultaneous IP camera streams under sustained inference load.
**Rationale:** GCC traffic deployments typically involve 6–10 camera
feeds per roadside cabinet. 8 streams represents the minimum viable
deployment configuration for this vertical.
**Priority:** Must Have
**Acceptance criteria:** Benchmark sheet demonstrates sustained 8-stream
inference at defined FPS without thermal throttling under 45°C ambient.

---

### FR-002: ANPR Pipeline Validation
**Requirement:** The Traffic SKU must have an ANPR (Automatic Number
Plate Recognition) pipeline validated and benchmarked on the Axelera
Metis accelerator.
**Rationale:** ANPR is the primary fixed-function workload for traffic
infrastructure deployments in the GCC. Validation is a prerequisite
for ISV and SI adoption conversations.
**Priority:** Must Have
**Acceptance criteria:** Validated FPS, accuracy rate, and latency
figures documented in benchmark sheet. Results reproducible by ISV
partner during technical validation engagement.

---

### FR-003: ONNX Model Format Support
**Requirement:** The platform must support ONNX as the primary model
interchange format for cross-platform portability.
**Rationale:** ONNX has become the dominant interoperability layer for
cross-platform model portability. ISVs optimised around CUDA stacks
require ONNX support to reduce migration friction and engineering cost.
**Priority:** Must Have
**Acceptance criteria:** ISV can convert and deploy an existing ONNX
model without custom SDK modifications within the 60-day technical
validation engagement.

---

### FR-004: ISV SDK Integration Documentation
**Requirement:** Comprehensive SDK integration documentation must be
available for ISV onboarding, covering model conversion, pipeline
configuration, and deployment validation.
**Rationale:** Engineering time is the primary barrier to ISV adoption.
Reducing integration friction through documentation directly lowers
switching resistance and accelerates time-to-pilot.
**Priority:** Must Have
**Acceptance criteria:** ISV engineering team can complete initial
integration without direct engineering support from the client within
defined timeframe.

---

### FR-005: Workload-Specific Benchmark Sheet
**Requirement:** Each deployment SKU must have a published benchmark
sheet defining stream capacity, FPS, latency, power draw, and thermal
behaviour under sustained load.
**Rationale:** Enterprise infrastructure buyers require quantified
performance data before procurement. Generic specifications do not
satisfy SI or ISV technical validation requirements.
**Priority:** Must Have
**Acceptance criteria:** Benchmark sheet covers all defined metrics,
tested at rated ambient temperature, results independently reproducible.

---

### FR-006: ISV Co-Branded Case Material
**Requirement:** Following successful technical validation, the client
must produce co-branded case material with the ISV partner documenting
deployment results.
**Rationale:** Press without validation is noise. Co-branded case
material provides credibility signal to subsequent ISV and SI prospects,
reducing adoption risk in the sales cycle.
**Priority:** Should Have
**Acceptance criteria:** At least one co-authored technical whitepaper
or case study published by month 9 of the roadmap.

---

### FR-007: SI Collaboration Structure
**Requirement:** The client must establish a structured collaboration
with at least one regional SI — either an MOU or participation in a
smaller RFP — by month 12 of the roadmap.
**Rationale:** SIs control the procurement pathway for large-scale GCC
infrastructure deployments. Without SI relationships, the client cannot
access the 50–150 node deployment tier that represents the target
commercial outcome.
**Priority:** Should Have
**Acceptance criteria:** Signed MOU or confirmed RFP participation with
a regional SI operating in traffic, public safety, or parking
infrastructure verticals.

---

### FR-008: Public Case Studies
**Requirement:** Two public production case studies must be published
by month 18 of the roadmap.
**Rationale:** GITEX attendance without validated deployment story is
noise. Case studies provide the credibility foundation for press
releases, conference presence, and subsequent enterprise conversations.
**Priority:** Could Have
**Acceptance criteria:** Two case studies published, covering different
deployment verticals, with quantified performance and efficiency data.

---

## Non-Functional Requirements

### NFR-001: Extended Temperature Certification
**Requirement:** The hardware platform must be certified for sustained
operation at 50°C ambient temperature.
**Category:** Reliability
**Rationale:** GCC outdoor deployments — roadside cabinets, parking
infrastructure, traffic gantries — regularly reach 45–50°C sustained
ambient in summer months. Uncertified hardware creates operational and
commercial risk for SI and ISV partners.
**Priority:** Must Have
**Acceptance criteria:** Thermal stress test documentation showing
sustained operation at 50°C for defined duration without performance
degradation or failure. Certification must be independently verified,
not self-claimed.

---

### NFR-002: IP54+ Ingress Protection Certification
**Requirement:** The hardware platform must carry IP54+ certification
for dust and water ingress protection.
**Category:** Compliance
**Rationale:** Roadside and outdoor deployments in the GCC expose
hardware to dust, sand, and occasional water ingress. IP54+ is the
minimum acceptable standard for enterprise infrastructure procurement.
**Priority:** Must Have
**Acceptance criteria:** Valid IP54+ certification from recognised
testing body. Certification documentation available to ISV and SI
partners on request.

---

### NFR-003: MTBF Documentation
**Requirement:** Mean Time Between Failures documentation must be
published for the hardware platform.
**Category:** Reliability
**Rationale:** Infrastructure-grade procurement requires reliability
data. SIs and enterprise buyers use MTBF figures to model total cost
of ownership and maintenance scheduling over a 5-year deployment
lifecycle.
**Priority:** Must Have
**Acceptance criteria:** MTBF figure calculated from accelerated life
testing or field data, documented and available in product
specification sheet.

---

### NFR-004: Power Draw Envelope
**Requirement:** Sustained inference power draw must remain within the
defined envelope under full workload at rated ambient temperature.
**Category:** Performance
**Rationale:** Power efficiency is the primary structural advantage
of the Axelera Metis architecture vs NVIDIA Jetson-class incumbent.
The efficiency advantage compounds significantly at scale across
distributed deployments — lower power draw reduces energy cost, UPS
capacity requirements, thermal management complexity, and cabinet
density requirements.
**Priority:** Must Have
**Acceptance criteria:** Sustained power draw measured under full
workload at 45°C ambient. Results documented in benchmark sheet.
Figures used in TCO modelling for SI engagement.
**Note:** Specific wattage figures redacted — commercially sensitive.

---

### NFR-005: Lifecycle Warranty Programme
**Requirement:** A defined lifecycle warranty programme must be
established and published before SI engagement conversations begin.
**Category:** Reliability
**Rationale:** Infrastructure deployments operate over 5-year cycles.
SIs require warranty coverage assurance before recommending hardware
to public sector clients. Absence of a formal warranty programme is
a disqualifying factor in enterprise procurement.
**Priority:** Should Have
**Acceptance criteria:** Warranty terms documented covering hardware
failure, RMA process, and replacement timelines. Published in product
documentation before Phase 4 SI engagement.

---

### NFR-006: Thermal Stress Test Documentation
**Requirement:** Thermal stress test results must be available to ISV
and SI partners as part of the technical validation package.
**Category:** Reliability
**Rationale:** ISVs and SIs conducting technical due diligence will
request thermal performance data. Self-reported figures are
insufficient — test methodology and results must be documented.
**Priority:** Should Have
**Acceptance criteria:** Thermal stress test report covering sustained
load at rated ambient, peak temperature recorded, thermal throttling
threshold, and recovery behaviour.

---

### NFR-007: Deployment Timeline Reduction
**Requirement:** The platform and SDK must enable ISV deployment
timelines reduced vs traditional GPU-heavy workflow benchmarks.
**Category:** Performance
**Rationale:** Reducing ISV engineering burden is a core value
proposition alongside power efficiency. If integration complexity
negates the hardware advantage, adoption stalls regardless of
performance metrics.
**Priority:** Should Have
**Acceptance criteria:** ISV documents deployment timeline in co-
authored case material. Reduction vs prior GPU-based deployment
baseline quantified and published.
**Note:** Specific percentage targets redacted — commercially sensitive.
