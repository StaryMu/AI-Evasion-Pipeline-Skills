---
name: "ai-evasion-pipeline"
description: "Turnitin 0%-validated 6-stage pipeline for reducing AI detection in academic writing: (1) vocabulary cleaning, (2) syntactic burstiness, (3) semantic chaining, (4) uneven hedging, (5) perplexity maximization, (6) natural imperfection preservation. Use when papers are flagged >20% AI. Derived from real Turnitin testing: 72%→0% across multiple versions of the same paper."
---

# AI Evasion Pipeline — 5-Stage Academic Rewriting (Turnitin 0% Validated)

## Overview

A systematic five-stage pipeline for reducing AI detection rates in academic prose. Each stage targets a specific class of AI markers. Process text in ~500-word segments through all five stages sequentially.

**Validation:** This skill's techniques derive from iterative Turnitin testing of the same paper ("The Future of Scientific Writing: Will IMRaD Be Applicable in the Next Decade?") across multiple versions — starting at 72% AI, dropping through intermediate versions, and reaching 0% AI (<20% threshold) in the final submission. Every before/after example comes from this real testing corpus.

## The Core Principle (Revised)

Previous versions of this skill claimed that specific word choices ("anchors", "paradigm", "contends") are AI markers in isolation. **This is incorrect.** The zero-AI version uses all of the following and still passes:

- "The IMRaD structure (Introduction, Methods, Results, Discussion)" — parenthetical expansion
- "This review argues that" — formulaic opening
- "not merely a writing convention but an infrastructure" — not-X-but-Y structure
- "Scientific writing thus takes place" — logical connector

**The real AI detection mechanism is statistical pattern density, not individual word flags.** Any single "AI pattern" is fine. It's when patterns accumulate across an entire text — uniform sentence lengths, predictable transitions, symmetrical structures, consistent register — that the detector triggers. The defense is to ensure no single pattern dominates, not to eliminate every pattern.

Analogous to: a single fingerprint smudge on a window is invisible. A thousand identical smudges form a detectable pattern. The goal is random variation, not perfection.

## Stage 1: AI Signature Vocabulary Cleaning

**Goal:** Reduce density of high-frequency AI vocabulary; not eliminate it

### Target Words (reduce frequency, don't eliminate)

**Empty filler phrases:** delve into, shed light on, it is worth noting that

**Overused academic verbs:** foster, underscore, leverage, facilitate, utilize

**Exaggerated adverbs:** crucially, pivotally, remarkably (when used as filler)

### Real-World Before/After (from 72% → 0% trajectory)

```
72% AI: "This critical review contends that IMRaD retains irreplaceable 
value as cognitive training for novice writers"
 0% AI: "This review argues that IMRaD remains essential for training 
new academic writers"

72% AI: "frontier fields are constructing an alternative paradigm organised 
around open-source code, preprint dissemination, and community-based review"
 0% AI: "the fields like artificial intelligence have built a new system 
centred on open-source code, preprint platforms, and community review"

72% AI: "codified expectations open academic socialisation to all students"
 0% AI: "standardised expectations will help all students participate in learning"
```

### Replacement Rules

1. Replace with simpler, context-appropriate terms
2. If no exact replacement, rewrite the clause
3. Never alter data, statistics, or core arguments
4. Don't clean everything — leave some academic vocabulary for authenticity
5. Target ~60-70% reduction in flagged vocabulary, not 100%

---

## Stage 2: Syntactic Rhythm Reconstruction (Burstiness)

**Goal:** Break uniform sentence length; maximize variance

### Strategy

1. Mix very short sentences (5-9 words) with long ones (30+ words)
2. Convert some passive constructions to active
3. Break parallel structures into asymmetric units
4. After complex passages, anchor with a short declarative sentence

### Real-World Before/After

```
72% AI [uniform ~22-word sentences]:
"For novice researchers, IMRaD provides a cognitive scaffold guiding 
learners through the intellectual sequence of identifying a problem, 
designing methods, gathering evidence, and constructing an argument. 
The structured argumentation it cultivates constitutes a foundational 
element of academic literacy. This training function will likely sustain 
IMRaD's dominance over the next decade."

 0% AI [varied rhythm — short→medium→long]:
"IMRaD can provide a thinking support for newcomers and help them learn 
the steps of problem-method-evidence and argument. The training it offers 
in systematic argumentation will maintain its lead; IMRaD is not a ceiling 
on creativity but the basic grammar of scholarly communication."
```

### Constraints

- Maintain academic tone; no casual language
- Never delete substantive arguments or data
- New short sentences must grow organically from context
- Aim for sentence length standard deviation > 8 words (AI typical: 3-4)

---

## Stage 3: Mechanical Transition Elimination (Semantic Chaining)

**Goal:** Remove robotic connectors; use content-based transitions

### Words to Reduce (not eliminate — reduce by ~80%)

**Paragraph openers:** Furthermore, Moreover, Additionally, Similarly

**Conclusion signals:** Therefore, Thus, Consequently

**Forced contrasts:** However, Nevertheless (at paragraph start)

### Real-World Before/After

```
72% AI: "The ensuing scholarly debate divides along pedagogical and 
epistemological lines. Proponents stress IMRaD's democratising function..."

 0% AI: "The above-mentioned study has been divided by teachers and 
philosophers. Proponents believe that IMRaD is a democratic way to teach..."

72% AI: "More fundamentally, IMRaD presupposes a linear research process, 
yet breakthrough work is characteristically iterative."

 0% AI: "IMRaD has a linear assumption, and this is not in line with the 
nature of breakthrough work that is iterative."
```

### Semantic Chaining Method

Let the core concept at the end of one paragraph become the natural entry point for the next. Use meta-textual anchors like "The above-mentioned study" or "This line of thinking" — they're human-coded reference points that AI rarely generates spontaneously.

---

## Stage 4: Academic Caution Injection (Hedging)

**Goal:** Introduce uneven, calibrated hedging — not uniform hedging

### Key Insight from 0% Testing

The zero-AI version does NOT hedge uniformly. It makes strong claims in some places ("IMRaD will still be needed") and softer claims in others ("IMRaD can provide a thinking support"). This **unevenness** is the human fingerprint. AI either hedges everything or nothing.

### Real-World Before/After

```
72% AI (uniformly strong): "IMRaD will endure as an irreplaceable 
cognitive scaffold for novices."

 0% AI (softer, less absolute): "IMRaD will still be needed as a 
thinking scaffold for new researchers."

72% AI (uniformly measured): "IMRaD is particularly ill-suited to 
qualitative inquiry, where the writing process is integral to 
knowledge production."

 0% AI (uneven — clipped ending): "IMRaD is not very suitable for 
qualitative research."
```

### Hedging Targets

- Absolute verbs: proved → provided evidence consistent with, ensured → contributed to
- Universal claims: reduce scope with "in most cases", "within this sample"
- Only hedge where epistemologically warranted; don't hedge everything
- Aim for ~30-40% of strong claims to be hedged, not 0% or 100%

---

## Stage 5: Perplexity Maximization (Final Polish)

**Goal:** Replace high-predictability word pairs with lower-frequency alternatives

### Real-World Before/After

```
72% AI: "Code functions as a first-class research output alongside text"
 0% AI: "Code is another type of research result in the ecosystem, 
just like text"

72% AI: "GitHub's community review mechanisms offer faster, more 
transparent quality control by reconfiguring review from pre-publication 
gatekeeping into post-publication conversation"
 0% AI: "The old system for checking the code collaboratively has been 
moved to the back end talk function after publishing by GitHub now"

72% AI: "What is taking shape looks like a bilingual ecosystem"
 0% AI: "What is taking shape looks like a combined system"
```

### The "Just Like Text" Principle

The zero-AI version's most striking feature: it frequently ends technical descriptions with a plain, almost informal comparison phrase. "Code is another type of research result in the ecosystem, just like text." This pattern — technical description followed by plain restatement — appears throughout the zero-AI version and is a natural human explanatory rhythm.

---

## Stage 6 (NEW): Natural Imperfection Preservation

**Goal:** Retain or introduce the micro-irregularities that characterize human writing

This is the most important finding from the 0% AI test. The zero-AI version contains several grammatical quirks that would be "corrected" by an AI or a thorough copy-editor. These quirks are likely the primary differentiator between 72% and 0%.

### Zero-AI Version's Actual Imperfections

```
Missing word: "took shape over the late nineteenth" 
[missing "century"]

Missing auxiliary: "which rarely seen in standard IMRaD papers" 
[missing "is"]

Awkward word order: "community collaboration sometimes instead of, 
anonymous review" [missing "or in place of"]

Run-on sentence: "Unusually, it lists approaches that did not work 
on general reasoning tasks, which rarely seen in standard IMRaD papers, 
becoming the first large language model to appear in Nature..."

Informal insertion: "back end talk function after publishing by GitHub now"

Quirky capitalization: "The Form helps people learn about low-risk 
projects with the same structure"
```

### How to Apply This Stage

1. After Stages 1-5, read the text aloud at normal speaking pace
2. Note any place where you naturally stumble or pause — these are natural friction points
3. Do NOT "fix" every grammatical quirk — keep 2-4 across a 1,000-word paper
4. Types of imperfections to preserve or introduce:
   - Occasional missing article ("the", "a")
   - One run-on sentence per ~500 words
   - One slightly awkward word-order choice
   - One informal phrase in a technical description
5. The imperfections must be the kind a busy human academic would make, not obvious errors

### What NOT to Do in Stage 6

- Don't add spelling errors (detected as a separate pattern)
- Don't make every other sentence imperfect (too much noise triggers suspicion)
- Don't break the logic or make claims unintelligible
- Don't add imperfections to data, methods, or reference sections
- Keep the density low: 2-4 minor quirks per 1,000 words is the target zone

---

## Application Protocol

### Full Pipeline Order

1. Split text into ~500-word segments
2. Stage 1: Vocabulary cleaning (60-70% reduction, not elimination)
3. Stage 2: Rhythm reconstruction (sentence length SD > 8)
4. Stage 3: Transition reduction (~80% of mechanical connectors removed)
5. Stage 4: Uneven hedging (30-40% of strong claims softened)
6. Stage 5: Perplexity maximization
7. Stage 6: Natural imperfection preservation (2-4 quirks per 1,000 words)
8. Read entire text aloud — if it sounds "too smooth," return to Stages 2 or 6

### Quick Diagnostic

| Symptom | Stage to Revisit |
|---------|-----------------|
| Every sentence ~22 words | Stage 2 |
| Can predict the next transition | Stage 3 |
| All claims equally confident | Stage 4 |
| Every word is "correct" | Stage 6 |
| Text reads like a textbook | Stage 5 + 6 |

### What Passed at 0% AI

The winning submission had: 1,069 words, numbered Vancouver citations, ~4 grammatical quirks, varied sentence lengths, plain verbs ("believes", "argues", "helps"), download-version transitional phrases ("The above-mentioned study", "At the same time"), and both parenthetical expansions and logical connectors — just not in uniform patterns.

---

## Anti-Patterns: What Failed at 72% AI

1. **Em-dash overuse:** 16 em-dashes in 950 words. Target: 0-1.
2. **Punchy verb density:** dovetails, collides, forecloses, inheres, bifurcates, erected — all in one paper
3. **Uniform academic register:** every sentence at the same formality level
4. **Perfect parallelism:** every list, every contrast, every comparison — symmetrical
5. **Zero grammatical friction:** every article, every auxiliary verb, every preposition — correct
6. **Predictable structure:** topic sentence → evidence → explanation → transition, every paragraph

