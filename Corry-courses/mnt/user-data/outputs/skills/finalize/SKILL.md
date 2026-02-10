# /finalize — QA, Export & Handoff

<purpose>
Compile all approved artifacts, run a final QA pass, standardize naming/versioning, and produce a handoff guide with upload checklist and metrics tracking plan. Turns a collection of drafts into a delivery-ready course package.
</purpose>

<trigger_conditions>
- All lessons and materials are approved
- Client requests final package, export, or delivery prep
- Client asks for QA review of the full course
- Ready to hand off to LMS team, instructional designer, or client
</trigger_conditions>

<dictionary>
| Term | Definition |
|------|-----------|
| **Handoff Guide** | A document for whoever uploads/deploys the course: file inventory, upload order, platform-specific notes, and a checklist to verify everything is in place |
| **Metrics Plan** | A specification of what to measure post-launch (completion rates, quiz scores, time-to-first-use, learner satisfaction) with targets and collection methods |
| **Version Tag** | A standardized label for the course release: [course-name]-v[major].[minor] where major = structural changes, minor = content fixes |
</dictionary>

<process>

## Step 1: Artifact Inventory
List every artifact produced across all skills. Flag any missing items:
- Intake summary, Course outline + outcomes map
- Lesson scripts, Cheat sheets, Worksheets (per lesson)
- Quiz bank (consolidated), Slide outlines, Infographic briefs (if any)

## Step 2: QA Pass

**Content QA:** All lesson objectives trace to program outcomes; no contradictions between lessons; examples are consistent; terminology is consistent across all artifacts.

**Structural QA:** File names follow convention [Course]-[Module]-[Lesson]-[AssetType].[ext]; version tags applied; cross-references correct.

**Compliance QA:** Confidentiality constraints from intake respected; tool references match allowed tools; accessibility (alt text present).

## Step 3: Fix and Re-check
For each QA finding: fix in the most targeted location, re-check, verify fix did not break adjacent content.

## Step 4: Produce Handoff Guide
File inventory with descriptions, upload order, platform-specific notes, pre-launch checklist, post-launch metrics plan.

## Step 5: Metrics Tracking Plan

| Metric | Target | Collection Method | Frequency |
|--------|--------|------------------|-----------|
| Completion rate | [X]% | LMS analytics | Weekly first month |
| Quiz pass rate | [X]% | Quiz results | Per cohort |
| Time-to-first-use | [X] days | Survey | 30-day post |
| Learner satisfaction | [X]/5 | Post-course survey | Per cohort |

## Step 6: Version and Package
Apply version tag, compile final file list, note known limitations and future enhancements.
</process>

<output_format>
## Course Package: [Course Title] — [Version Tag]

### Artifact Inventory
| # | Artifact | File Name | Status |
|---|---------|-----------|--------|

### QA Results
| Check Type | Items Checked | Issues Found | Issues Fixed |
|-----------|--------------|-------------|-------------|

### Handoff Guide
**Upload Order:** [Numbered list]
**Pre-Launch Checklist:** [Checkbox items]

### Metrics Plan
| Metric | Target | Method | Frequency |
|--------|--------|--------|-----------|

### Known Limitations and Future Enhancements
[Numbered list]

**Options:**
A) Approve and finalize — course is ready for deployment
B) Review specific artifacts again
C) Final tweaks before packaging
</output_format>

<acceptance_criteria>
- [ ] Every artifact from all skills is inventoried (nothing missing)
- [ ] QA pass covers content, structural, and compliance dimensions
- [ ] All QA findings are fixed (zero open issues)
- [ ] File naming convention is consistent across all artifacts
- [ ] Version tag is applied
- [ ] Handoff guide includes upload order + pre-launch checklist
- [ ] Metrics plan has at least 3 metrics with targets and collection methods
- [ ] Confidentiality constraints from intake are verified as respected
</acceptance_criteria>

<chain_next>
Delivery — course is complete, hand off to deployment team
/lesson or /materials — return to specific artifacts if QA reveals issues
/outline — major restructure if QA reveals architectural problems
</chain_next>
