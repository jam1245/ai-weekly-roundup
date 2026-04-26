# Case-by-Case Lessons Learned: Deep Dives

## Companion Document to the AI Strategy Library

---

## Case 1: Adobe — GenAI Opportunity or Threat? (HBS 9-525-052)

### Company Context

Adobe is a $17.6B revenue company (FY2022) anchored by three pillars: Creative Cloud (~$10.7B), Document Cloud (~$2.5B), and Experience Cloud (~$4.4B). The company successfully navigated the perpetual license-to-subscription transition a decade earlier under CEO Shantanu Narayen. At the case's opening (December 2022), Adobe's stock had dropped ~50% YoY despite record revenue, and a pending Figma acquisition signaled competitive pressure from below.

### Strategic Decisions and Their Logic

**Decision 1: Dive In, Don't Wait**

Internal voices advocated three positions: stay out entirely (the technology isn't ready for professional use), wait and see (let others prove the market), or dive in (this is a once-in-a-lifetime technology shift). The "dive in" camp won.

*Why it mattered:* Adobe's Malte Bernholz called it a "once-in-a-lifetime technology shift." The risk of inaction was greater than the risk of action. Even if early models were rudimentary, the pace of improvement (DALL-E to DALL-E 2 in months) meant the quality gap would close fast.

**Decision 2: Build Your Own Model**

Arguments for partnering were compelling: faster time to market, lower cost, staying focused on core tooling competencies. But Adobe chose to build, driven by the conviction that their goals were "radically different" from potential partners' AGI-focused missions.

*Key enablers:* Adobe's Head of Research (Gavin Miller) provided the conviction that they could match or exceed competitors. Pre-existing compute investment (ramped since mid-2021) meant infrastructure was ready. And Adobe Stock's 300M+ curated assets provided irreplaceable training data.

**Decision 3: Commercially Safe Training Only**

This was Adobe's most distinctive strategic choice. By training exclusively on content they had rights to use (Stock images, public domain, Creative Commons, licensed material), Adobe created a differentiated product that competitors couldn't easily replicate.

*The enabling infrastructure:* Stock contributor terms already allowed derivative product creation. Images had undergone AI and human moderation to strip IP and inappropriate content. Public domain and Creative Commons expanded the dataset further.

*The competitive advantage:* IP indemnification for customers. Enterprise and agency adoption (clients who would "never touch" unverified GenAI). International regulatory readiness. Brand safety — the model literally couldn't generate Batman because it had never seen Batman.

**Decision 4: Integration Over Standalone**

Rather than launching a separate GenAI product, Adobe chose to weave AI into existing tools as a "superpower." The reasoning: Adobe's strength was in customer workflows, not standalone image generation. Integration would delight existing subscribers and deepen switching costs.

### Lessons for Executives

1. **Your existing assets are more valuable than you think.** Adobe's Stock library, contributor terms, and creative workflow expertise weren't built for GenAI, but they became its most important strategic inputs. Audit your company's assets through the lens of AI before assuming you need to acquire new ones.

2. **Values can be competitive advantages.** Adobe's commitment to commercial safety, content provenance, and creator rights wasn't just ethics — it was strategy. Enterprise customers pay premiums for safety guarantees.

3. **Cross-functional alignment is essential.** Narayen included research, applied research, product, design, marketing, and strategy in GenAI planning because GenAI is "a little bit like alchemy" requiring all perspectives.

4. **Don't underestimate your customer relationship.** Adobe understood their customers deeply enough to know professionals wanted control, not a "slot machine." This insight shaped product design toward workflow integration rather than standalone generation.

5. **The CFO is a strategic partner, not just a financial controller.** Dan Durn recognized that communicating the long-term vision to investors was as important as managing profitability. AI transitions require patience from capital markets.

6. **Hedge your bets internally.** While committing to build, Narayen maintained benchmarks and hedges. The strategy was conviction paired with pragmatism.

---

## Case 2: AI Wars in 2025 (HBS 9-725-484)

### Company Context

Google/Alphabet dominates search (93.4% global desktop share) and digital advertising, generating hundreds of billions in revenue. The company invented key AI technologies (Transformer architecture, TensorFlow) but was perceived as falling behind in commercializing generative AI. In June 2025, the revelation that Google searches declined for the first time in 20 years triggered a quarter-trillion dollar market cap loss.

### The Competitive Landscape Dynamics

**OpenAI: The Disruptor**

OpenAI demonstrated the power of consumer-first product design. ChatGPT reached 100M users in 2 months — the fastest consumer app adoption in history. Key strategic moves included: novel training approaches (low-cost human annotation in Kenya, Uganda, India), shifting from open to closed source (creating controversy but protecting IP), massive Microsoft partnership ($10B+ investment, Azure exclusivity), and API access creating a developer ecosystem (with the acknowledged risk of competitors cloning models).

*Financial reality:* Despite 700M weekly active users and $12B ARR by mid-2025, OpenAI projected $8B cash burn and didn't expect profitability until 2029 at $125B revenue.

**Meta: The Open-Source Disruptor**

Meta pursued open-weight models (LLaMA) because its business model didn't depend on selling compute — unlike Google, Microsoft, or Amazon. Open source let Meta benefit from community improvements, drive down infrastructure costs, and position its tools as industry standards.

*The talent gambit:* Zuckerberg launched Meta Superintelligence Labs with $100M signing bonuses, but the strategy showed early cracks. Key talent rejected Meta for mission-driven companies, and pay disparities created cultural problems. Some recruits left within months.

**DeepSeek: The Efficiency Disruptor**

DeepSeek's R1 model demonstrated that architectural innovation (Mixture of Experts, distillation) could achieve near-frontier performance at dramatically lower cost. This challenged the assumption that AI leadership required massive capital expenditure and raised questions about Nvidia's GPU dominance.

*Meta's Yann LeCun acknowledged:* DeepSeek built on open research (including Meta's PyTorch and LLaMA), came up with new ideas, and shared them back — demonstrating the virtuous cycle of open source.

**Perplexity: The Answer Engine**

Perplexity positioned itself as an "answer engine" rather than a search engine, using LLMs to synthesize responses rather than return pages of links. The company acknowledged using OpenAI and Anthropic models through API access, essentially building an application layer on top of others' foundational models.

*Monetization struggles:* Perplexity admitted subscriptions alone couldn't sustain the business and moved to advertising at $60 CPM. Advertisers cited limited scale, unclear ROI, and brand safety concerns.

### Google's Multi-Pronged Response

1. **Incremental Search integration:** AI Overviews (7-15% of searches) and a separate AI Mode tab rather than wholesale replacement. Preserved the ad business while experimenting.

2. **Strategic investment:** $2.3B+ into Anthropic to hedge against being bypassed, with Google Cloud commitments.

3. **Open source hedging:** Gemma models to maintain ecosystem leadership and prevent Meta from owning the open source standard.

4. **Custom silicon:** Trillium TPUs to reduce Nvidia dependency and lower long-term compute costs.

5. **Premium subscription:** AI Ultra Plan at $249.99/month for power users, testing willingness to pay.

### Unit Economics Deep Dive

The case provides the clearest picture of GenAI economics in the industry:

- Traditional search cost: ~1.06 cents per query
- GenAI inference addition: ~0.36 cents per query (basic)
- Search ad revenue: ~1.61 cents per query
- But: 10x longer prompts = 10x inference cost
- And: more complex models (reasoning, step-by-step) cost dramatically more
- Inference costs declining ~30% annually, but usage is growing faster
- Subscription ceiling: even Netflix, Spotify, and Microsoft 365 max out at ~400M paid users globally
- Pareto distribution: 20% of paid users would represent 80% of usage, making heavy subscribers unprofitable

### Lessons for Executives

1. **Inventing the technology doesn't guarantee capturing the value.** Google invented the Transformer but OpenAI commercialized it. Having the best research lab is necessary but insufficient — you need product-market fit, consumer UX, and speed to market.

2. **Distribution is a double-edged sword.** Google's dominance in search, Chrome, and Android provided massive distribution for AI features. But that same dominance created antitrust risk (the DOJ case) and made competitors attractive to regulators.

3. **Risk aversion is the real threat to incumbents.** Google's culture evolved toward caution about ethical, reputational, and legal risks. While these concerns were valid, they slowed response time. Competitors with less to lose moved faster.

4. **No one has solved AI monetization yet.** The most successful GenAI product in history (ChatGPT) is deeply unprofitable. The search advertising model may not translate to chat. Subscription conversion is low. Advertising in AI responses is unproven. Executives should plan for a multi-year investment period.

5. **Open source can be a competitive weapon regardless of your position.** Google used open source (TensorFlow, Chrome, Android) to cement platform leadership. Meta used open-weight LLMs to commoditize the model layer and benefit from community R&D. Both strategies served their respective business models.

6. **Custom infrastructure creates long-term advantage.** Google's TPUs represent a decade-long investment in reducing dependency on Nvidia. Companies that control their compute stack have more flexibility on pricing and capacity.

7. **Copyright is a growing liability.** The wave of AI copyright lawsuits (NYT vs. OpenAI, Reddit vs. Anthropic, and dozens more) creates legal uncertainty that affects every company using AI. Content licensing deals ($60M/year for Google-Reddit) add costs but reduce risk.

8. **Section 230 protection may not cover AI-generated responses.** This is a potentially massive legal exposure for any company delivering AI-generated answers "in its own voice" rather than surfacing third-party links.

---

## Case 3: From LLM to Agent? Anthropic's Next Move (HBS 9-726-407)

### Company Context

Anthropic was founded in 2021 by former OpenAI executives concerned about rapid commercialization at the expense of safety. By fall 2025, the company had achieved $3B ARR, 32% enterprise AI market share (surpassing OpenAI), a $183B valuation, 42% code generation market share, and a $200M U.S. Department of Defense prototype agreement. However, the industry was pivoting from LLMs to autonomous AI agents, threatening to shift the competitive landscape.

### Anthropic's Distinctive Strategic Choices

**Public Benefit Corporation structure** with a Long-Term Benefit Trust (LTBT) that had board appointment authority. This wasn't window dressing — it structurally bound the company to prioritize long-term societal benefit.

**Constitutional AI** reduced reliance on human-labeled training data by training models to follow human-written guiding principles, with refinement by other models. This made safety oversight more scalable and transparent.

**Fully closed source** — unlike competitors pursuing hybrid strategies, all Anthropic models remained proprietary. This aligned with safety goals but left them potentially vulnerable as open models narrowed the performance gap.

**Premium pricing** — Claude's API costs exceeded most competitors (Claude Opus 4.1 input cost was roughly $15/million tokens vs. single digits for many alternatives). This worked while Claude led on quality but created risk as models converged.

**Safety-first timing** — Anthropic had Claude ready before ChatGPT launched but delayed for safety testing. This cost them the first-mover advantage in consumer chatbots.

### The Agent Decision Framework

Anthropic faced five strategic paths:

1. **First-mover into agents:** Aggressively launch agent platforms/applications, accepting higher risk. Pro: captures market position. Con: conflicts with safety-first mission and may produce unreliable products.

2. **Deliberate follower:** Learn from competitors (OpenAI Operator, Salesforce Agentforce, Microsoft Build 2025) to identify successful patterns. Pro: lower risk, can enter with superior products. Con: market moving at breakneck speed.

3. **Consumer agents:** Leverage Claude's conversational strengths for personal assistants, competing directly with ChatGPT Agent. Pro: large addressable market. Con: requires massive consumer acquisition spend.

4. **Enterprise/government agents:** Target regulated industries where safety and reliability carry premium value. Pro: aligns with Anthropic's strengths. Con: long sales cycles, intensifying competition.

5. **Vertical specialization (coding):** Rather than horizontal expansion, deepen dominance in code generation (already 42% market share, 2x OpenAI). Pro: plays to demonstrated strength, clear monetization. Con: limits total addressable market.

### Agent Market Realities

The case paints a sobering picture of agent readiness:

- 40% of agentic AI projects predicted to be cancelled by 2027 (Gartner)
- 95% of enterprise GenAI pilots yielding zero return (MIT, July 2025)
- Only 3% of organizations trust agents for autonomous judgment calls
- 86% need significant tech stack upgrades for agent deployment
- Hallucination rates remain high even in newest models
- Regulatory framework is fragmented globally

### Lessons for Executives

1. **Safety can be a sustainable competitive advantage.** Anthropic's safety-first approach attracted the Department of Defense, enterprise clients in regulated industries, and mission-driven talent that rejected higher-paying competitors. In a world where AI errors can cause real harm, reliability is premium.

2. **The late-mover penalty is real but surmountable.** Anthropic delayed Claude's launch and lost consumer mindshare to ChatGPT. But by focusing on enterprise quality, they surpassed OpenAI in enterprise market share within two years. The consumer and enterprise markets reward different things.

3. **Model convergence threatens pure-play model providers.** As performance differences between models narrow, differentiation shifts to developer ecosystems, safety features, integration ease, and pricing. Companies building on a single model's superiority must plan for a future where that advantage diminishes.

4. **Multi-homing is the enterprise norm.** Most Fortune 500 companies use 3-5+ different model providers. This suggests that no single model will dominate, and that switching costs may remain lower than expected. Platform and ecosystem stickiness matters more than model performance.

5. **Vertical specialization may be the winning strategy in the agent era.** Broad, horizontal agents face massive trust barriers. Domain-specific agents (Harvey in legal, Decagon in customer experience, Anthropic in coding) can achieve higher reliability in narrow domains and build deep customer relationships.

6. **Don't build full-stack unless you must.** Anthropic grew through partnerships (Salesforce, BCG, Accenture, Slack, GitHub) rather than building end-to-end applications. This conserved resources for core model development. In a fast-moving market, platform strategies often beat application strategies.

7. **Talent loyalty follows mission, not money.** Anthropic staff rejected $100M Meta offers because of alignment with the company's values. In the current talent market, having a compelling mission and research culture may be more sustainable than compensation-driven retention.

8. **The agent era is earlier than the hype suggests.** Despite $2B+ in investment and breathless coverage, most "agentic" products are glorified automation tools at Level 1-2 autonomy. Executives should experiment cautiously, start with human-in-the-loop designs, and be skeptical of vendor claims about agent capabilities.

---

## Comparative Analysis: Key Themes Across Cases

### Theme 1: Speed vs. Safety

| Company | Approach | Outcome |
|---------|----------|---------|
| OpenAI | Speed first, safety second | Massive consumer adoption, but leadership crises, lawsuits, and talent departures |
| Adobe | Deliberate but decisive | Maintained customer trust while building competitive GenAI capabilities |
| Google | Cautious incumbent | Perceived as behind despite technical leadership; cultural risk aversion slowed response |
| Anthropic | Safety first | Lost consumer first-mover to ChatGPT but won enterprise market share |

### Theme 2: Business Model Fit

| Company | AI Role | Monetization Strategy |
|---------|---------|----------------------|
| Adobe | Enhances existing subscription products | Bundle AI into Creative Cloud subscriptions |
| Google | Potentially cannibalizes core ad business | Incremental integration, premium subscriptions, preserved ad model |
| OpenAI | AI *is* the product | Subscriptions + API + enterprise licensing |
| Anthropic | AI *is* the product | Premium API pricing + enterprise partnerships |
| Meta | AI enables existing ad/social business | Open source models, monetize through ad-supported platforms |

### Theme 3: Data as Competitive Moat

| Company | Data Advantage |
|---------|---------------|
| Adobe | 300M+ curated, commercially safe Stock images |
| Google | Decades of search data, YouTube, Gmail, Maps |
| OpenAI | Novel low-cost annotation pipelines, massive user interaction data |
| Meta | 3B+ social media users, open-weight community contributions |
| Anthropic | Constitutional AI training approach, safety evaluation data |

### Theme 4: Ecosystem Strategy

| Company | Approach |
|---------|----------|
| Adobe | Platform-agnostic; allowed third-party models alongside its own |
| Google | Invested in competitors (Anthropic), open-sourced lower-tier models, built developer tools |
| OpenAI | Moved from open to closed; built walled-garden app ecosystem |
| Meta | Open-weight models to create community dependency |
| Anthropic | API-first; partnerships for distribution; closed models |

---

*Each case offers distinct but complementary lessons. The strongest executive strategy draws from all three: Adobe's customer-centric values, Google's ecosystem thinking, and Anthropic's principled focus on safety and quality.*
