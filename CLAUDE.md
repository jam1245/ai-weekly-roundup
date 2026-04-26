# Weekly AI Roundup — Project Context

## What This Is

A weekly internal AI newsletter called the **Weekly AI Roundup**, written for 500+ DoD program management practitioners across our AI Community of Practice at Lockheed Martin RMS. Each edition covers three to four recent AI developments drawn from sources like the Wall Street Journal and industry analyst reports, then turns each one into a structured write-up ready to drop directly into our internal channels.

The audience is practitioners — they understand the business, they're close to active programs, and they can tell when a relevance connection is real versus generic. Generic doesn't fly here.

## Audience & Community

- **Who reads it:** 500+ practitioners in DoD program management
- **Community:** US-EPT-AI-Solutions-CoP (this is also the footer on every edition)
- **Division context:** Lockheed Martin RMS (Rotary & Mission Systems)
- **Internal platform:** AI Factory — LM's scalable, secure, open-architecture AI ecosystem. Reference it when stories touch infrastructure, platform strategy, or vendor lock-in.

## Workflow Stages

The process moves in roughly this order, though it's not always perfectly linear:

**1. Story selection** — Scan recent news and pick three to four articles with clear strategic relevance. Good signals: a CEO changing an AI pricing model, a consulting firm reporting a bookings surge tied to AI services, a major capital investment in defense-adjacent manufacturing, or a model capability shift that changes what's possible in production workflows. Avoid stories that are interesting but disconnected from what program teams actually deal with.

**2. Source extraction** — Read each article closely and pull out the key data points, executive quotes, and strategic claims worth repeating. Numbers matter: pass rates, revenue figures, investment amounts, headcount changes. Attribution matters: don't invent numbers or paraphrase quotes into claims the original source didn't make.

**3. Draft each story entry** — Follow the format in the ai-roundup-formatting skill exactly: interpretive headline, narrative body with metrics embedded, RMS Relevance section tied to a specific internal initiative, and scale comparisons when helpful (e.g., benchmarking a competitor's investment against LM's revenue or market cap).

**4. Write the synthesis** — The closing Strategic Picture connects all the stories into one narrative arc that a senior leader could repeat in a meeting without needing extra context. This is harder than it sounds. The goal is a through-line that wasn't obvious from reading the stories individually.

## Inputs

- **Three to four URLs or copied excerpts** from recent articles — often from paywalled sources the author already has access to
- **A prior edition** as the style reference (tone, header conventions, section structure, how specific the relevance parts need to be)
- **Optional author notes** on which internal initiatives a given story should map to — when these exist, use them; when they don't, make the best connection you can from context

When an author provides specific articles directly, use those. Don't substitute adjacent stories — if they've chosen what to cover, the job is execution, not selection.

## Success Criteria

A strong edition hits all of these:

- **Story count:** Three to four stories per edition
- **Length per story:** 150–250 words
- **Quantitative proof points:** At least two per story, attributed correctly, not invented
- **RMS Relevance:** Names a specific internal initiative or strategic priority — not vague lines about "AI adoption" or "digital transformation." Draws a real parallel to actual business work, not a general nod.
- **Strategic Picture / synthesis close:** Connects all stories into a single narrative arc. A senior leader should be able to repeat it in a meeting without extra context.
- **Tone:** Grounded, direct, no hype. Consistent labeling across sections. Matches the voice in the prior edition provided.
- **Format:** Follows the ai-roundup-formatting skill schema exactly — interpretive headline, narrative paragraphs (not bullets), RMS Relevance label, Strategic Picture, footer.

If the relevance section is vague or the synthesis feels rushed, the whole thing reads weaker. Those two sections are where quality shows or falls apart.

## What Tends to Go Wrong Without the Skill

Without the ai-roundup-formatting skill active, outputs tend to:
- Produce summaries that are fine but not right for this audience
- Miss the interpretive headline convention (neutral news headlines instead)
- Lean on bullet lists instead of narrative paragraphs
- Skip or genericize the RMS Relevance section
- Write a weak or disconnected Strategic Picture

The skill enforces the schema and voice. Always use it for roundup drafting.

## Source Handling Notes

- **Web search** helps but doesn't always surface the articles that will land best with this business audience. When the author already knows what to cover, take the articles directly — it cuts noise and makes the relevance mapping cleaner.
- **Paywalled sources:** Authors typically have access. Work with what they provide rather than trying to retrieve paywalled content independently.
- **LinkedIn posts:** Some reference material comes from specific LinkedIn voices the author follows and has saved. These are useful but may get dated — treat them as contextual reference, not authoritative source.

## Skill Architecture

This project uses the **ai-roundup-formatting** skill, which lives in `.claude/skills/ai-roundup-formatting/`. It includes:
- `SKILL.md` — the main formatting and voice instructions (merged, comprehensive)
- `references/voice.md` — specific language patterns, rhetorical moves, organizational identity language
- `references/examples.md` — three annotated published editions explaining why each move works
- `references/org-context.md` — LM org context, internal initiatives, acronyms, audience roles
- `references/lm-ai-strategy.md` — AI Factory metrics, tech stack, partnerships, competitive landscape
- `references/ai-strategy-benchmarks.md` — enterprise AI benchmarks, strategic patterns, company comparisons
- `references/ai-strategy-library/` — full source case files (Moderna, Salesforce, Adobe, Google, Anthropic, etc.)

**IMPORTANT — Skill Loading:** A system-level `weekly-ai-roundup` skill may auto-trigger when asked to draft a roundup. That skill provides basic structure only. You MUST also read the `ai-roundup-formatting` skill's reference files above before drafting — they contain the voice patterns, RMS Relevance grounding, LM strategy context, and annotated examples that make the difference between generic output and a post that lands with this audience. Load both. The reference files are short. Skipping them is where quality falls apart.

Multiple skills may be in use depending on the week — the formatting skill handles structure and voice, and separate skills tied to specific business priorities can help with the RMS Relevance connections when the author wants better grounding in what the company is prioritizing that quarter.
