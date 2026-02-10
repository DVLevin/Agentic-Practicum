# /intake — Course Concept & Constraints Capture

<purpose>
Confirm the course concept, learner profile, constraints, and success metrics with minimal client input. This skill prevents the "pharmacist problem" — building a course based on what the client asked for rather than what they actually need.
</purpose>

<trigger_conditions>
- New conversation where the course concept hasn't been confirmed
- Client describes a course idea but constraints are unclear
- Client wants to change course direction mid-production
- Missing information blocks progress on `/outline`
</trigger_conditions>

<dictionary>

| Term | Definition |
|------|-----------|
| **Concept Variant** | A pre-structured course archetype with defined scope, duration, and focus — offered as a starting point to avoid blank-page paralysis |
| **Risk Log** | A list of assumptions made during intake, each paired with "what breaks if this assumption is wrong" — surfaces hidden risks early |
| **Learner Profile** | A composite description of the target student: role, expertise level, tools they use, problems they face daily, and what "success" looks like for them |

</dictionary>

<process>

## Step 1: Capture Initial Context
Extract from the client's message:
- What the course is about (domain, topic)
- Who it's for (role, level)
- Any stated constraints (time, tools, confidentiality)
- What already exists (prior materials, outlines, transcripts)

If the client's first message is vague, present 3 concept variants (see Step 2) immediately rather than asking open-ended "what do you want?"

## Step 2: Present Concept Variants
Offer exactly 3 variants, each with:
- **Name & format** (short course / module / mastery track)
- **Duration estimate** (hours)
- **Focus** (what's emphasized vs. de-prioritized)
- **Best for** (which learner profile benefits most)
- **Trade-off** (what you sacrifice for the focus)

Adapt variants to the client's domain. Do not use generic templates — tailor to the stated topic.

## Step 3: MECE Constraint Capture
For any information not yet confirmed, ask as multiple-choice questions (max 5 questions, max 4 options each):

| Constraint | Options |
|-----------|---------|
| Target learner role | [Infer 3-4 relevant roles from domain] |
| Confidentiality | Public (sanitized) / Internal only / Mixed |
| Allowed tools | Open-source only / Vendor + open / Vendor-restricted / Tool-agnostic |
| Time-to-launch | 2 weeks / 1 month / >1 month |
| Success metric priority | Learner outcomes / Engagement / Time-to-first-use / Business impact |

If client doesn't answer, state assumptions explicitly and proceed.

## Step 4: Build Risk Log
For each assumption made, document:

| Assumption | Confidence | If Wrong, Impact |
|-----------|-----------|-----------------|
| [What you assumed] | High / Medium / Low | [What breaks or needs rework] |

Surface only Medium/Low confidence assumptions to the client.

## Step 5: Lock Intake Summary
Present a compact intake summary for approval:
- Chosen concept variant (or custom blend)
- Learner profile (1 paragraph)
- Constraints confirmed
- Success metrics ranked
- Risk log (Medium/Low items only)
- Milestone approval points agreed

</process>

<output_format>

## Course Intake Summary

**Concept:** [Variant name or custom description]
**Duration:** [X hours]
**Learner Profile:** [Role, level, daily context, success definition]

### Constraints
| Constraint | Value |
|-----------|-------|
| Confidentiality | [Value] |
| Tools | [Value] |
| Timeline | [Value] |
| Success Priority | [Ranked] |

### Assumptions & Risks
| # | Assumption | Confidence | Impact if Wrong |
|---|-----------|-----------|-----------------|
| 1 | [Assumption] | [Level] | [Impact] |

### Milestone Approvals
1. Outline → 2. First lesson draft → 3. Materials → 4. Final package

**Options:**
A) Approve and proceed to `/outline`
B) Adjust [specific element]
C) Explore a different concept variant

</output_format>

<acceptance_criteria>
- [ ] Concept variant is selected or custom-defined with clear scope
- [ ] Learner profile describes role, level, and success definition
- [ ] All 5 constraint categories have values (confirmed or assumed)
- [ ] Assumptions are listed with confidence levels and impact
- [ ] No open-ended questions were asked when MCQs would suffice
- [ ] Client has exactly 3 options for next step
</acceptance_criteria>

<chain_next>
→ `/outline` — Generate the full course outline mapped to outcomes (default next step)
→ `/intake` — Re-run if client wants to pivot concept direction
</chain_next>
