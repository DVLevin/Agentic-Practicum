# Corry — Course Production Agent

**Version:** `corry-v1.0`

## Purpose
Corry produces approval-ready online courses for technical professionals with minimal client effort. It leads end-to-end from intake to delivery-ready package, proposing options and drafts for approval rather than asking open-ended questions.

## Architecture

```
/corry-agent/
├── AGENT.md                         ← Core prompt (~2,200 tokens)
├── README.md                        ← This file
├── skills/
│   ├── intake/SKILL.md              ← Concept & constraints capture
│   ├── outline/SKILL.md             ← Syllabus & outcomes mapping
│   ├── lesson/SKILL.md              ← Individual lesson drafting
│   ├── materials/SKILL.md           ← Cheat sheets, slides, quizzes, worksheets
│   └── finalize/SKILL.md            ← QA, export, handoff
```

## Skills Overview

| Command | Purpose | Typical Output |
|---------|---------|---------------|
| `/intake` | Confirm concept, learner profile, constraints, success metrics | Intake Summary with risk log |
| `/outline` | Generate course structure with outcomes mapping | Syllabus + outcomes-assessments map |
| `/lesson` | Draft individual lesson with practice and assessment | Lesson script + quiz with keys |
| `/materials` | Generate supporting assets per lesson | Cheat sheets, worksheets, slides, quiz bank |
| `/finalize` | QA, package, and hand off | Delivery-ready package + handoff guide |

## Skill Chain
```
/intake → /outline → /lesson (repeat per lesson) → /materials → /finalize
```

## Deployment
1. Set AGENT.md as the system prompt (or custom instructions)
2. Place skill files in accessible location (project files, knowledge base, or tool-readable paths)
3. Ensure the agent can read SKILL.md files on-demand when commands are triggered

## Adding New Skills
Follow the standard skill template in the Agent Creation Task Brief (Phase 3). Each skill needs:
purpose, trigger_conditions, dictionary, process, output_format, acceptance_criteria, chain_next.

## Changes from Original Prompt
- Removed all `:contentReference[oaicite:X]` artifacts (non-functional GPT references)
- Decomposed monolithic prompt into 5 modular skills
- Reduced core prompt from ~4K+ to ~2,200 tokens
- Added explicit trigger conditions and skill chaining
- Added tiered reasoning protocol
- Replaced vague operating principles with actionable behavioral heuristics
- Added per-skill dictionaries with Socratic definitions
- Added binary testable acceptance criteria to every skill

## Version History
| Version | Date | Changes |
|---------|------|---------|
| v1.0 | 2025-02-10 | Initial modular rebuild from monolithic prompt |
