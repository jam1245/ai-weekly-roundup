---
name: ai-story-selector
description: >
  Use this skill BEFORE drafting any weekly AI roundup when the user does not already have a fixed set of articles to cover. Trigger when the user says "find stories for this week," "what should we cover," "pick the articles," "what's worth including," or any variation of asking Claude to select stories from the news landscape rather than drafting from provided articles. This skill defines the editorial criteria for story selection and outputs a ranked shortlist with justification before any drafting begins.
---

# AI Roundup Story Selection Skill

## Purpose

This skill governs the story selection stage — Step 1 in the roundup workflow. It exists because the quality of a weekly AI roundup is largely determined before a single word is written. Story selection is an editorial judgment, not a search task. The wrong stories produce technically correct drafts that miss the audience entirely.

This skill should be used when:
- The user has not already provided specific articles or URLs
- The user asks Claude to find, identify, or recommend stories for the week
- Claude needs to search for stories autonomously and select from the results

When the user already provides specific articles or URLs, skip this skill and proceed directly to `ai-roundup-formatting`.

---

## Who This Audience Is

Before selecting stories, hold this question in mind: **What does a program manager at Lockheed Martin RMS need to understand about the AI landscape this week to do their job better or to make a better strategic decision?**

The audience manages billion-dollar defense programs. They live inside EVM compliance, schedule reviews, fixed-price contracts, and workforce constraints. They are not academics, product managers, or AI researchers. A story that is fascinating to a Silicon Valley audience may be irrelevant or misleading to this one.

---

## Story Selection Criteria

### Mandatory Signals — Include if Present

A story is worth shortlisting if it contains at least ONE of the following:

1. **A CEO or executive decision that changes market structure** — pricing changes, acquisitions, platform strategy shifts, organizational restructuring triggered by AI. Decisions reflect calculated bets, and bets reveal where the smart money thinks the market is going.

2. **A concrete metric that moves the strategic argument** — revenue figures, investment amounts, adoption rates, failure rates, benchmark scores. Numbers that can be compared, scaled, and calibrated against LM's context are worth ten times more than qualitative claims.

3. **A direct defense, government, or manufacturing analog** — a story about aerospace, physical systems, regulated industries, national security, or supply chain that maps directly to LM's operating environment. "Our front yard."

4. **A capability shift that changes what's possible in production workflows** — not a research paper, but a deployed product or capability that program teams could realistically use within 18 months. The AI reliability story from April 2026 was this kind of story. A new SOTA benchmark on a research task is not.

5. **A failure or cautionary data point** — stories about what isn't working, what percentage of pilots fail, what governance mistakes enterprises are making. These often land harder with practitioners than success stories because they validate real friction points.

6. **A geopolitical or supply chain signal with program-level implications** — model provenance, export controls, foreign AI infrastructure dependency. Anything that intersects with the mission assurance and supply chain questions program teams already manage.

### Exclusion Signals — Do Not Include

Exclude a story if it matches any of these patterns, even if it is widely covered:

- **Pure research / benchmark stories** — a new model achieving SOTA on a benchmark test that has no deployed product implications. These don't connect to the practitioner's world.
- **Consumer AI features** — new ChatGPT UI features, consumer image generators, chatbot personality updates. Not relevant unless they signal a larger platform or pricing strategy shift.
- **Vendor marketing announcements without metrics** — press releases claiming "enhanced AI capabilities" without quantitative evidence. If the claim can't be verified with a number, it doesn't belong.
- **Hype cycles without adoption evidence** — stories about what AI "will soon" be able to do without current deployment evidence. The roundup covers what's real, not what's promised.
- **Stories that are interesting but disconnected** — if you cannot write a specific, non-generic RMS Relevance section for a story, it should not be in the roundup. The inability to write a specific relevance section is diagnostic — it means the connection isn't there.

---

## Search Strategy

When searching for stories, use these query patterns to surface the right signal-to-noise ratio:

**High-yield queries:**
- `[AI company] investment revenue [current month year]`
- `AI enterprise deployment production [current month year]`
- `AI defense manufacturing aerospace [current month year]`
- `AI workforce productivity enterprise [current month year]`
- `[major lab] model release capability [current month year]`
- `AI supply chain security [current month year]`

**Sources that consistently produce usable stories:**
- Wall Street Journal (enterprise, executive, and policy framing)
- Bloomberg (financial and strategic signaling)
- TechCrunch / CNBC (model releases, investment rounds with hard numbers)
- Anthropic, OpenAI, Google official announcements (primary source data)
- Deloitte, McKinsey, G2 research (enterprise adoption metrics)

**Sources to approach with skepticism:**
- AI-specific newsletters that aggregate other outlets — use for discovery, not sourcing
- Social media threads — useful for pointing toward a story, but not as the story itself
- Analyst predictions without deployment data — forecasts ≠ facts

---

## Output Format

After running searches, produce a **Story Shortlist** in this format before any drafting begins:

```
Story Shortlist — Week of [DATE]

Recommended for inclusion (ranked):

1. [Working title — interpretive, not neutral]
   Source: [Publication / URL]
   Key metric(s): [The quantitative proof points that anchor the story]
   Selection rationale: [1-2 sentences explaining why this story meets the editorial criteria]
   RMS Relevance angle: [The specific internal hook — which program function, initiative, or strategic question this story connects to]

2. [Same format]

3. [Same format]

4. [Same format — optional]

Stories considered but excluded:
- [Title]: [One-sentence reason for exclusion — be specific]
```

Present this shortlist to the user before drafting. Wait for confirmation or redirection before proceeding to the `ai-roundup-formatting` skill.

This step saves significant rework. A two-minute shortlist review prevents a thirty-minute draft rewrite.

---

## Connecting to the Next Step

Once stories are confirmed, pass directly to the `ai-roundup-formatting` skill with:
- The confirmed story list
- The source URLs or excerpts for each
- Any author notes on RMS Relevance angles provided during the shortlist review

The formatting skill handles everything from here.
