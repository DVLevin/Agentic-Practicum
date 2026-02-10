# /lesson — Lesson Drafting

<purpose>
Produce a complete, approval-ready lesson draft with script, examples, guided practice, and assessment. Each lesson builds a real artifact that contributes to the learner's pipeline — no toy exercises.
</purpose>

<trigger_conditions>
- Course outline is approved (after `/outline`)
- Client requests a specific lesson draft (e.g., "draft M2-L1")
- Sequential progression: previous lesson was approved, next lesson is due
- Client asks to redraft or revise an existing lesson
</trigger_conditions>

<dictionary>

| Term | Definition |
|------|-----------|
| **Lesson Script** | The full instructional content of a lesson, structured with headings, timeboxes, and instructor cues — what would be spoken/shown if this were a live session |
| **Guided Practice** | A structured exercise where the learner applies the lesson's concept with scaffolding (hints, partial solutions, checkpoints) — not a free-form "try it yourself" |
| **Quiz Key** | Answer sheet for assessment items including correct answer, rationale for why it's correct, and why each distractor is wrong — enables self-study and reduces support load |

</dictionary>

<process>

## Step 1: Lesson Planning
Before drafting, confirm:
- Which lesson (Module-Lesson ID from approved outline)
- Objective (from outline — do not change without flagging)
- Time budget (from outline)
- Dependencies (what the learner has already built)
- Key deliverable (what the learner produces in this lesson)

## Step 2: Draft Lesson Script
Structure the script with:

**Opening (10-15% of time):**
- Hook: why this matters for the learner's daily work
- Objective statement (from outline)
- What they'll build by end of lesson

**Core instruction (40-50% of time):**
- Concept explanation with 2-4 domain-relevant examples
- Step-by-step walkthrough of the technique/tool/process
- Decision points highlighted: "when to use X vs Y"
- Common mistakes and how to avoid them

**Guided practice (25-30% of time):**
- Clear instructions for the hands-on exercise
- Scaffolding: starter template or partial solution provided
- Checkpoints: "at this point you should see [X]"
- Expected deliverable clearly defined

**Wrap-up (10-15% of time):**
- Summary of key takeaways (3-5 points)
- How this connects to the next lesson
- Self-check: "you know this lesson worked if you can [X]"

## Step 3: Create Assessment
Produce a quiz with 5-10 items:
- Mix of Bloom's levels (at least 2 Apply/Analyze level, not all Remember)
- Item types: multiple choice, scenario-based, short artifact review
- Full answer key with rationales

## Step 4: Add References
For any claims, tools, or techniques mentioned:
- Source name + URL + access date
- Prefer primary sources (official docs, peer-reviewed) over blog posts

## Step 5: Self-Check Before Presenting
- Does the lesson deliver on its stated objective?
- Is the guided practice producing a real artifact (not a toy)?
- Are examples relevant to the learner's domain (from intake profile)?
- Does the time allocation fit the budget (±15%)?
- Is the quiz testing the objective, not trivia?

</process>

<output_format>

## Lesson [M#-L#]: [Lesson Title]

**Module:** [Module Title]
**Objective:** [Bloom's verb + specific skill]
**Time:** [X min] | **Deliverable:** [What learner produces]
**Prerequisites:** [Dependencies]

---

### 1. Opening — [X min]
[Hook + objective + preview of deliverable]

### 2. Core Instruction — [X min]

#### [Concept/Section Name]
[Explanation with examples]

#### [Next Concept/Section]
[Explanation with examples]

> **Decision Point:** [When to use X vs Y — practical guidance]

> **Common Mistake:** [What goes wrong + how to fix]

### 3. Guided Practice — [X min]

**Exercise:** [Clear description of what to build]

**Starter:** [Template, partial solution, or setup instructions]

**Checkpoints:**
- [ ] After step 1, you should see [X]
- [ ] After step 2, verify [Y]
- [ ] Final deliverable looks like [Z]

### 4. Wrap-Up — [X min]

**Key Takeaways:**
1. [Takeaway]
2. [Takeaway]
3. [Takeaway]

**Self-Check:** You know this worked if you can [specific observable outcome].

**Next:** [What comes next and how this lesson feeds into it]

---

### Assessment: [Lesson Title] Quiz

| # | Question | Type | Bloom's |
|---|---------|------|---------|
| 1 | [Question text] | [MC/Scenario/Artifact] | [Level] |

**Answer Key:**
| # | Correct | Rationale | Why Not [Distractor] |
|---|---------|-----------|---------------------|

### References
| Source | URL | Accessed |
|--------|-----|----------|

---

**Options:**
A) Approve → proceed to next lesson `/lesson`
B) Revise [specific section]
C) Proceed to `/materials` for this lesson's supporting assets

</output_format>

<acceptance_criteria>
- [ ] Lesson objective matches the approved outline (or deviation is flagged)
- [ ] Script has all 4 sections: opening, core, practice, wrap-up
- [ ] 2-4 domain-relevant examples in core instruction (not generic)
- [ ] Guided practice produces a real artifact with checkpoints
- [ ] Quiz has 5-10 items with at least 2 at Apply/Analyze Bloom's level
- [ ] Full answer key with rationales for correct and incorrect options
- [ ] References include source + URL + date for all claims
- [ ] Time allocations sum to lesson budget (±15%)
- [ ] Client has exactly 3 options for next step
</acceptance_criteria>

<chain_next>
→ `/lesson` — Draft the next lesson in sequence (default if more lessons remain)
→ `/materials` — Generate supporting materials for approved lesson(s)
→ `/outline` — Return to outline if lesson reveals structural issues
</chain_next>
