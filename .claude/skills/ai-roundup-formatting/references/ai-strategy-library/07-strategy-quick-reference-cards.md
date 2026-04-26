# AI Strategy Quick Reference Cards

## Decision Frameworks and Key Data Points for Executives

---

## Card 1: The AI Readiness Assessment

Before making any strategic AI decision, assess your organization across these dimensions:

### Data Readiness
- Do you have proprietary data assets that could train or differentiate AI models?
- Is your data clean, structured, and accessible?
- Do you have clear data governance and IP provenance?
- Can you offer customers IP indemnification?

### Talent Readiness
- Do you have AI/ML researchers who can build vs. just integrate?
- What's your GPU-per-researcher ratio vs. competitors?
- Can you articulate a mission that attracts mission-driven talent?
- Are your compensation structures competitive for the AI talent market?

### Infrastructure Readiness
- Do you have sufficient compute capacity (or cloud partnerships)?
- Can your tech stack support AI integration without major overhaul?
- Do you have MLOps capabilities for model deployment and monitoring?
- Have you evaluated custom silicon vs. Nvidia dependency?

### Organizational Readiness
- Does leadership have conviction about AI's strategic importance?
- Are cross-functional teams (not just engineering) involved in AI strategy?
- Do you have an AI ethics framework and governance structure?
- Is there a clear owner for AI strategy at the executive level?

### Customer Readiness
- How will your customers react to AI in your products?
- Which segments will embrace it vs. resist it?
- Do you understand the specific AI use cases your customers value?
- Have you developed a stakeholder communication strategy?

---

## Card 2: Key Financial Benchmarks from the Cases

### Revenue Trajectories
- OpenAI: $0 → $4B (2024) → $12B ARR (mid-2025)
- Anthropic: $0 → ~$1B (2024) → $3B ARR (mid-2025), projecting $12-34.5B by 2027
- Adobe Digital Media: $12.84B (2022), growing 10%+ YoY before GenAI integration

### Cost Benchmarks
- Model training: $900 (original Transformer) to $191M (Gemini 1.0 Ultra)
- OpenAI total development cost for ChatGPT: $540M+ (2022 alone)
- OpenAI projected cash burn: $8B (2025)
- Anthropic projected cash burn: $3B (2025), compute costs alone at $2.5B
- Inference cost addition to search: ~0.36 cents per query (basic)
- Inference costs declining ~30% annually

### Profitability Timelines
- OpenAI: expects cash flow positive by 2029 at $125B revenue
- Anthropic: best case breakeven by 2027
- Google: profitable overall but AI threatens the advertising margin structure

### Valuation Context
- Anthropic: $183B (September 2025) on $3B ARR (~61x revenue multiple)
- OpenAI: implied multi-hundred-billion valuation on $12B ARR
- Adobe: ~$315B peak market cap (December 2021), ~50% decline by December 2022

### Talent Cost Benchmarks
- OpenAI median software engineer: $810K/year
- San Francisco average software engineer: $220K/year
- Meta AI researcher signing bonuses: up to $100M (rumored)
- Scale AI CEO acquisition cost (Meta): $14.3B investment

---

## Card 3: The Monetization Menu

### Per-Unit / Usage-Based
- **How it works:** Charge per image generated, per API call, per token
- **Pros:** Revenue scales with usage, transparent
- **Cons:** Creates usage friction, unpredictable revenue, heavy users are unprofitable
- **Example:** OpenAI API token pricing, early DALL-E credit system

### Tiered Subscription
- **How it works:** Monthly plans at different capability/usage levels
- **Pros:** Predictable recurring revenue, customer segmentation
- **Cons:** Low free-to-paid conversion, heavy users subsidized by light users
- **Examples:** Anthropic ($17/mo Pro, $100/mo Max), OpenAI ($20/mo), Google ($249.99/mo Ultra)

### Bundled into Existing Products
- **How it works:** AI features included in current subscription pricing
- **Pros:** Drives adoption, deepens switching costs, minimal incremental customer acquisition cost
- **Cons:** Adds inference costs to existing revenue, may not capture full willingness to pay
- **Example:** Adobe GenAI in Creative Cloud, Microsoft Copilot in 365

### Enterprise / Custom Licensing
- **How it works:** Negotiated contracts for organization-wide deployment
- **Pros:** High contract values, deep integration creates switching costs
- **Cons:** Long sales cycles, heavy customization requirements
- **Examples:** Anthropic Enterprise, OpenAI ChatGPT Enterprise (600K+ paying business users)

### API / Platform
- **How it works:** Charge developers per-token for building on your models
- **Pros:** Ecosystem creation, scales without direct customer acquisition
- **Cons:** Prices declining rapidly, risk of customers cloning your model via API
- **Examples:** Anthropic API, OpenAI API, Google Gemini API

### Advertising
- **How it works:** Free to users, monetized through sponsored content
- **Pros:** Massive scale, proven model (in traditional search)
- **Cons:** Unclear how ads work in chat interfaces, brand safety concerns, low CPM efficiency
- **Examples:** Google Search ads (1.61 cents/search), Perplexity sponsored questions ($60 CPM)

---

## Card 4: Open Source Decision Matrix

### When to Open Source Your AI

Go open when:
- AI is complementary to your core business (e.g., Meta's social media)
- You want to commoditize a layer where competitors charge premium (attack their moat)
- You lack resources to keep pace alone and need community R&D
- You're trying to establish a standard or platform
- You want to attract developers and researchers to your ecosystem

Stay closed when:
- AI IS your core business and primary revenue source
- You need maximum control for safety and compliance
- Your competitive advantage comes from model quality
- You serve regulated industries requiring auditability
- You have unique training data you don't want replicated

Consider hybrid when:
- You want ecosystem effects but need to protect premium capabilities
- You serve both developer and enterprise markets
- You want to hedge against open source competition eroding your position
- You're in a period of rapid model improvement where today's premium is tomorrow's commodity

---

## Card 5: AI Agent Readiness Checklist

### Before Investing in AI Agents, Verify:

**Market Readiness**
- [ ] Is there a proven use case with measurable ROI in your industry?
- [ ] Are your customers asking for agent capabilities (vs. vendor-pushed)?
- [ ] Can you start with Level 1-2 autonomy (human-in-the-loop)?
- [ ] Do you have realistic expectations? (Remember: 40% cancellation prediction by 2027)

**Technical Readiness**
- [ ] Can you access 8+ data sources required for effective agent deployment?
- [ ] Is your tech stack ready, or do you need the upgrades 86% of organizations require?
- [ ] Can you handle the computational intensity of dynamic reasoning models?
- [ ] Do you have monitoring and guardrail infrastructure?

**Trust and Safety**
- [ ] Have you established human oversight protocols?
- [ ] Can you explain agent decisions to stakeholders?
- [ ] Are your data security policies robust enough for broad agent access?
- [ ] What's your plan for when (not if) an agent makes a critical error?

**Organizational Readiness**
- [ ] Do you have internal AI expertise or reliable partners?
- [ ] Have you communicated the impact on affected roles to employees?
- [ ] Is leadership aligned on risk tolerance for autonomous systems?
- [ ] Do you have clear success metrics and kill criteria?

---

## Card 6: Customer Communication Playbook (from Adobe)

### For AI-Skeptical Customer Bases

1. **Lead with values, not features.** Adobe's "amplify human intelligence, not replace it" message preceded specific product announcements by years.

2. **Build ethical infrastructure before you need it.** Adobe's AI Ethics Board (2019) and Content Authenticity Initiative preceded their GenAI model by years. This wasn't reactive crisis management; it was proactive trust-building.

3. **Use "Customer Zero" credibility.** Adobe's design team used their own tools first. Having internal professionals validate AI tools before external launch provides authentic testimonials.

4. **Address fears directly.** Adobe didn't dodge the job displacement concern — they acknowledged it and positioned AI as a tool that frees professionals for higher-order creative work while lowering barriers for newcomers.

5. **Provide concrete protections.** IP indemnification, Content Credentials for provenance, and commercially safe training weren't just marketing — they were tangible risk mitigations customers could verify.

6. **Segment your message.** Professionals care about control and workflow integration. Casual creators care about simplicity and output quality. Enterprises care about commercial safety and compliance. Tailor accordingly.

---

## Card 7: Critical Data Points for Board Presentations

### Market Size and Growth
- Global AI agent market: $5.1B (2024) → $47.1B projected (2030)
- GenAI consumer apps: ChatGPT leads with 339M MAU (Jan 2025), growing to 700M WAU by Aug 2025
- Enterprise adoption: 25% of companies expected to pilot AI agents by end of 2025, doubling by 2027
- 90% of executives view agentic AI as a potential source of competitive advantage

### Cautionary Data
- 95% of enterprise GenAI pilots yielding zero return (MIT, July 2025)
- 40% of agentic AI projects predicted to be cancelled by 2027 (Gartner)
- Only 3% of organizations trust AI agents for autonomous judgment calls
- 45% of business leaders concerned about data accuracy and bias
- No major GenAI company is profitable yet

### Investment Context
- U.S. private fixed investment in information processing equipment/software: 4.44% of GDP (Q2 2025), comparable to dot-com peak
- $2B+ invested in AI agent ecosystem
- Google's annual payment to Apple for default search: ~$20B
- Content licensing costs emerging: Google-Reddit deal at $60M/year

### Technology Trajectory
- LLM inference costs dropping ~30% annually
- But tokens per query increasing rapidly with reasoning models
- Performance gap between open and closed models narrowing
- Model switching costs lower than expected (3-5+ providers per Fortune 500 company)

---

## Card 8: The Program Guardian Connection

### Applying Case Lessons to Defense Industry AI Transformation

These HBS cases directly inform enterprise AI program management in defense:

**From Adobe — Commercially Safe AI for Regulated Environments:**
- Defense programs require IP-clean, auditable AI models
- Anthropic's Claude Gov for classified environments mirrors Adobe's commercially safe approach
- Content provenance (Content Credentials) parallels OPSEC requirements
- Customer indemnification maps to contractor liability frameworks

**From Google — The Platform vs. Application Decision:**
- Program Guardian's orchestration layer (Guardian as coordinator, Program Expert as domain-specific deputy) mirrors Google's platform strategy
- A2A and MCP protocols for multi-agent communication parallel Google's Agent2Agent protocol
- Custom infrastructure (Google's TPUs) parallels LM's Genesis platform investment

**From Anthropic — Safety-First Agent Design:**
- Anthropic's emphasis on human-in-the-loop oversight directly applies to PM Approval Workflows
- Constitutional AI's principle-based guardrails map to command media and policy compliance
- The agent autonomy levels (1-4) provide a framework for Program Guardian's phased deployment
- Pre-authorized autonomous actions (Phase 2) should start at Level 1-2, with PM approval gates before any Level 3 capability

**Enterprise AI Adoption Lessons:**
- 86% of organizations need tech stack upgrades → Genesis platform modernization
- 8+ data sources required → IMS, ROADS, VEMO, PMM, Supply Chain integration
- Multi-homing is the norm → ADK orchestration supporting multiple sub-agents
- Vertical specialization beats horizontal → Program Expert configured per-program

---

*These quick reference cards are designed for rapid retrieval during strategic planning sessions, board presentations, and investment decisions. Each card can be used independently or in combination with the full AI Strategy Library and Case-by-Case Lessons documents.*
