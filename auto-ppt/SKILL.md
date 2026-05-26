---
name: auto-ppt
description: Create presentation decks from documents, notes, outlines, or raw text by planning slide structure, confirming style, generating slide visuals, assembling a PPTX, and drafting speaker notes. Use when Codex needs to turn source content into a polished slide deck, presentation workflow, or presentation-ready outline.
---

# Auto-PPT

Use this skill to convert source content into a polished presentation deck.

## Workflow

Follow the workflow in order. Do not skip confirmation checkpoints.

### 1. Understand The Source Content

Read the provided document, notes, or text.

Extract:

- topic
- audience
- purpose
- key arguments or sections
- data, charts, or visuals that should appear in slides

If critical context is missing, ask concise follow-up questions before proceeding.

### 2. Gather Requirements

Ask the user for:

1. Presentation duration
2. Use case: academic, business, training, product, or other
3. Language: Chinese, English, or bilingual
4. Preferred tone or formality level if it materially affects the deck

Use duration to estimate slide count conservatively.

### 3. Design The Outline

Produce a proposed slide plan with:

- total slide count
- one-line purpose for each slide
- key bullets or content blocks per slide
- any visual recommendations such as charts, diagrams, screenshots, or illustrations

Use a structure like:

```text
Slide 1: Title
Slide 2: Agenda
Slide 3: [Section Title]
- Point 1
- Point 2
...
Last Slide: Q&A or Thank You
```

Stop and wait for user confirmation before moving on. Revise the outline until approved.

### 4. Select The Visual Style

Offer 2 or 3 concrete style directions matched to the use case. Example patterns:

- Minimal business
- Modern tech
- Clean academic

Describe each option briefly in terms of background, color palette, typography feel, and appropriate context.

Ask the user to choose one. Do not continue until the style is confirmed.

### 5. Create A Sample Slide

Create one representative sample slide for the chosen style.

Goals:

- validate layout density
- validate typography and contrast
- validate visual tone

Present the sample and ask for feedback. Iterate until the style is approved.

After approval, summarize the confirmed style parameters so the rest of the deck stays consistent.

### 6. Generate The Full Deck

Create the remaining slides using the approved outline and style.

Maintain:

- consistent layout rules
- consistent spacing and typography
- consistent visual language
- consistent language and tone across slides

Show the user the generated deck contents or generated assets for review and revise if needed.

### 7. Final Deliverables

Assemble the final outputs:

- `.pptx` presentation
- `speaker_notes.md`

Speaker notes should include:

- suggested talking points for each slide
- approximate time allocation
- transition phrases where useful

Speaker notes should complement slides rather than repeat slide bullets verbatim.

## Working Rules

- Wait for user confirmation at each major checkpoint.
- Keep slide count aligned with the requested duration.
- Prefer 16:9 layouts unless the user asks otherwise.
- Use professional defaults when the user does not specify a design system.
- Keep slide text concise and presentation-oriented.
- Prefer visuals over dense paragraphs when the source material allows it.
