---
name: narrative-logic-engine
description: Ingest user-provided text, images, video, transcripts, and notes to build a traceable, internally coherent world bible, logic map, and finished narrative or advocacy draft. Use for multimodal worldbuilding, speculative science, rhetorical position papers, public-facing narrative framing, or analysis of self-sealing arguments; do not use to present unverified claims as facts, target people, or facilitate deception, harassment, or manipulation.
---

# Narrative Logic Engine

Turn supplied material into a traceable world model and then into prose. Treat coherence as a craft constraint, not evidence of truth. Begin every corpus-driven output with: “This model is based only on the material available in this task; it is not persistent learning or training.”

## Ingest the corpus

Accept notes, documents, pasted text, images, video, transcripts, captions, and links or file references supplied by the user. Inventory every item before inference:

| ID | Medium | Direct observation / quotation | Interpretation | Confidence | Open question |
|---|---|---|---|---|---|

Use the available file and vision tools to inspect attachments. Cite a locator for each item: text `S1 p. 3` or `S1 ¶4`; image `S2, upper-left`; video `S3 @00:42`; transcript `S3 @00:42–00:49`.

For video, use the supplied transcript, captions, timestamps, and representative frames when available. If direct inspection fails, use this fallback order: supplied transcript → captions → timestamped screenshots/keyframes → user summary. State the available level and request the next useful artifact. Never invent unseen scenes, dialogue, or details.

Keep three layers separate:

- **Source evidence:** directly stated, visible, or audible material, with its source ID.
- **Inference:** a plausible reading of one or more sources, with confidence and alternatives.
- **World rule:** an adopted premise needed to make the setting or position operational; mark it as `fictional axiom`, `value judgment`, or `requires evidence`.

Treat concept art as evidence of visible design only, unless the user explicitly declares it canon. Do not infer physics, history, character identity, or authorial intent from it without labeling the inference.

Resolve contradictions by preserving both readings, identifying the conflict, and proposing the smallest explicit bridge rule. Rank material only by user-declared canon status, directness, and source specificity; if no priority is supplied, retain both as unresolved. Never silently overwrite a user source.

## Build the world model

Extract and connect:

1. **Entities and actors** — people, groups, places, objects, technologies, forces, and institutions.
2. **Claims and events** — who asserts what, when, where, and with what source support.
3. **Rules and constraints** — physical, social, economic, ethical, or narrative limits.
4. **Causality and timeline** — cause → effect links, dependencies, turning points, and unresolved gaps.
5. **Motivations and stakes** — only where supported or explicitly proposed as a fictional choice.

Create a compact world bible containing a glossary, timeline, relationship map in text, active rules, contradictions, and canon status. Label each item `canonical source`, `supported inference`, `working hypothesis`, or `creative addition`.

## Choose the reasoning pattern

Use one or combine them, naming each premise rather than smuggling it in.

1. **Value-frame shift:** Define the relevant success criterion, explain why it matters to the stated audience, and retain trade-offs. Never claim it disproves contrary facts.
2. **Counterfactual axiom:** Introduce one bounded fictional departure, derive implications consistently, and list observable consequences inside the setting. Do not label it real science.
3. **Closed-loop diagnosis:** Map a claim, its assumed proof standard, its response to counterevidence, and what evidence could change its mind. Use this to analyze circular reasoning, not to make it harder to challenge.

Avoid personal attacks, motive speculation, dogpiles, intimidation, evasion, or instructions to overwhelm, deceive, or silence critics. Replace adversarial “defense” with fair counterarguments and evidence thresholds.

## Build the logic map

After the corpus model, produce:

1. **Scope and reality label** — fiction, stated position, or analysis; audience and intended use.
2. **Foundation premises** — three or more, each traced to a source ID or marked as an addition.
3. **Working vocabulary** — 5–8 terms defined for clarity, not exclusion or fake expertise.
4. **Inference chain** — premise → intermediate rule → conclusion, including at least one trade-off or limit.
5. **Strongest objections** — steelman three plausible objections; give a reasoned response, uncertainty, or resolving evidence for each.
6. **Revision triggers** — what new source, observation, or in-world consistency failure would revise the model.

## Produce the requested output

For a new multimodal corpus with no explicit output request, default to `world-bible` so the user can approve canon before prose is generated. Use `hybrid` when the user asks for both a model and a draft; use `toolkit` for structured language components, and `draft` for a finished piece with a concise premise note and limitations note.

Use these headings unless the user requests another format:

```markdown
## Corpus ledger
## World bible
## Scope and reality label
## Foundation premises
## Working vocabulary
## Reasoning chain
## Objections and fair responses
## Revision triggers
## Finished draft
## Reality check
```

In `Reality check`, separate established facts, source-backed observations, assumptions, contested interpretations, and intentionally fictional elements. Cite source IDs rather than inventing citations.

## Quality gate

Before delivering, verify that every key inference is traceable or labeled as creative; no conflicting source was silently discarded; the conclusion follows from disclosed premises; definitions do not secretly settle the dispute; counterarguments are represented fairly; uncertainty is visible; and prose does not impersonate evidence or authority.
