# LM AI Strategy Reference

**Purpose:** Strategic context for the Weekly AI Roundup — use this for scale calibration, competitive framing, and grounding RMS Relevance sections in real LM AI programs. Not for external publication; sourced from public LM disclosures.

---

## AI Factory — What It Actually Is

The AI Factory is a **secure, reusable platform** inside the Lockheed Martin AI Center (LAIC) for training, validating, deploying, and sustaining AI systems across enterprise, engineering, and mission use cases. It is not a marketing label. Think of it as LM's internal answer to the question every large enterprise faces: how do you go from pilot to production at scale, in classified environments, with DoD-grade assurance requirements?

**Three jobs it does simultaneously:**

1. **Internal productivity engine** — Standardizes AI development, centralizes scarce compute, automates pipelines. The backbone of 1LMX business transformation and engineering modernization.
2. **Mission-enablement layer** — Supports edge ISR, autonomy, cyber, sustainment, and C2 applications on fielded and future defense systems.
3. **Commercialization platform** — Through Astris AI (launched Dec. 2024), LM is now packaging the AI Factory stack as a product for government and regulated-industry buyers.

**Why the integration layer matters more than the models:** LM's moat is not model ownership — it's controlling the data access, security approvals, reusable pipelines, edge deployment, and authority to embed AI into existing certified defense programs. That's what makes the AI Factory strategically durable.

---

## Key Metrics (Use for Scale Calibration)

These are disclosed figures from public LM sources and partner case studies. Note that user-count figures measure different populations at different points in time — treat directional trends as robust, exact numbers as scope-dependent.

| Metric | Figure | Source context |
|--------|--------|---------------|
| On-prem token processing | 1B+ tokens/week | NVIDIA case study, 2025 |
| Automated pipelines | Thousands | NVIDIA case study, 2025 |
| Weekly API requests | Millions | NVIDIA case study, 2025 |
| Models consolidated on-prem | 30+ | NVIDIA case study, 2025 |
| Engineers/devs on AI Factory | ~7,000 | NVIDIA case study; IBM reported 10,000+ separately |
| LM employees using AI tools broadly | 50,000+ developers, engineers, scientists | LM 2024 annual report |
| LMText Navigator users | ~75,000 employees | Astris-facing materials, 2025 |
| Training time improvement | Weeks → Days | NVIDIA case study |
| Environment spin-up time | Weeks → Minutes | NVIDIA case study |
| Data/HR QA accuracy improvement | 45.45% → 66.0% | IBM case study (prompt eng + query optimization) |
| Data tools consolidated | 46 systems → 1 platform | IBM case study |
| R&D investment (2024) | $3B+ in R&D and capex | LM disclosure, early 2025 |
| IRAD (2025) | $2.0B | LM 2025 results |
| Capex (2025) | $1.6B | LM 2025 results |
| Revenue (2025) | ~$74.7B total | Public financials — use for competitor investment comparisons |
| U.S. government revenue (2025) | ~$53.4B | LM 2025 |
| International revenue (2025) | ~$21.3B | LM 2025 |
| Fixed-price contracts (approx.) | ~60% of 2025 sales | LM 2025 — means AI productivity gains directly protect margins |

---

## Technology Stack

| Layer | What's Running | Why It Matters |
|-------|---------------|----------------|
| Compute | NVIDIA DGX SuperPOD (on-prem) | Keeps sensitive data local; avoids public-cloud token cost at scale |
| Model serving | Triton Inference Server, NVIDIA AI Enterprise | Production-grade inference with monitoring |
| Container/orchestration | Red Hat OpenShift, MicroShift, Device Edge, KServe, Ray clusters | Cloud-native patterns on classified and edge hardware |
| Models | IBM Granite, Meta open-source LLMs, Google Gemini | Model plurality — avoids lock-in to any single supplier |
| Data layer | Integrated enterprise platform (replaced 46 tools); mission sensor data | Foundation for RAG, analytics, copilots |
| Cloud/classified | Azure Government Secret (Microsoft); Google Cloud/Vertex AI incl. air-gapped | Hybrid: classified on-prem + cloud burst for non-classified |
| Edge | Red Hat Device Edge, low-SWaP hardware (Stalker UAS demonstrated) | AI inference pushed into field environments |
| Governance/security | Traceability, explainability, monitoring, data governance, AI ethics training | The assurance posture that makes this deployable in DoD programs |

---

## Key Partnerships

| Partner | Role | Strategic Implication |
|---------|------|-----------------------|
| NVIDIA | DGX SuperPOD, Triton, NeMo, CUDA, AI Enterprise | Core on-prem compute; faster training; avoids public-cloud exposure |
| IBM | Granite LLMs, watsonx data/governance/orchestration | Enterprise data unification, model choice, agentic internal tools |
| Red Hat | Device Edge, MicroShift, OpenShift | Edge-Kubernetes path into military platforms |
| Microsoft | Azure Government Secret, classified cloud, 1LMX digital foundation | Classified cloud operations and enterprise transformation backbone |
| Google Cloud | Vertex AI, Gemini, Google Distributed Cloud (air-gapped capable) | Foundation-model expansion in secure national-security settings |
| Meta | Open-source LLMs in AI Factory | Open-model optionality; reduces dependence on proprietary suppliers |
| Oracle | Astris AI for Government on OCI | External commercialization of the AI Factory stack |

---

## Astris AI — The Commercialization Arm

Launched December 2024. LM is packaging the AI Factory's high-assurance AI infrastructure, MLOps, and engineering services for external buyers — government agencies and similarly regulated industries. Key positioning:

- No vendor lock-in (explicitly marketed)
- Cloud-to-edge deployment without moving sensitive data off network
- Full-stack: reduces procurement fragmentation for risk-averse government buyers
- Available on Oracle Cloud Infrastructure and Oracle Marketplace
- Late 2025: Astris AI for Government announced with Oracle, NVIDIA, and Meta

**Why it matters for the roundup:** When external stories cover enterprise AI platform consolidation, commercial AI infrastructure, or government AI procurement, Astris is the RMS hook. LM is no longer just a buyer of AI infrastructure — it's becoming a seller.

---

## Organizational Context (AI Leadership)

- **Mike Baylor** — Chief Digital and AI Officer
- **Greg Forrest** — VP, AI Foundations / Director of AI Foundations (leads LAIC engineers supporting Astris AI)
- **John Clark** — SVP, Technology & Strategic Innovation (AI Factory partnerships connect through this function)
- **Maria Demaree** — 1LMX transformation lead (enterprise integration of AI Factory)

**Governance:** AI Ethics Executive Steering Committee, with an AI Ethics Subcommittee (meets monthly, reports quarterly). Includes all BAs plus legal, ethics, HR, comms, and business transformation. 100% of AI developers trained in systems-engineering approaches to AI ethics. Aligned to DoD's five responsible AI principles (Responsible, Equitable, Traceable, Reliable, Governable).

---

## Competitive Landscape

### The Core Tension
LM competes against traditional primes, AI-native defense software firms, and hyperscale ecosystems simultaneously. Its advantage is not model quality — it's the integration layer: classified data access, security approvals, certified platform embeddability, and reusable production pipelines. That's harder to replicate than building a good model.

### Competitor Map

| Competitor | AI Posture | Overlap with LM | Assessment |
|------------|-----------|-----------------|------------|
| Northrop Grumman | Mission AI, autonomy, C2, AI ethics | Strong — mission AI, platform integration | Closest traditional-prime analogue |
| RTX / Raytheon | Sensors, radar, embedded AI, collaborative autonomy, safety-critical AI | Strong — sensing, mission systems, embedded AI | Strong technical competitor especially in sensing |
| Boeing | Enterprise AI, defense logistics, onboard AI for space, Palantir partnership for classified work | Moderate — aerospace engineering, enterprise modernization | Less centralized than AI Factory; still major platform access |
| **Palantir** | AIP for Defense, Gotham, CJADC2/decision software | High — C2, analytics, AI orchestration, sensitive environments | Fast software cycles; substitute AND partner competitor |
| **Anduril** | Lattice for Mission Autonomy, counter-UAS, edge AI, partner ecosystem | High — autonomy, edge AI, mission C2 | **Most important AI-native disruptor in autonomy and software-defined mission systems** |

**Palantir and Anduril are the ones worth watching most closely.** Their software-development velocity is higher; LM's moat is integration depth and mission-data access, not speed.

---

## Key Risk Factors (from LM's 10-K)

Use when stories touch AI risk, enterprise AI adoption hesitation, or compliance pressure:

- **Supplier concentration:** NVIDIA-class GPU availability, semiconductor shortages, and sole/single-source exposure can shape AI Factory cost and timeline
- **Cleared talent:** Fierce competition for AI-skilled personnel with security clearances — a real constraint on how fast LM can scale
- **Buyer power:** ~72% of 2025 revenue from U.S. government; buyers can dictate security, interoperability, data-rights, and price/performance terms
- **Fixed-price exposure:** ~60% of sales are fixed-price; AI productivity failures hit margins directly
- **Compliance tightening:** CMMC final rule published Oct. 2024; phased implementation began Nov. 2025. For Astris AI selling into the defense industrial base, cyber maturity is product-market fit
- **Export controls on compute:** U.S. BIS controls on advanced AI chips tightened in 2025-2026. Compute is a policy-constrained input in defense AI, not just a cost input
- **IP/data-rights exposure:** Government contracts can let DoD obtain and authorize use of technical data developed under contract — an AI training-data risk
- **AI-enabled adversaries:** The 10-K explicitly flags cyber threats that include AI-enabled adversary behavior

---

## Business Strategy Frame — For the Strategic Picture

When writing the Strategic Picture, these are the through-lines that hold:

**Integration layer > model ownership.** LM's AI economics hinge on controlling data access, security approvals, reusable pipelines, edge deployment, and embeddability in existing programs — not on owning the best model. This is why the AI Factory is more valuable than any single partnership announcement.

**Fixed-price math.** Roughly 60% of LM's revenue is fixed-price. Every story about AI-driven productivity, schedule compression, or reduced engineering rework connects directly to margin protection on current programs — not a future aspiration.

**Platform before product.** AI Factory → 1LMX → Astris AI is a logical sequence: standardize internally, use it to improve programs, then sell the platform externally. When external stories cover this same arc at other companies, LM is ahead of most.

**Compute is policy.** Export controls on advanced AI chips are tightening. For a company selling AI systems to allied governments, this is an operational constraint, not background noise.

**The classified moat.** LM's expertise in compartmentalization and classified environments is a genuine advantage in a moment when enterprises are anxious about data governance. It's not just a constraint — it's credibility.
