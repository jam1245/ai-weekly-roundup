# AI Strategy Benchmarks & Patterns Reference

**Purpose:** Roundup-optimized synthesis of the AI Strategy Library (8 HBS case-based documents stored in `ai-strategy-library/`). Use this for scale calibration, Strategic Picture through-lines, competitor and peer comparisons, and grounding RMS Relevance sections in what enterprise AI actually looks like at other organizations.

Full source files are in `references/ai-strategy-library/` if deeper context is needed on any case.

---

## Company Benchmarks for Scale Calibration

Use when a roundup story involves investment figures, user counts, or revenue metrics that need grounding.

### Revenue & Growth
| Company | Metric | Figure | Date context |
|---------|--------|--------|-------------|
| OpenAI | ARR | $12B | Mid-2025 |
| Anthropic | ARR | $3B | Mid-2025; projecting $12–34.5B by 2027 |
| Adobe Digital Media | Revenue | $12.84B | FY2022, growing 10%+ YoY before GenAI |
| Adobe total | Revenue | $17.6B | FY2022 |
| Google | Search ad revenue per query | ~1.61 cents | Baseline |

### Burn Rates & Profitability Timelines
| Company | Annual Burn | Profitability |
|---------|------------|---------------|
| OpenAI | ~$8B (2025) | Expects cash-flow positive 2029 at $125B revenue |
| Anthropic | ~$3B (2025; compute alone $2.5B) | Best case breakeven 2027 |
| Google | Profitable overall | But AI threatens search advertising model |

**Key frame:** No major GenAI company is profitable yet. Plan for multi-year investment horizons. Use when stories cover AI company financials or enterprise ROI expectations.

### Valuations
| Company | Valuation | Revenue Multiple |
|---------|-----------|----------------|
| Anthropic | $183B (Sept. 2025) | ~61x ARR |
| OpenAI | Multi-hundred-billion implied | ~25x+ ARR |
| Adobe | ~$315B peak (Dec. 2021); ~50% decline by Dec. 2022 | — |

### Training Cost Trajectory (for compute/investment stories)
| Model | Reported Training Cost |
|-------|----------------------|
| Original Google Transformer | ~$900 |
| OpenAI ChatGPT (2022 alone) | $540M+ |
| Gemini 1.0 Ultra | ~$191M |
| DeepSeek R1 (claimed) | ~$6M (via MoE + distillation) |

**Key frame:** Training costs are escalating for frontier models, but architectural innovation (MoE, distillation) is proving that efficiency can close the gap at a fraction of the cost.

---

## Inference Economics (Use for AI Pricing & Infrastructure Stories)

| Metric | Figure |
|--------|--------|
| Traditional Google search cost | ~1.06 cents/query |
| Adding GenAI inference | ~+0.36 cents/query (basic) |
| Search ad revenue per query | ~1.61 cents |
| Inference cost decline rate | ~30% annually |
| Token pricing trajectory | ~$200/million tokens (GPT-4, mid-2023) → single digits by late 2024 |
| But: reasoning models increase tokens per query dramatically | Net cost trajectory uncertain |

**The tension:** Per-token costs are falling fast, but usage is growing faster. Especially with reasoning and agentic models, the net economics are still unsettled.

---

## Enterprise AI Adoption Data

Use when stories cover AI rollout pace, enterprise readiness, or the gap between pilot and production.

### Adoption Rates
- 25% of companies expected to pilot AI agents by end of 2025; doubling by 2027
- 90% of executives view agentic AI as potential competitive advantage
- Only 19% of organizations have made significant AI agent investments

### The Pilot-to-Production Gap
- **95% of enterprise GenAI pilots yielding zero return** (MIT, July 2025) — the single most useful stat for grounding AI hype stories
- 40% of agentic AI projects predicted to be cancelled by 2027 (Gartner)
- Only 3% of organizations trust AI agents for autonomous judgment calls
- 45% of business leaders cite data accuracy and bias as primary concern
- 86% of organizations need significant tech stack upgrades before agent deployment
- Successful agent deployments require 8+ integrated data sources

### Market Size
- Global AI agent market: $5.1B (2024) → $47.1B projected (2030)
- ChatGPT: 339M MAU (Jan. 2025), 700M WAU (Aug. 2025)
- OpenAI enterprise: 600K+ paying business customers

---

## Strategic Patterns — For the Strategic Picture

These are the recurring themes across all six cases. Use them to name the through-line in the Strategic Picture rather than just listing what happened.

### "Model is not the moat"
The most consistent finding across all cases. Adobe won with commercially safe training data and workflow integration, not frontier model scale. Moderna won through broad access and training. Salesforce won through trust and platform position. Google's own internal memo warned "we have no moat" despite inventing the Transformer.

**Roundup use:** When a story is about a company changing its model strategy, pricing, or partnerships — the question to pose is "which layer of the stack are they actually competing on?"

### "Platform thinking beats isolated pilots"
Moderna built shared digital infrastructure that scaled across use cases. Adobe embedded AI across its existing product suite rather than launching a standalone tool. Salesforce used its existing CRM platform as the agent foundation.

**Roundup use:** When a story is about an enterprise AI rollout — is the company building a platform or accumulating experiments? The ones building platforms compound; the ones accumulating pilots stall.

### "Trust is a strategic asset, not a compliance checkbox"
Salesforce weaponized trust to sell enterprise agents. Adobe's commercially safe training and content provenance turned values into competitive differentiation. Anthropic's safety-first approach won the DoD.

**Roundup use:** Directly maps to LM's classified-environment posture and AI Factory's assurance architecture. When a story involves AI safety, governance, or enterprise hesitancy.

### "Democratization requires layered governance"
Moderna's 1,400+ custom GPTs created energy but also duplication, hallucination risk, and governance gaps. The winning model: broad experimentation for low-risk work, formal review for regulated or consequential decisions.

**Three-tier governance frame:**
- Tier 1 (low risk): summarization, drafting, internal brainstorming — basic tool access + acceptable-use guidance
- Tier 2 (moderate risk): internal workflow copilots, policy interpretation, analytics — named owner, monitoring, periodic review
- Tier 3 (high risk): customer-facing agents, regulated content, safety/finance/legal decisions — formal review, human oversight, auditability

**Roundup use:** When stories cover enterprise AI governance, shadow AI, or the tension between enabling innovation and managing risk.

### "AI changes the operating model, not just productivity"
Salesforce made service leaders (not IT) accountable for digital labor performance. Adobe's adoption required cross-functional alignment across research, product, design, marketing, and strategy. Moderna's AI Academy became a mechanism for organizational change.

**Roundup use:** When stories cover AI workforce impacts — the question isn't "will AI replace jobs?" but "how is the organization restructuring work?"

### "The integration layer is the moat"
Value accrues to whoever controls data access, workflow integration, and deployment in specific high-value contexts — not to whoever owns the best model. This applies to Adobe (workflow integration), Salesforce (CRM data), Anthropic (safety reputation + enterprise positioning), and LM (classified data + platform embeddability).

---

## Company-Specific Reference Points

### Adobe
- **Core insight:** Built own model (Firefly) on 300M+ curated, royalty-free Stock images — no competitor can replicate this training data
- **Result:** IP indemnification for enterprise customers; legal defensibility in copyright litigation era
- **AI Ethics Board established 2019** — years before GenAI wave, not reactive
- **"Amplify, not replace"** framing since 2016
- **Stock declined ~50% (2021–2022)** despite record revenue — market initially misread the AI strategy
- **Embedded AI as "superpower" into existing products** rather than launching standalone — deepened subscriptions instead of cannibalizing them

### Google / Alphabet
- **93.4% global desktop search share** at case time
- **Invented the Transformer** but was blindsided by ChatGPT's consumer breakout
- **Internal memo: "We have no moat"** — warning even the inventor of GenAI couldn't assume model leadership
- **Google searches declined for the first time in 20 years** — triggering ~$250B market cap loss
- **Unit economics dilemma:** AI inference adds ~0.36 cents/query to a model that earns 1.61 cents/search in ads; at 5T+ annual searches, each incremental AI query is a margin risk
- **Invested $2.3B+ in Anthropic** as a strategic hedge while building own Gemini models
- **Custom silicon (Trillium TPUs)** to reduce NVIDIA dependency

### Anthropic
- **$3B ARR, $183B valuation** (mid-2025) — 61x revenue multiple
- **32% enterprise AI market share**, surpassing OpenAI in enterprise
- **42% code generation market share** — 2x OpenAI's share
- **$200M DoD prototype agreement** — safety positioning won classified/regulated work
- **Constitutional AI:** trains models on human-written principles refined by other models — scalable, auditable oversight
- **Had Claude ready before ChatGPT launched** but delayed for safety testing — lost consumer first-mover, recovered in enterprise
- **Multi-homing norm:** most Fortune 500 companies use 3–5+ model providers; no single model will dominate

### Moderna (Enterprise AI Scaling Case)
- **~6,000 employee company** competing with pharma rivals of 100,000+ — AI as force multiplier
- **1,400+ custom GPTs** built by employees after broad access was granted
- **AI Academy** turned training into organizational change, not just upskilling
- **Replaced 46 data/analytics/BI systems** with one integrated platform before scaling AI (parallels LM's AI Factory data consolidation)
- **Key insight:** AI success depended on digital groundwork laid years earlier — fragmented digital foundation = failed AI rollout

### Salesforce / Agentforce
- **"Customer Zero" strategy:** deployed agents internally in customer service before customer rollout — learn on real work
- **Repositioning:** from CRM/SaaS to competing in the labor market — AI shifted from software seats to "work performed"
- **Service leaders (not IT) made accountable** for digital labor performance — business owns AI outcomes
- **Best early agent use cases:** high-volume, structured, repetitive, low-emotion interactions with clear escalation logic
- **Pricing challenge:** outcome-based and capacity-based pricing being explored as seat-based subscriptions stop fitting AI value

### DeepSeek (Disruption Case)
- **Claimed training cost ~$6M** for near-frontier performance vs. hundreds of millions for competitors
- **Innovations:** Mixture of Experts (MoE), knowledge distillation, built on Meta's open-source PyTorch/LLaMA
- **Implication:** architectural innovation can close the performance gap at a fraction of the capital cost — the "you need a billion dollars to compete" assumption is challenged

---

## AI Talent Economics

Use when stories involve AI hiring, compensation, or talent competition.

| Metric | Figure |
|--------|--------|
| OpenAI median software engineer | $810K/year |
| San Francisco avg. software engineer | $220K/year |
| Meta AI researcher signing bonuses | Up to $100M (rumored) |
| Scale AI CEO acquisition (Meta) | $14.3B investment |

**Key finding across cases:** In the AI talent market, mission alignment, research culture, and compute access may matter as much as compensation. Talent rejected $100M Meta offers to join mission-driven companies (Anthropic). Talent retention is as strategic as acquisition.

**For LM context:** cleared AI talent is a compounding constraint — the talent pool is already smaller, and competition for cleared AI-capable engineers is intensifying.

---

## AI Agent Readiness Framework

Use when stories cover agentic AI, autonomous systems, or enterprise AI autonomy.

### Autonomy Levels
- **Level 1–2:** Fixed sequences or limited dynamic workflows; human-in-the-loop — where most production deployments actually live today
- **Level 3:** Partial autonomy — only experimental in most organizations
- **Level 4:** Full autonomy — theoretical

### What makes agent deployments succeed
Per Salesforce case: target work that is high-volume, structured, repetitive, low-emotion, with **clear escalation design**. Human handoff is not failure — it's a designed part of a trustworthy agent system.

### What makes them fail
- Overselling autonomy before reliability is proven
- Weak handoff to humans
- Missing the 8+ data source integrations required
- Trying to force old pricing/metrics onto new AI value

---

## Monetization Models & Dynamics

Use when stories cover AI pricing changes, subscription models, or vendor economics.

| Model | Example | Key tension |
|-------|---------|-------------|
| Usage/per-token | OpenAI API | Prices declining 30%+ annually; heavy users unprofitable |
| Tiered subscription | Anthropic ($17–$100/mo), Google ($249.99/mo Ultra) | Low conversion; Pareto problem (20% of users = 80% of cost) |
| Bundled into existing product | Adobe Creative Cloud | Absorbs inference cost; may not capture full willingness to pay |
| Enterprise licensing | Anthropic Enterprise, OpenAI Enterprise | Long cycles; high contract value; deep switching costs |
| Outcome/capacity-based | Salesforce Agentforce (experimenting) | Right fit for digital labor; hard to price before reliability is proven |
| Advertising | Google Search (~1.61 cents/search), Perplexity ($60 CPM) | Unproven in chat interfaces; brand safety concerns |

---

## Open Source vs. Closed — Decision Frame

Use when stories cover open-source model releases (Meta LLaMA, Google Gemma, DeepSeek, etc.).

**Go open when:** AI is complementary to your core business (not your revenue source); you want to commoditize a competitor's moat; you need community R&D; you want to attract developers.

**Stay closed when:** AI IS your revenue; you serve regulated industries requiring auditability; your moat is model quality or unique training data.

**LM frame:** Closed is the right call for AI Factory — LM's training data and deployment environments can't be open-sourced, and the regulated/classified context requires auditability. But *using* open-source models (Meta, IBM Granite) within the AI Factory is the right hedge against proprietary model lock-in.

---

## Defense / Regulated Industry Mappings

The quick reference library (Card 8) explicitly maps HBS case lessons to defense AI. Key parallels:

| Case lesson | Defense / LM parallel |
|-------------|----------------------|
| Adobe's commercially safe training → IP indemnification | LM AI Factory's data governance → auditable, trusted AI for DoD programs |
| Adobe's Content Credentials (provenance) | OPSEC requirements; chain-of-custody for AI-generated outputs in defense workflows |
| Anthropic's Constitutional AI (principle-based guardrails) | LM's command media and policy compliance layer — AI outputs bounded by governing policy |
| Anthropic's human-in-the-loop oversight (Level 1–2 autonomy first) | PM Approval Workflows; escalation design before autonomous action |
| Moderna's AI Academy → organizational change | LM's AI CoP and workforce training as strategic capability, not support function |
| Salesforce: business leaders own digital labor performance, not IT | PM owns AI-enabled workflow outcomes, not IT alone |
| Platform before products (all cases) | AI Factory as the enabling platform; programs are the products — don't build bespoke per program |
| Governance tiers (Moderna) | EVM/IMS outputs at Tier 3; internal drafting at Tier 1 — different controls for different stakes |

---

## What This Library Is NOT For

- Do not cite specific HBS case numbers in the roundup — this is internal reference, not sourcing
- Do not attribute financial figures to "an HBS case" — verify current figures through public sources before using in published editions
- These case lessons are strategic frames, not news events — use them to sharpen analysis, not as the stories themselves
