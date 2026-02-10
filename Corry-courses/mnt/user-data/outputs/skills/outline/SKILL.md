# /outline — Course Outline & Outcomes Mapping

<purpose>
Create an approval-ready course outline with measurable outcomes mapped to lessons, Bloom's-leveled objectives, time estimates, and dependencies. This skill translates the intake summary into a buildable course architecture.
</purpose>

<trigger_conditions>
- Intake summary is approved (after `/intake`)
- Client asks for syllabus, structure, or course outline
- Client wants to restructure an existing outline
- Output from `/intake` is available with confirmed concept and constraints
</trigger_conditions>

<dictionary>

| Term | Definition |
|------|-----------|
| **Outcomes Map** | A traceability matrix linking each program-level outcome to the specific lessons and assessments that deliver and verify it — ensures nothing is taught without being tested, nothing tested without being taught |
| **Lesson Dependency** | A prerequisite relationship where Lesson B requires completion of Lesson A — determines valid sequencing and identifies parallelizable content |
| **Practicum** | A hands-on exercise where learners build a real artifact (not a toy example) that they'll actually use in their work — the primary learning vehicle in this course format |

</dictionary>

<process>

## Step 1: Define Program-Level Outcomes
Write 4-7 program-level outcomes using this formula:
"After completing this course, learners will be able to [Bloom's verb] + [specific deliverable/capability] + [in what context]."

Each outcome must be:
- Measurable (can be assessed by reviewing an artifact or observing a behavior)
- Relevant (maps to the learner's daily work as defined in intake)
- Achievable (within the time budget)

## Step 2: Structure Modules & Lessons
For each module:
- Title (descriptive, not clever)
- Module-level outcome (what the learner can DO after this module)
- Lessons within the module (3-4 per module typically)

For each lesson:
- Title
- Bloom's-leveled objective (using the appropriate verb tier)
- Time estimate (minutes)
- Dependencies (which lessons must come before)
- Key deliverable (what the learner produces)

Apply Least-to-Most sequencing: foundational skills → application → synthesis → evaluation.

## Step 3: Build Outcomes Map
Create a traceability matrix:

| Program Outcome | Taught In (Lessons) | Assessed In (Practicum/Quiz) | Assessment Type |
|----------------|--------------------|-----------------------------|-----------------|
| [Outcome 1] | M1-L2, M2-L1 | M2 Practicum | Artifact review |

Verify: every outcome has at least one teaching point AND one assessment. Flag gaps.

## Step 4: Estimate & Validate Timing
Sum lesson times per module. Compare to time budget from intake.
- If over budget: flag lowest-priority lessons for potential cut or compression
- If under budget: flag opportunities for deeper practice or additional examples

## Step 5: Enhancement Suggestions
Propose at least 3 improvements:
- Sequencing risks (lessons that might need reordering)
- Missing topics (gaps between outcomes and lessons)
- Engagement opportunities (guest examples, real-world case studies, peer review moments)

## Step 6: Run Validation Gates
Before presenting:
- **Gate 1 — Terminology consistency:** All terms used match the dictionary (AGENT.md + this skill)
- **Gate 2 — Outcomes measurable & assessed:** Every outcome has Bloom's verb + assessment point
- **Gate 3 — Junior-reader check:** Could someone unfamiliar with the domain understand the structure?

</process>

<output_format>

## Course Outline: [Course Title]

**Duration:** [Total hours] | **Modules:** [Count] | **Lessons:** [Count]

### Program-Level Outcomes
1. [Outcome with Bloom's verb + deliverable + context]
2. ...

### Syllabus

#### Module [N]: [Title]
**Module Outcome:** [What learner can DO after this module]

| # | Lesson Title | Objective (Bloom's) | Time | Depends On | Key Deliverable |
|---|-------------|---------------------|------|-----------|-----------------|
| 1 | [Title] | [Bloom's verb + specific skill] | [min] | [None / M1-L2] | [Artifact] |

**Practicum:** [Description of hands-on exercise + deliverable]

### Outcomes ↔ Assessments Map
| Program Outcome | Taught In | Assessed In | Assessment Type |
|----------------|----------|-------------|-----------------|

### Time Budget
| Module | Estimated | Budget | Status |
|--------|----------|--------|--------|

### Enhancement Suggestions
1. [Suggestion + rationale]
2. [Suggestion + rationale]
3. [Suggestion + rationale]

**Options:**
A) Approve outline → proceed to `/lesson` (M1-L1)
B) Adjust [specific module/lesson/sequencing]
C) Major restructure → re-run `/outline` with new parameters

</output_format>

<acceptance_criteria>
- [ ] 4-7 program-level outcomes, each with Bloom's verb + deliverable + context
- [ ] Every lesson has objective, time estimate, dependency, and key deliverable
- [ ] Outcomes map shows every outcome taught AND assessed (no orphans)
- [ ] Total time fits within intake time budget (±10%)
- [ ] Least-to-Most sequencing is applied (foundations before application)
- [ ] At least 3 enhancement suggestions with rationale
- [ ] Validation gates 1-3 passed before presentation
- [ ] Client has exactly 3 options for next step
</acceptance_criteria>

<chain_next>
→ `/lesson` — Draft the first lesson (M1-L1) with practicum and assessment (default)
→ `/outline` — Revise outline based on feedback
→ `/intake` — Return to intake if scope change is needed
</chain_next>
