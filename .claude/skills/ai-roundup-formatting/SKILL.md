---
name: ai-roundup-formatting
description: >
  Use this skill EVERY TIME the user asks to write, draft, create, produce, or format a weekly AI roundup, AI briefing, AI newsletter, or AI news summary — especially for a Lockheed Martin or defense/enterprise audience. Also trigger when the user says things like "write up this week's AI news", "put together the roundup", "make the weekly post", or "turn these stories into a briefing". This skill defines the exact structure, tone, and voice that must be followed. Do NOT skip this skill and improvise a format.
---

# Weekly AI Roundup Formatting Skill

## Before You Start

Read all reference files before drafting. They are short and the quality of your output depends on them:

1. **`references/voice.md`** — John's specific language patterns, rhetorical moves, organizational identity language (RMS, "our front yard," triple imperatives, etc.), and what to avoid
2. **`references/examples.md`** — Three annotated published posts. The annotations explain *why* each move works, not just what it is.
3. **`references/org-context.md`** — LM organizational context: internal initiatives (AI Factory, EP&T, Genesis), terminology and acronyms, audience intel, functional org roles, and RMS program workflow context. Essential for writing RMS Relevance sections that name something specific instead of gesturing at "AI adoption."
4. **`references/lm-ai-strategy.md`** — LM AI Factory strategic backgrounder: concrete metrics (1B+ tokens/week, 50K+ users, training weeks→days), tech stack, key partnerships (NVIDIA, IBM, Microsoft, Red Hat, Google, Meta, Oracle), Astris AI commercialization, competitive landscape (Palantir, Anduril, traditional primes), and risk factors from the 10-K. Use for scale calibration, competitor references, and the Strategic Picture.
5. **`references/ai-strategy-benchmarks.md`** — Synthesis of the AI Strategy Library (8 HBS case-based documents on Adobe, Google, Anthropic, Moderna, Salesforce, and value chain analysis). Use for: company benchmarks (OpenAI/Anthropic ARR and burn rates, inference economics, training cost trajectories), enterprise adoption data (95% of pilots yield zero return, 40% of agent projects cancelled), recurring strategic patterns to name in the Strategic Picture (model is not the moat, platform beats pilots, trust as competitive advantage), and defense/regulated industry mappings. Full source files are in `references/ai-strategy-library/` if deeper context is needed.

Reading these takes five minutes. Skipping them produces generic output that misses the voice and gets the relevance sections wrong.

---

## Inputs

The user will typically provide:
- 3–4 AI news stories (as links, pasted text, or brief descriptions)
- Optionally, a suggested theme or connecting thread
- Optionally, a prior edition as a style reference

When the user provides articles directly, use those — don't substitute adjacent stories. If they've chosen what to cover, the job is execution, not selection. If the user provides only brief descriptions or links, use web search to gather enough detail for a substantive summary. If the user provides paywalled content directly, work with what they provide.

---

## Document Structure

Every roundup follows this structure exactly, in order:

### 1. Title

```
AI Weekly Roundup – Week of [DATE]
```

The em-dash (`–`) is required. "AI Weekly" comes before "Roundup." Include the specific date.

### 2. Framing Hook (1–2 sentences)

Immediately below the title. This is the most important sentence in the document — it should deliver a strategic insight or pose a strategic question, not preview the three headlines. A reader who only reads this one sentence should walk away with the most important thing to understand about this week.

Patterns that work:
- "...this week's stories point to the same strategic question: [question]?"
- "...this week's signals converge on [theme]."
- "...[X] isn't a future state. It's the current competitive landscape."
- Two-part hook: narrative setup, then strategic verdict in two short sentences.

**Do not** open with "This week we cover..." or any list of what's coming.

### 3. Story Sections (3–4 stories)

Each story follows this structure:

```
[#]. [Headline Framed as Insight — not a neutral news headline]
Coverage: [Source(s) / Publication name]

[Body: see formats below]

RMS Relevance: [2–4 sentences connecting to LM/RMS context]

---
```

**Headline framing:** The headline should deliver the strategic conclusion, not describe the event. Compare:
- Weak: "OpenAI Acquires OpenClaw Developer"
- Strong: "OpenAI's Hire of OpenClaw's Creator Is a Bet on Agent Infrastructure as the Next Competitive Moat"

**Body formats — choose based on the story:**

*Format A (default — flowing prose):* 3–5 paragraphs, each 2–4 sentences. Structure: what happened → why it matters → deeper implication(s). Lead with the strategic significance, not just the news. Use **bold lead-in phrases** to organize key dimensions within paragraphs when the story has multiple distinct angles — e.g., "The core technology:", "The business model shift:", "The competitive signal:", "The supply chain angle:", "What went wrong:", "The fix:". Pick framing that fits the story — don't force a template.

*Format B (trend aggregation):* An opening framing paragraph, then bullet points showing multiple data points or companies, then a synthesis paragraph labeled "The Pattern:" or similar. Use when the story is really a collection of signals (multiple companies doing the same thing, a study with multiple findings, etc.).

**RMS Relevance:** This section is mandatory. The label is **"RMS Relevance:"** (not "Relevance:"). It should:
- Name a specific LM function, program type, workflow, or capability at stake — not just assert that AI is important
- Use first-person plural: "our programs," "we're seeing this internally," "our workforce"
- Reference specific LM context when appropriate: AI Factory, EP&T, Genesis, RMS, program management, manufacturing, classified environments
- End with either an action orientation ("worth tracking closely" for early signals, or a specific recommendation for mature signals)

### 4. The Strategic Picture

This section earns its place by finding the through-line the reader wouldn't have seen on their own. It must not just restate the stories.

```
The Strategic Picture

[1–2 sentences connecting all stories to a single convergent dynamic]

[2–4 paragraphs or named subpoints developing the convergence]

[Closing: triple imperative OR direct question to the reader]
```

Opening patterns:
- "These [N] stories aren't disconnected headlines. They're converging on..."
- "Three stories this week point to the same underlying dynamic."
- "[N] stories this week point to the same strategic question."

Connect the threads explicitly — show how Story 1 relates to Story 3, how a theme in Story 2 reinforces or complicates the lesson from Story 4. The reader should feel that the stories were curated because they illuminate the same underlying dynamic. Every sentence should be doing work: connecting stories, naming the convergence, or issuing the takeaway. No throat-clearing.

Closing options:
- **Triple imperative** (when the post calls for action): Three short parallel sentences ending on verbs. *"Build the pipe. Architect for swap-out. Get to production."*
- **Direct question** (when the post is more of an assessment): A challenge back to the reader. *"Are we moving fast enough?"*
- **Posture statement:** *"That's the posture we need."*

### 5. Footer

```
US-EPT-AI-Solutions-CoP
```

No punctuation. No tagline. Just the community name.

---

## Tone & Writing Guidelines

**Confident, direct, informed.** Write like a trusted colleague briefing a peer, not a journalist writing for clicks.

**No hype words:** avoid "revolutionary," "game-changing," "paradigm shift," "unprecedented," "transformative" — unless quoting someone and it serves a purpose.

**No corporate filler:** avoid "leverage synergies," "drive transformation," "unlock value," or passive hedged language like "it could potentially suggest that perhaps..."

**Analytical, not breathless.** Show the reader why something matters rather than telling them it's important.

**Mix sentence lengths deliberately.** Short declarative sentences after longer analytical ones land hard. The final short sentence is the punch.

**Quantitative proof points:** At least two per story, attributed correctly. Numbers matter — pass rates, revenue figures, investment amounts, headcount changes. Don't invent numbers or paraphrase quotes into claims the original source didn't make.

---

## Key Voice Moves

These appear in the published examples and should be used when the story supports them. Don't force them — earn them.

**Scale calibration:** When a story involves a large dollar figure, ground it by comparing to LM's known financials (revenue ~$74.7B, market cap varies). This makes abstract numbers tangible. Skip if you don't have a reliable current figure — don't fabricate.

**"Our front yard":** Use when a story about manufacturing, physical systems, aerospace, or defense-adjacent tech intersects with LM's territory. Signals that LM is inside this story, not watching it.

**"That should be us":** Use when an outside company is doing something LM could or should be doing. Direct challenge.

**"The real story isn't X, it's Y":** Use in the first paragraph of a story body when the surface-level event hides the more important signal.

**"Rhymes with":** When an outside-industry story is structurally analogous to LM's situation without being directly comparable. *"That is not the same role Lockheed Martin plays, but it rhymes with it."*

**Security as advantage:** When a story involves security concerns in enterprise AI, reframe LM's classified-environment expertise as an advantage. *"Our expertise in compartmentalization and classified environments isn't a constraint — it can be an advantage in this moment."*

**"Worth tracking closely":** Use to close a Relevance section when the story is early-signal rather than immediate-action.

**The contrast pivot:** *"It's not perfect [...] But the point isn't replacing production compilers. It's what happens when you design the right orchestration..."*

---

## RMS Relevance — How to Write It Well

This is the most important differentiator of the roundup. To write it well:

1. Read `references/org-context.md` for LM/RMS context — internal programs, acronyms, audience roles
2. Connect the external development to specific RMS realities: programs, capabilities, organizational dynamics, competitive position, or internal initiatives
3. Be concrete. "This could apply to our manufacturing workflows" is weak. "The use of video models to train autonomous systems on production floor data could apply directly to defense/aerospace assembly, inspection, and maintenance workflows" is strong.
4. When possible, reference AI Factory, EP&T AI program, Genesis platform, AI Community of Practice, or other internal initiatives the reader will recognize — Program Guardian, the BA Suite
5. Frame relevance as opportunity, competitive benchmark, design lesson, or strategic signal — not just "this is interesting"

What NOT to write:
- "This could help LM stay competitive" — too vague
- "AI adoption is accelerating across industries" — that's the story, not the relevance
- "This is relevant to Lockheed Martin because AI is important" — not a relevance statement
- Referencing internal initiatives the audience doesn't recognize — if you name something, it must be real
- Invented LM executive quotes or positions not sourced from the article

---

## What Strong Output Looks Like

- The framing hook poses one strategic question that all stories answer
- Each headline is interpretive, not descriptive
- The body of each story moves fast from event to implication — no lingering summaries
- RMS Relevance sections are specific, not generic — they name the workflow, program type, or capability at stake
- The Strategic Picture names the convergent dynamic that wasn't obvious from reading the stories individually
- The closing lands — either a triple imperative or a direct challenge to the reader
- It reads like a briefing a senior leader would forward, not a newsletter they'd skim

---

## Anti-Patterns

- Opening with a story preview instead of strategic insight
- Neutral news headlines ("Company X Does Y")
- Generic Relevance sections ("This matters for Lockheed Martin because AI is evolving rapidly")
- A Strategic Picture that just says "all three stories are about AI deployment"
- Missing the "RMS Relevance:" label (not "Relevance:")
- Missing the footer
- Long paragraphs (more than 5 sentences)
- Buzzwords without grounding ("transformative," "revolutionary")
- Bullet summaries instead of narrative prose in story bodies
- Vague connections in RMS Relevance ("could help with program management broadly")
- Losing the thread in the Strategic Picture — every sentence must be doing work
