---
name: narrative-logic-engine
description: Generate structured, internally coherent narrative or advocacy arguments with explicit assumptions, terminology, counterargument handling, a finished draft, and a reality check. Use for fictional worldbuilding, speculative science, rhetorical position papers, public-facing narrative framing, or analysis of self-sealing arguments; do not use to present unverified claims as facts, target people, or facilitate deception, harassment, or manipulation.
---

# Narrative Logic Engine

Build a transparent argument architecture, then turn it into prose. Treat coherence as a craft constraint, not evidence of truth.

## Gather the brief

Extract or ask only for missing material facts:

- **Core conclusion:** the claim, outcome, or world rule to develop.
- **Domain and audience:** e.g. hard-SF setting guide, fictional public statement, policy advocacy, or critical analysis.
- **Output mode:** `hybrid` by default; `draft` or `toolkit` on request.
- **Reality label:** `fiction`, `position`, or `analysis`.
- **Tone and length:** infer sensible defaults when absent.

State any invented premise plainly. If the request concerns real science, history, medicine, law, finance, people, or events, distinguish sourced facts from interpretation and unsupported assumptions. Do not fabricate citations, data, witnesses, consensus, or credentials.

## Choose the reasoning pattern

Use one or combine them, naming each premise rather than smuggling it in.

1. **Value-frame shift:** Define the relevant success criterion, explain why it matters to the stated audience, and retain trade-offs. Use for narrative framing and values disputes; never claim it disproves contrary facts.
2. **Counterfactual axiom:** Introduce one bounded fictional departure, derive implications consistently, and list observable consequences inside the setting. Use for speculative fiction; do not label it real science.
3. **Closed-loop diagnosis:** Map a claim, its assumed proof standard, its response to counterevidence, and what evidence could change its mind. Use to analyze circular reasoning, not to make it harder to challenge.

Avoid personal attacks, motive speculation, dogpiles, intimidation, evasion, or instructions to overwhelm, deceive, or silence critics. Replace adversarial "defense" with fair counterarguments and evidence thresholds.

## Build the logic map

Before drafting, produce:

1. **Reality label and scope** — fiction, stated position, or analysis; audience and intended use.
2. **Three foundation premises** — each marked `given`, `value judgment`, `fictional axiom`, or `requires evidence`.
3. **Definitions** — 5–8 concise terms; define terms for clarity, not exclusion or fake expertise.
4. **Inference chain** — show premise → intermediate rule → conclusion. Include at least one trade-off or limiting condition.
5. **Strongest objections** — steelman 3 plausible objections. For each, specify either a reasoned response, an uncertainty, or evidence that would resolve it.
6. **Falsifiability / revision trigger** — identify what would revise the claim. For fiction, give an in-universe consistency test; for a position, give an empirical or ethical condition.

## Produce the requested output

### Hybrid (default)

Return the logic map, followed by a publication-ready draft. The draft must faithfully use the map, avoid claiming assumptions are proven, and make the reality label legible in its opening or framing.

### Draft

Return only a coherent article or setting entry, but retain a brief premise note and a closing limitations note where relevant.

### Toolkit

Return the logic map and reusable language components: framing sentences, definitions, question prompts, and evidence requests. Never provide abuse, deception, or harassment scripts.

## Output schema

Use these headings unless the user requests another format:

```markdown
## Scope and reality label
## Foundation premises
## Working vocabulary
## Reasoning chain
## Objections and fair responses
## Revision triggers
## Finished draft
## Reality check
```

In `Reality check`, separate: established facts (with sources when available), assumptions, contested interpretations, and intentionally fictional elements. Omit `Finished draft` for toolkit mode and omit the prior sections for draft mode except concise premise/limitations notes.

## Quality gate

Before delivering, verify that the conclusion follows from disclosed premises; definitions do not secretly settle the dispute; counterarguments are represented fairly; uncertainty is visible; and the prose does not impersonate evidence or authority.
