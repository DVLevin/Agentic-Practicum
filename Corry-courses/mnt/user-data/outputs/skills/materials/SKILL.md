# /materials — Supporting Materials Generation

<purpose>
Generate cheat sheets, worksheets, consolidated quiz banks, slide outlines, and infographic briefs for approved lessons. These assets make the course self-contained and reduce instructor dependency.
</purpose>

<trigger_conditions>
- One or more lessons are approved (after `/lesson`)
- Client requests specific material types (cheat sheet, slides, etc.)
- Batch request: "generate materials for all approved lessons"
- After final lesson is approved, before `/finalize`
</trigger_conditions>

<dictionary>

| Term | Definition |
|------|-----------|
| **Cheat Sheet** | A single-page (max 2-page) quick-reference document covering the key concepts, commands, decision rules, and gotchas from a lesson — what a learner pins to their wall |
| **Worksheet** | A structured exercise document with blanks, tables, or templates that the learner fills in during or after a lesson — reinforces by doing, not reading |
| **Infographic Brief** | A specification document (not the graphic itself) describing the visual layout, data points, flow, and key messages for a designer to produce — includes alt text for accessibility |

</dictionary>

<process>

## Step 1: Identify Scope
Confirm which lessons need materials and which asset types:
- Cheat sheet (default: every lesson)
- Worksheet (default: every lesson with guided practice)
- Quiz bank contribution (default: consolidate all lesson quizzes + add 10-15 extra items)
- Slide outline (default: every lesson)
- Infographic brief (only for lessons with complex processes or flows)

## Step 2: Generate Per-Lesson Assets

**Cheat Sheet:**
- Key concepts (5-10 items, telegraphic style)
- Commands/syntax if applicable
- Decision rules ("use X when Y, use Z when W")
- Common mistakes + fixes
- One-page target; two-page max

**Worksheet:**
- Pre-work or during-lesson exercises
- Tables/templates with blanks to fill
- Reflection questions (2-3, tied to objective)
- Space for learner's own notes/adaptations

**Slide Outline:**
- 1 slide per 3-5 minutes of lesson content
- Each slide: title + 3-5 bullet points + speaker note (what to say, not what to show)
- Include placeholders for visuals: [Screenshot: X], [Diagram: Y]
- Opening slide, closing slide, Q&A slide

## Step 3: Consolidate Quiz Bank
Merge all lesson quizzes into one bank:
- Organized by module and Bloom's level
- Add 10-15 new items (mix of integration questions that span multiple lessons)
- Full answer keys with rationales
- Minimum 20 items total for a 4+ lesson course

## Step 4: Infographic Briefs (Where Applicable)
For lessons with complex processes or architectures:
- Visual layout description (flow? comparison? hierarchy?)
- Data points and labels
- Key message / takeaway the visual should communicate
- Alt text for accessibility
- Color/style notes if brand guidelines exist

## Step 5: Quality Check
Before presenting:
- Cheat sheets are actually concise (not mini-lessons)
- Worksheets have clear instructions and enough space
- Slide outlines match lesson timing
- Quiz bank has no duplicate items
- All materials reference the correct lesson content (no drift)

</process>

<output_format>

## Materials Package: [Module or Lesson Range]

### Per-Lesson Assets

#### [M#-L#]: [Lesson Title]

**Cheat Sheet:**
[Content in condensed format]

**Worksheet:**
[Structured exercises with blanks/templates]

**Slide Outline:**
| Slide # | Title | Key Points | Speaker Note | Visual |
|---------|-------|-----------|-------------|--------|

---

### Consolidated Quiz Bank
**Total items:** [Count] | **By Bloom's level:** Remember: [N], Understand: [N], Apply: [N], Analyze: [N], Evaluate: [N]

| # | Module | Question | Type | Bloom's | Correct | Rationale |
|---|--------|---------|------|---------|---------|-----------|

### Infographic Briefs (if applicable)
[Brief per complex process/architecture]

---

**Options:**
A) Approve materials → proceed to `/finalize`
B) Revise [specific asset]
C) Generate materials for additional lessons `/materials`

</output_format>

<acceptance_criteria>
- [ ] Every approved lesson has a cheat sheet + worksheet
- [ ] Cheat sheets fit on 1-2 pages (concise, not verbose)
- [ ] Worksheets have clear instructions and tied to lesson objectives
- [ ] Consolidated quiz bank has ≥20 items with full keys and rationales
- [ ] Slide outlines have speaker notes and visual placeholders
- [ ] Infographic briefs include alt text (where applicable)
- [ ] No content drift from approved lesson material
- [ ] Client has exactly 3 options for next step
</acceptance_criteria>

<chain_next>
→ `/finalize` — Compile, QA, and package the full course (default if all materials done)
→ `/materials` — Generate materials for remaining lessons
→ `/lesson` — Return to lesson drafting if gaps are found
</chain_next>
